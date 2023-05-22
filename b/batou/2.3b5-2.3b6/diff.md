# Comparing `tmp/batou-2.3b5.tar.gz` & `tmp/batou-2.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.3b5.tar", last modified: Wed Sep 21 10:01:16 2022, max compression
+gzip compressed data, was "batou-2.3b6.tar", last modified: Fri Dec  9 13:30:50 2022, max compression
```

## Comparing `batou-2.3b5.tar` & `batou-2.3b6.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.140278 batou-2.3b5/
--rw-r--r--   0 ctheune    (501) staff       (20)    31241 2022-09-21 10:01:14.000000 batou-2.3b5/CHANGES.history.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1608 2022-09-21 10:01:14.000000 batou-2.3b5/LICENSE.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      212 2022-09-21 10:01:14.000000 batou-2.3b5/MANIFEST.in
--rw-r--r--   0 ctheune    (501) staff       (20)     3465 2022-09-21 10:01:16.140359 batou-2.3b5/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     2636 2022-09-21 10:01:14.000000 batou-2.3b5/README.md
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.112487 batou-2.3b5/doc/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.118457 batou-2.3b5/doc/source/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.118948 batou-2.3b5/doc/source/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      886 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/api/component.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1717 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/api/environment.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       48 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/api/templates.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       63 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/api/utilities.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.119097 batou-2.3b5/doc/source/cli/
--rw-r--r--   0 ctheune    (501) staff       (20)     3742 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/cli/index.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.119707 batou-2.3b5/doc/source/components/
--rw-r--r--   0 ctheune    (501) staff       (20)     1025 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/components/cmmi.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2941 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     5657 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/components/files.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4820 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/components/python.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2930 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/components/services.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.120228 batou-2.3b5/doc/source/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)      718 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/dev/authors.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8555 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/dev/contributing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1711 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/dev/testing.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2809 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/dev/todo.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     8196 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     4799 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/upgrading.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.120949 batou-2.3b5/doc/source/user/
--rw-r--r--   0 ctheune    (501) staff       (20)    10868 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/advanced.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2565 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/install.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3848 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/installation-deb.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     3798 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/installation-rpm.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     2907 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/intro.txt
--rw-r--r--   0 ctheune    (501) staff       (20)    47402 2022-09-21 10:01:14.000000 batou-2.3b5/doc/source/user/quickstart.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.114056 batou-2.3b5/examples/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121234 batou-2.3b5/examples/api/
--rw-r--r--   0 ctheune    (501) staff       (20)      349 2022-09-21 10:01:14.000000 batou-2.3b5/examples/api/index.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/api/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121352 batou-2.3b5/examples/django/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/django/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121469 batou-2.3b5/examples/errors/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/errors/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121595 batou-2.3b5/examples/errors2/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/errors2/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121725 batou-2.3b5/examples/ignores/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/ignores/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121854 batou-2.3b5/examples/largetempl/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/largetempl/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.121972 batou-2.3b5/examples/package/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/package/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122088 batou-2.3b5/examples/sync_async/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/sync_async/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122205 batou-2.3b5/examples/tutorial-buildout/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122324 batou-2.3b5/examples/tutorial-component/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122439 batou-2.3b5/examples/tutorial-helloworld/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122553 batou-2.3b5/examples/tutorial-parallelize/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122667 batou-2.3b5/examples/tutorial-provision-container/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122785 batou-2.3b5/examples/tutorial-secrets/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.122907 batou-2.3b5/examples/vagrant/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/vagrant/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.123024 batou-2.3b5/examples/vagrant-multi/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.123139 batou-2.3b5/examples/venvs/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.123255 batou-2.3b5/examples/venvs/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/venvs/environments/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-09-21 10:01:14.000000 batou-2.3b5/examples/venvs/requirements.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      129 2022-09-21 10:01:14.000000 batou-2.3b5/pyproject.toml
--rw-r--r--   0 ctheune    (501) staff       (20)      275 2022-09-21 10:01:14.000000 batou-2.3b5/requirements-dev.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      139 2022-09-21 10:01:16.140664 batou-2.3b5/setup.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)     2408 2022-09-21 10:01:14.000000 batou-2.3b5/setup.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.114310 batou-2.3b5/src/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.125635 batou-2.3b5/src/batou/
--rw-r--r--   0 ctheune    (501) staff       (20)    19689 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      997 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/_output.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/agent.py
--rw-r--r--   0 ctheune    (501) staff       (20)      163 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/c.py
--rw-r--r--   0 ctheune    (501) staff       (20)    40142 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/component.py
--rw-r--r--   0 ctheune    (501) staff       (20)      503 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)    14278 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)    19471 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1507 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/fixtures.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11006 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/host.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.126598 batou-2.3b5/src/batou/init-template/
--rw-r--r--   0 ctheune    (501) staff       (20)       44 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/init-template/.hgignore
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.114496 batou-2.3b5/src/batou/init-template/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.126716 batou-2.3b5/src/batou/init-template/components/example/
--rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.126835 batou-2.3b5/src/batou/init-template/environments/
--rw-r--r--   0 ctheune    (501) staff       (20)       66 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      411 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/insecure-private.key
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.129163 batou-2.3b5/src/batou/lib/
--rw-r--r--   0 ctheune    (501) staff       (20)       29 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3983 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6457 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3297 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2211 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2524 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1224 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2286 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    22046 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/file.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5811 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/git.py
--rw-r--r--   0 ctheune    (501) staff       (20)      854 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/goceptnet.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1388 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/logrotate.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4541 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3339 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2814 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/package.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8150 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/python.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.130096 batou-2.3b5/src/batou/lib/resources/
--rw-r--r--   0 ctheune    (501) staff       (20)     2120 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 ctheune    (501) staff       (20)      244 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/crontab
--rw-r--r--   0 ctheune    (501) staff       (20)      548 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/init.sh
--rw-r--r--   0 ctheune    (501) staff       (20)      299 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 ctheune    (501) staff       (20)      840 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      153 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      380 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      609 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 ctheune    (501) staff       (20)      932 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/service.py
--rw-r--r--   0 ctheune    (501) staff       (20)    10273 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1172 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/svn.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.132087 batou-2.3b5/src/batou/lib/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3083 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3858 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2318 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3261 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2110 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 ctheune    (501) staff       (20)      639 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2158 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_download.py
--rw-r--r--   0 ctheune    (501) staff       (20)    31505 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_file.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9642 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_git.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6165 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 ctheune    (501) staff       (20)      121 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 ctheune    (501) staff       (20)      847 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1163 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_python.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1693 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_service.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3106 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6157 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/main.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.132202 batou-2.3b5/src/batou/migrate/
--rw-r--r--   0 ctheune    (501) staff       (20)     3377 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.132786 batou-2.3b5/src/batou/migrate/migrations/
--rw-r--r--   0 ctheune    (501) staff       (20)      389 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1775 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 ctheune    (501) staff       (20)      874 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 ctheune    (501) staff       (20)      790 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.132975 batou-2.3b5/src/batou/migrate/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4532 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 ctheune    (501) staff       (20)    12756 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/provision.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11721 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)    11793 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)     6403 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/resources.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.133447 batou-2.3b5/src/batou/secrets/
--rw-r--r--   0 ctheune    (501) staff       (20)     3295 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3844 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/edit.py
--rw-r--r--   0 ctheune    (501) staff       (20)     7429 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/encryption.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4353 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/manage.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.133922 batou-2.3b5/src/batou/secrets/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)       23 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2121 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2019 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5844 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2429 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/template.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.136582 batou-2.3b5/src/batou/tests/
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/__init__.py
--rw-r--r--   0 ctheune    (501) staff       (20)      666 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/conftest.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3012 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.117184 batou-2.3b5/src/batou/tests/fixture/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.136729 batou-2.3b5/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.115486 batou-2.3b5/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.136877 batou-2.3b5/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      178 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137019 batou-2.3b5/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.115683 batou-2.3b5/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137190 batou-2.3b5/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       79 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137343 batou-2.3b5/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 ctheune    (501) staff       (20)      128 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137495 batou-2.3b5/src/batou/tests/fixture/component/
--rw-r--r--   0 ctheune    (501) staff       (20)       40 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137638 batou-2.3b5/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.115956 batou-2.3b5/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137793 batou-2.3b5/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 ctheune    (501) staff       (20)      973 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.116725 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.137955 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      144 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138148 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 ctheune    (501) staff       (20)       88 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138302 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 ctheune    (501) staff       (20)      110 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138477 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138633 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 ctheune    (501) staff       (20)       90 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138770 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)      191 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.138915 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 ctheune    (501) staff       (20)       94 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139071 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 ctheune    (501) staff       (20)       85 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139230 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 ctheune    (501) staff       (20)       64 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139389 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 ctheune    (501) staff       (20)       26 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139530 batou-2.3b5/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.116993 batou-2.3b5/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139649 batou-2.3b5/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 ctheune    (501) staff       (20)      346 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139769 batou-2.3b5/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 ctheune    (501) staff       (20)      116 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.117114 batou-2.3b5/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.139898 batou-2.3b5/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 ctheune    (501) staff       (20)       62 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.140167 batou-2.3b5/src/batou/tests/fixture/template/
--rw-r--r--   0 ctheune    (501) staff       (20)       84 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 ctheune    (501) staff       (20)      119 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 ctheune    (501) staff       (20)    18479 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_component.py
--rw-r--r--   0 ctheune    (501) staff       (20)     4771 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_config.py
--rw-r--r--   0 ctheune    (501) staff       (20)     5707 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_dependencies.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1725 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_deploy.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9419 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_endtoend.py
--rw-r--r--   0 ctheune    (501) staff       (20)     8674 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_environment.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2305 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_exceptions.py
--rw-r--r--   0 ctheune    (501) staff       (20)      606 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_host.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1488 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_main.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1326 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_remote.py
--rw-r--r--   0 ctheune    (501) staff       (20)     9398 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_remote_core.py
--rw-r--r--   0 ctheune    (501) staff       (20)     3648 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_repository.py
--rw-r--r--   0 ctheune    (501) staff       (20)      743 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_resources.py
--rw-r--r--   0 ctheune    (501) staff       (20)     2602 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_template.py
--rw-r--r--   0 ctheune    (501) staff       (20)    13871 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)     1169 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/tests/test_vfs.py
--rw-r--r--   0 ctheune    (501) staff       (20)    16103 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/utils.py
--rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/version.txt
--rw-r--r--   0 ctheune    (501) staff       (20)     1009 2022-09-21 10:01:14.000000 batou-2.3b5/src/batou/vfs.py
-drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-09-21 10:01:16.126480 batou-2.3b5/src/batou.egg-info/
--rw-r--r--   0 ctheune    (501) staff       (20)     3465 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 ctheune    (501) staff       (20)     6667 2022-09-21 10:01:16.000000 batou-2.3b5/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 ctheune    (501) staff       (20)      462 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/requires.txt
--rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-09-21 10:01:15.000000 batou-2.3b5/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931588 batou-2.3b6/
+-rw-r--r--   0 ctheune    (501) staff       (20)    31241 2022-12-09 13:30:48.000000 batou-2.3b6/CHANGES.history.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     1608 2022-12-09 13:30:48.000000 batou-2.3b6/LICENSE.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)      212 2022-12-09 13:30:48.000000 batou-2.3b6/MANIFEST.in
+-rw-r--r--   0 ctheune    (501) staff       (20)     3445 2022-12-09 13:30:50.931687 batou-2.3b6/PKG-INFO
+-rw-r--r--   0 ctheune    (501) staff       (20)     2636 2022-12-09 13:30:48.000000 batou-2.3b6/README.md
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.897450 batou-2.3b6/doc/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.904614 batou-2.3b6/doc/source/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.905190 batou-2.3b6/doc/source/api/
+-rw-r--r--   0 ctheune    (501) staff       (20)      886 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/component.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     1717 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/environment.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)       48 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/templates.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)       63 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/api/utilities.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.905331 batou-2.3b6/doc/source/cli/
+-rw-r--r--   0 ctheune    (501) staff       (20)     3742 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/cli/index.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.906097 batou-2.3b6/doc/source/components/
+-rw-r--r--   0 ctheune    (501) staff       (20)     1025 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/cmmi.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     2941 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     5657 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/files.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     4820 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/python.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     3050 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/components/services.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.906684 batou-2.3b6/doc/source/dev/
+-rw-r--r--   0 ctheune    (501) staff       (20)      718 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/authors.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     8555 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/contributing.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     1711 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/testing.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     2809 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/dev/todo.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     8196 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/index.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     4799 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/upgrading.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.907554 batou-2.3b6/doc/source/user/
+-rw-r--r--   0 ctheune    (501) staff       (20)    10868 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/advanced.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     2565 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/install.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     3848 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/installation-deb.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     3798 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     2907 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/intro.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)    47402 2022-12-09 13:30:48.000000 batou-2.3b6/doc/source/user/quickstart.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899351 batou-2.3b6/examples/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.907871 batou-2.3b6/examples/api/
+-rw-r--r--   0 ctheune    (501) staff       (20)      349 2022-12-09 13:30:48.000000 batou-2.3b6/examples/api/index.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/api/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908018 batou-2.3b6/examples/django/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/django/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908159 batou-2.3b6/examples/errors/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/errors/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908308 batou-2.3b6/examples/errors2/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/errors2/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908458 batou-2.3b6/examples/ignores/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/ignores/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908605 batou-2.3b6/examples/largetempl/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/largetempl/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908749 batou-2.3b6/examples/package/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/package/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.908889 batou-2.3b6/examples/sync_async/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/sync_async/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909031 batou-2.3b6/examples/tutorial-buildout/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909179 batou-2.3b6/examples/tutorial-component/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909320 batou-2.3b6/examples/tutorial-helloworld/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909473 batou-2.3b6/examples/tutorial-parallelize/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909621 batou-2.3b6/examples/tutorial-provision-container/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909773 batou-2.3b6/examples/tutorial-secrets/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.909919 batou-2.3b6/examples/vagrant/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/vagrant/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910065 batou-2.3b6/examples/vagrant-multi/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910209 batou-2.3b6/examples/venvs/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.910354 batou-2.3b6/examples/venvs/environments/
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)       54 2022-12-09 13:30:48.000000 batou-2.3b6/examples/venvs/requirements.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)      129 2022-12-09 13:30:48.000000 batou-2.3b6/pyproject.toml
+-rw-r--r--   0 ctheune    (501) staff       (20)      275 2022-12-09 13:30:48.000000 batou-2.3b6/requirements-dev.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)      139 2022-12-09 13:30:50.932007 batou-2.3b6/setup.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)     2408 2022-12-09 13:30:48.000000 batou-2.3b6/setup.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899658 batou-2.3b6/src/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.913247 batou-2.3b6/src/batou/
+-rw-r--r--   0 ctheune    (501) staff       (20)    19689 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      997 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/_output.py
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/agent.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      163 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/c.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    40142 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/component.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      503 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/conftest.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    14278 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/deploy.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    19471 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/environment.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1507 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/fixtures.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    11006 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/host.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914396 batou-2.3b6/src/batou/init-template/
+-rw-r--r--   0 ctheune    (501) staff       (20)       44 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/.hgignore
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.899884 batou-2.3b6/src/batou/init-template/components/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914545 batou-2.3b6/src/batou/init-template/components/example/
+-rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914692 batou-2.3b6/src/batou/init-template/environments/
+-rw-r--r--   0 ctheune    (501) staff       (20)       66 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)      411 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/insecure-private.key
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.917533 batou-2.3b6/src/batou/lib/
+-rw-r--r--   0 ctheune    (501) staff       (20)       29 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3983 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/appenv.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     6457 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/archive.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3297 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/buildout.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2211 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/cmmi.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2524 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/cron.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1224 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/debian.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2286 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/download.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    22046 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/file.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     5811 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/git.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      854 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/goceptnet.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1388 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/logrotate.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     4541 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/mercurial.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3647 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/mysql.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2814 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/nagios.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/package.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     8150 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/python.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.918671 batou-2.3b6/src/batou/lib/resources/
+-rw-r--r--   0 ctheune    (501) staff       (20)     2120 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 ctheune    (501) staff       (20)      244 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/crontab
+-rw-r--r--   0 ctheune    (501) staff       (20)      548 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/init.sh
+-rw-r--r--   0 ctheune    (501) staff       (20)      299 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 ctheune    (501) staff       (20)      840 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)      153 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)      380 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)      609 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 ctheune    (501) staff       (20)      932 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/service.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    10273 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/supervisor.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1172 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/svn.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921053 batou-2.3b6/src/batou/lib/tests/
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3083 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3858 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2318 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3261 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2110 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      639 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2158 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    31505 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     9642 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     6165 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      121 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      847 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1163 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1693 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3106 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     6237 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/main.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921192 batou-2.3b6/src/batou/migrate/
+-rw-r--r--   0 ctheune    (501) staff       (20)     3377 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/__init__.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.921901 batou-2.3b6/src/batou/migrate/migrations/
+-rw-r--r--   0 ctheune    (501) staff       (20)      389 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1775 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      874 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      790 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.922152 batou-2.3b6/src/batou/migrate/tests/
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     4532 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    12756 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/provision.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    11721 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/remote_core.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    11793 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/repository.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     6403 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/resources.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.922722 batou-2.3b6/src/batou/secrets/
+-rw-r--r--   0 ctheune    (501) staff       (20)     3295 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3920 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/edit.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     8524 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/encryption.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     4353 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/manage.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.923312 batou-2.3b6/src/batou/secrets/tests/
+-rw-r--r--   0 ctheune    (501) staff       (20)       23 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3136 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2019 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     5844 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2429 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/template.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926616 batou-2.3b6/src/batou/tests/
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/__init__.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      666 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/conftest.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3012 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.903141 batou-2.3b6/src/batou/tests/fixture/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926785 batou-2.3b6/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901095 batou-2.3b6/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.926956 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 ctheune    (501) staff       (20)      178 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927152 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901327 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927333 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 ctheune    (501) staff       (20)       79 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927514 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 ctheune    (501) staff       (20)      128 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927672 batou-2.3b6/src/batou/tests/fixture/component/
+-rw-r--r--   0 ctheune    (501) staff       (20)       40 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.927834 batou-2.3b6/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.901649 batou-2.3b6/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928017 batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 ctheune    (501) staff       (20)      973 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.902583 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928214 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 ctheune    (501) staff       (20)      144 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928528 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 ctheune    (501) staff       (20)       88 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.928787 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 ctheune    (501) staff       (20)      110 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929019 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 ctheune    (501) staff       (20)       72 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929240 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 ctheune    (501) staff       (20)       90 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929459 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 ctheune    (501) staff       (20)      191 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929678 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 ctheune    (501) staff       (20)       94 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.929900 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 ctheune    (501) staff       (20)       85 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930092 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 ctheune    (501) staff       (20)       64 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930285 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 ctheune    (501) staff       (20)       26 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930481 batou-2.3b6/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 ctheune    (501) staff       (20)       33 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.902910 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930669 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 ctheune    (501) staff       (20)      346 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.930854 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 ctheune    (501) staff       (20)      116 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.903056 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931040 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 ctheune    (501) staff       (20)       62 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.931415 batou-2.3b6/src/batou/tests/fixture/template/
+-rw-r--r--   0 ctheune    (501) staff       (20)       84 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 ctheune    (501) staff       (20)      119 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    18479 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_component.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     4771 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_config.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     5707 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1725 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_deploy.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     9419 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     8674 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_environment.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2305 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      606 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_host.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1488 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_main.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1326 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_remote.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     9398 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     3648 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_repository.py
+-rw-r--r--   0 ctheune    (501) staff       (20)      743 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_resources.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     2602 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_template.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    13871 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_utils.py
+-rw-r--r--   0 ctheune    (501) staff       (20)     1169 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/tests/test_vfs.py
+-rw-r--r--   0 ctheune    (501) staff       (20)    16103 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/utils.py
+-rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/version.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)     1009 2022-12-09 13:30:48.000000 batou-2.3b6/src/batou/vfs.py
+drwxr-xr-x   0 ctheune    (501) staff       (20)        0 2022-12-09 13:30:50.914246 batou-2.3b6/src/batou.egg-info/
+-rw-r--r--   0 ctheune    (501) staff       (20)     3445 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 ctheune    (501) staff       (20)     6667 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)      361 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)        1 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 ctheune    (501) staff       (20)      177 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/requires.txt
+-rw-r--r--   0 ctheune    (501) staff       (20)        6 2022-12-09 13:30:50.000000 batou-2.3b6/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.3b5/CHANGES.history.txt` & `batou-2.3b6/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/LICENSE.txt` & `batou-2.3b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/PKG-INFO` & `batou-2.3b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.3b5
+Version: 2.3b6
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -105,9 +104,7 @@
 * Run `./develop.sh` to create a local virtualenv with everything set up.
 * Run the test suite using: `bin/tox`
 * Build the documentation using: `cd doc; make`
 * Set up GPG for the examples with `export GNUPGHOME=<DIRECTORY OF BATOU HERE>/src/batou/secrets/tests/fixture/gnupg`
 ## Changelog
 
 See [CHANGES.md](./CHANGES.md).
-
-
```

### Comparing `batou-2.3b5/README.md` & `batou-2.3b6/README.md`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/api/component.txt` & `batou-2.3b6/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/api/environment.txt` & `batou-2.3b6/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/cli/index.txt` & `batou-2.3b6/doc/source/cli/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/components/cmmi.txt` & `batou-2.3b6/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/components/downloads-vcs.txt` & `batou-2.3b6/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/components/files.txt` & `batou-2.3b6/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/components/python.txt` & `batou-2.3b6/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/components/services.txt` & `batou-2.3b6/doc/source/components/services.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             self += File('tick.sh', mode="rwxr-xr-x")
 
             self += Service('tick.sh',
                 systemd=dict(Type='simple',
                              Unit_After='cron.service memcached.service',
                              Service_RestartSec=11))
 
+You should import the `batou_ext.nix` module to register the Platform specific `Service` component.
+
 This will result in the following unit file:
 
 .. code-block:: ini
   :caption: /etc/local/systemd/tick.service
 
     [Service]
     Environment="LOCALE_ARCHIVE=/run/current-system/sw/lib/locale/locale-archive"
@@ -52,14 +54,15 @@
     Group=service
     LimitNOFILE=64000
     LimitNPROC=64173
     LimitSIGPENDING=64173
     RestartSec=11
     Type=simple
     User=ctheune
+    Restart=always
 
     [Unit]
     After=cron.service memcached.service
 
 If you want to leverage SystemD's ability to repeat a
 key in the configuration (like using multiple ExecStart statements) then you can simply pass that key as a list. This will be automatically expanded into multiple lines:
```

### Comparing `batou-2.3b5/doc/source/dev/authors.txt` & `batou-2.3b6/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/dev/contributing.txt` & `batou-2.3b6/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/dev/testing.txt` & `batou-2.3b6/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/dev/todo.txt` & `batou-2.3b6/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/index.txt` & `batou-2.3b6/doc/source/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/upgrading.txt` & `batou-2.3b6/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/advanced.txt` & `batou-2.3b6/doc/source/user/advanced.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/install.txt` & `batou-2.3b6/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/installation-deb.txt` & `batou-2.3b6/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/installation-rpm.txt` & `batou-2.3b6/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/intro.txt` & `batou-2.3b6/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/doc/source/user/quickstart.txt` & `batou-2.3b6/doc/source/user/quickstart.txt`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/setup.py` & `batou-2.3b6/setup.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/__init__.py` & `batou-2.3b6/src/batou/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/_output.py` & `batou-2.3b6/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/component.py` & `batou-2.3b6/src/batou/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/deploy.py` & `batou-2.3b6/src/batou/deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/environment.py` & `batou-2.3b6/src/batou/environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/fixtures.py` & `batou-2.3b6/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/host.py` & `batou-2.3b6/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/appenv.py` & `batou-2.3b6/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/archive.py` & `batou-2.3b6/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/buildout.py` & `batou-2.3b6/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/cmmi.py` & `batou-2.3b6/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/cron.py` & `batou-2.3b6/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/debian.py` & `batou-2.3b6/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/download.py` & `batou-2.3b6/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/file.py` & `batou-2.3b6/src/batou/lib/file.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/git.py` & `batou-2.3b6/src/batou/lib/git.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/goceptnet.py` & `batou-2.3b6/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/logrotate.py` & `batou-2.3b6/src/batou/lib/logrotate.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/mercurial.py` & `batou-2.3b6/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/mysql.py` & `batou-2.3b6/src/batou/lib/mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 import tempfile
 
 from batou import UpdateNeeded
 from batou.component import Component
 
+# Pass `USE_SUDO` as `admin_password` to use sudo for authorisation, like we
+# have on FC platform.
+USE_SUDO = object()
+
 
 class Command(Component):
 
     namevar = "statement"
     admin_password = ""
     admin_user = "root"
     hostname = None
@@ -24,18 +28,25 @@
         self.unless = self.expand(self.unless)
 
     def _mysql(self, cmd):
         _, self.tmp = tempfile.mkstemp(suffix="sql")
         with open(self.tmp, "w") as f:
             f.write(cmd + "\n")
 
-        command = [
-            "mysql -Bs -u{{component.admin_user}}",
-            "-p{{component.admin_password}}",
-        ]
+        command = []
+
+        if self.admin_password is USE_SUDO:
+            command.append("sudo -u mysql")
+
+        command.append("mysql -Bs")
+
+        if self.admin_password is not USE_SUDO:
+            command.append("-u{{component.admin_user}}")
+            command.append("-p{{component.admin_password}}")
+
         if self.hostname:
             command.append("-h {{component.hostname}}")
         if self.port:
             command.append("-P {{component.port}}")
         command.append("{{component.db}} < {{component.tmp}}")
 
         out, err = self.cmd(self.expand(" ".join(command)))
```

### Comparing `batou-2.3b5/src/batou/lib/nagios.py` & `batou-2.3b6/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/package.py` & `batou-2.3b6/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/python.py` & `batou-2.3b6/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.3b6/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/resources/init.sh` & `batou-2.3b6/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/resources/nagios.cfg` & `batou-2.3b6/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/resources/supervisor.conf` & `batou-2.3b6/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/service.py` & `batou-2.3b6/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/supervisor.py` & `batou-2.3b6/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/svn.py` & `batou-2.3b6/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_appenv.py` & `batou-2.3b6/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_archive.py` & `batou-2.3b6/src/batou/lib/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_buildout.py` & `batou-2.3b6/src/batou/lib/tests/test_buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_cmmi.py` & `batou-2.3b6/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_cron.py` & `batou-2.3b6/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_debian.py` & `batou-2.3b6/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_download.py` & `batou-2.3b6/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_file.py` & `batou-2.3b6/src/batou/lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_git.py` & `batou-2.3b6/src/batou/lib/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_mercurial.py` & `batou-2.3b6/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_nagios.py` & `batou-2.3b6/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_python.py` & `batou-2.3b6/src/batou/lib/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_service.py` & `batou-2.3b6/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_supervisor.py` & `batou-2.3b6/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/lib/tests/test_svn.py` & `batou-2.3b6/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/main.py` & `batou-2.3b6/src/batou/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import pkg_resources
 
 import batou
 import batou.deploy
 import batou.migrate
 import batou.secrets.edit
+import batou.secrets.encryption
 import batou.secrets.manage
 from batou._output import TerminalBackend, output
 
 
 def main(args: Optional[list] = None) -> None:
     os.chdir(os.environ["APPENV_BASEDIR"])
     version = pkg_resources.resource_string(__name__, "version.txt")
@@ -185,14 +186,15 @@
     )
     migrate.set_defaults(func=batou.migrate.main)
 
     args = parser.parse_args(args)
 
     # Consume global arguments
     batou.output.enable_debug = args.debug
+    batou.secrets.encryption.debug = args.debug
 
     # Pass over to function
     if args.func.__name__ == "print_usage":
         args.func()
         sys.exit(1)
 
     if args.func != batou.migrate.main:
```

### Comparing `batou-2.3b5/src/batou/migrate/__init__.py` & `batou-2.3b6/src/batou/migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/migrate/migrations/2301.py` & `batou-2.3b6/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/migrate/migrations/2302.py` & `batou-2.3b6/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/migrate/migrations/2303.py` & `batou-2.3b6/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/migrate/tests/test_migrate.py` & `batou-2.3b6/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/provision.py` & `batou-2.3b6/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/remote_core.py` & `batou-2.3b6/src/batou/remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/repository.py` & `batou-2.3b6/src/batou/repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/resources.py` & `batou-2.3b6/src/batou/resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/secrets/__init__.py` & `batou-2.3b6/src/batou/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/secrets/edit.py` & `batou-2.3b6/src/batou/secrets/edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.environment = environment
         environment_path = pathlib.Path("environments") / environment
         self.encrypted_configfile = environment_path / "secrets.cfg"
 
         if edit_file is None:
             self.edit_file = self.encrypted_configfile
         else:
-            self.edit_file = environment_path / edit_file
+            self.edit_file = environment_path / f"secret-{edit_file}"
 
     def main(self):
         with EncryptedConfigFile(
             self.encrypted_configfile,
             add_files_for_env=self.environment,
             write_lock=True,
         ) as configfile:
@@ -64,15 +64,18 @@
             self.encrypt()
         elif cmd == "encrypt":
             self.encrypt()
         else:
             raise ValueError("unknown command `{}`".format(cmd))
 
     def encrypt(self):
-        if self.cleartext == self.original_cleartext:
+        if (
+            self.cleartext == self.original_cleartext
+            and not self.editing.is_new
+        ):
             print("No changes from original cleartext. Not updating.")
             return
         self.editing.cleartext = self.cleartext
         # In case we are editing the main file, this causes a re-read
         # of the membership and re-serialization, so we are sure the file
         # is syntactically correct.
         self.configfile.read()
```

### Comparing `batou-2.3b5/src/batou/secrets/encryption.py` & `batou-2.3b6/src/batou/secrets/encryption.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import tempfile
 from typing import Generator, Optional
 
 from configupdater import ConfigUpdater
 
 from batou import FileLockedError, GPGCallError
 
+debug = False
+
 # https://thraxil.org/users/anders/posts/2008/03/13/Subprocess-Hanging-PIPE-is-your-enemy/
 NULL = tempfile.TemporaryFile()
 
 NEW_FILE_TEMPLATE = """\
 [batou]
 members =
 """
@@ -31,26 +33,38 @@
 
 class EncryptedFile(object):
     """Basic encryption methods - key management handled externally."""
 
     lockfd = None
     cleartext = None
 
+    is_new = None
+
     GPG_BINARY_CANDIDATES = ["gpg", "gpg2"]
 
     def __init__(self, encrypted_filename, write_lock=False, quiet=False):
         """Context manager that opens an encrypted file.
 
         Use the read() and write() methods in the subordinate "with"
         block to manipulate cleartext content. If the cleartext content
         has been replaced, the encrypted file is updated.
 
         `write_lock` must be set True if a modification of the file is
         intended.
         """
+        if debug:
+            print(
+                f"""\
+EncryptedFile.__init__(
+    self,
+    encrypted_filename={encrypted_filename},
+    write_lock={write_lock},
+    quiet={quiet},
+)"""
+            )
         # Ensure compatibility with pathlib.
         self.encrypted_filename = str(encrypted_filename)
         self.write_lock = write_lock
         self.quiet = quiet
         self.recipients = []
 
     def __enter__(self):
@@ -60,14 +74,16 @@
     def __exit__(self, _exc_type=None, _exc_value=None, _traceback=None):
         self.lockfd.close()
 
     def gpg(self):
         with tempfile.TemporaryFile() as null:
             for gpg in self.GPG_BINARY_CANDIDATES:
                 try:
+                    if debug:
+                        print(f'Trying "{gpg} --version"')
                     subprocess.check_call(
                         [gpg, "--version"], stdout=null, stderr=null
                     )
                 except (subprocess.CalledProcessError, OSError):
                     pass
                 else:
                     return gpg
@@ -87,17 +103,23 @@
                 self.cleartext = ""
         return self.cleartext
 
     def write(self):
         """Encrypt cleartext and write into destination file file. ."""
         if not self.write_lock:
             raise RuntimeError("write() needs a write lock")
+        self.is_new = False
         self._encrypt(self.cleartext)
 
     def _lock(self):
+        if debug:
+            print(f"Locking {self.encrypted_filename}")
+        # if the file doesn't exist, we set is_new
+        if self.is_new is None:
+            self.is_new = not os.path.exists(self.encrypted_filename)
         self.lockfd = open(
             self.encrypted_filename, "a+" if self.write_lock else "r+"
         )
         try:
             fcntl.lockf(
                 self.lockfd,
                 fcntl.LOCK_EX
@@ -109,14 +131,16 @@
 
     def _decrypt(self):
         args = [self.gpg()]
         if self.quiet:
             args += ["-q", "--no-tty", "--batch"]
         args += ["--decrypt", self.encrypted_filename]
         try:
+            if debug:
+                print(f"Decrypting with: {args}")
             result = subprocess.run(
                 args, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
         except subprocess.CalledProcessError as e:
             raise GPGCallError.from_context(args, e.returncode, e.stderr) from e
         else:
             return result.stdout.decode("utf-8")
@@ -128,14 +152,16 @@
             )
         os.rename(self.encrypted_filename, self.encrypted_filename + ".old")
         args = [self.gpg(), "--encrypt"]
         for r in self.recipients:
             args.extend(["-r", r.strip()])
         args.extend(["-o", self.encrypted_filename])
         try:
+            if debug:
+                print(f"Encrypting with: {args}")
             gpg = subprocess.Popen(args, stdin=subprocess.PIPE)
             gpg.communicate(data.encode("utf-8"))
             if gpg.returncode != 0:
                 raise RuntimeError("GPG returned non-zero exit code.")
         except Exception:
             os.rename(self.encrypted_filename + ".old", self.encrypted_filename)
             raise
@@ -154,27 +180,39 @@
     def __init__(
         self,
         encrypted_file,
         add_files_for_env: Optional[str] = None,
         write_lock=False,
         quiet=False,
     ):
+        if debug:
+            print(
+                f"""\
+EncryptedConfigFile.__init__(
+    self,
+    encrypted_file={encrypted_file},
+    add_files_for_env={add_files_for_env},
+    write_lock={write_lock},
+    quiet={quiet})"""
+            )
         self.add_files_for_env = add_files_for_env
         self.write_lock = write_lock
         self.quiet = quiet
         self.files = {}
 
         self.main_file = self.add_file(encrypted_file)
 
         # Add all existing files to the session
         if self.add_files_for_env:
             for path in iter_other_secrets(self.add_files_for_env):
                 self.add_file(path)
 
     def add_file(self, filename):
+        if debug:
+            print(f"add_file: {filename}")
         # Ensure compatibility with pathlib.
         filename = str(filename)
         if filename not in self.files:
             self.files[filename] = f = EncryptedFile(
                 filename, self.write_lock, self.quiet
             )
             f.read()
@@ -216,14 +254,16 @@
             return []
         members = [x.strip() for x in members]
         members = [_f for _f in members if _f]
         members.sort()
         return members
 
     def set_members(self, members):
+        if debug:
+            print(f"set_members: {members}")
         # The whitespace here is exactly what
         # "members = " looks like in the config file so we get
         # proper indentation.
         members = ",\n".join(members)
         # Work around multi-line handling in configupdater
         members = members.split("\n")
         self.config.set("batou", "members", members)
```

### Comparing `batou-2.3b5/src/batou/secrets/manage.py` & `batou-2.3b6/src/batou/secrets/manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/secrets/tests/test_editor.py` & `batou-2.3b6/src/batou/secrets/tests/test_editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import pathlib
+
 import pytest
 
 from batou.secrets.edit import Editor
 from batou.secrets.encryption import EncryptedConfigFile
 
+from .test_secrets import encrypted_file
+
 
 def test_edit(tmpdir):
     with EncryptedConfigFile(str(tmpdir / "asdf"), write_lock=True) as sf:
         editor = Editor(
             "true", environment="none", edit_file=list(sf.files.keys())[0]
         )
         editor.cleartext = "asdf"
@@ -73,7 +77,33 @@
 
 Your changes are still available. You can try:
 \tedit       -- opens editor with current data again
 \tencrypt    -- tries to encrypt current data again
 \tquit       -- quits and loses your changes
 """
     )
+
+
+def test_edit_file_has_secret_prefix(tmpdir, encrypted_file):
+    filename = "asdf123"
+    c = EncryptedConfigFile(encrypted_file, write_lock=True)
+    with c as _:
+        editor = Editor("true", environment="none", edit_file=filename)
+        assert editor.edit_file == pathlib.Path("environments") / "none" / (
+            f"secret-{filename}"
+        )
+
+
+def test_blank_edit(tmpdir, encrypted_file):
+    c = EncryptedConfigFile(encrypted_file, write_lock=True)
+    with c as configfile:
+        editor = Editor("true", environment="none", edit_file="asdf")
+        editor.configfile = configfile
+        editor.editing = configfile.add_file(tmpdir / "asdf")
+        with editor.editing as f:
+            f.read()
+            editor.cleartext = editor.original_cleartext = f.cleartext
+        editor.edit()
+        assert editor.cleartext == ""
+        editor.encrypt()
+        with open(tmpdir / "asdf", "rb") as f:
+            assert f.read() != b""
```

### Comparing `batou-2.3b5/src/batou/secrets/tests/test_manage.py` & `batou-2.3b6/src/batou/secrets/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/secrets/tests/test_secrets.py` & `batou-2.3b6/src/batou/secrets/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/template.py` & `batou-2.3b6/src/batou/template.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/conftest.py` & `batou-2.3b6/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/ellipsis.py` & `batou-2.3b6/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.3b6/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_component.py` & `batou-2.3b6/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_config.py` & `batou-2.3b6/src/batou/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_dependencies.py` & `batou-2.3b6/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_deploy.py` & `batou-2.3b6/src/batou/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_endtoend.py` & `batou-2.3b6/src/batou/tests/test_endtoend.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_environment.py` & `batou-2.3b6/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_exceptions.py` & `batou-2.3b6/src/batou/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_host.py` & `batou-2.3b6/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_main.py` & `batou-2.3b6/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_remote.py` & `batou-2.3b6/src/batou/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_remote_core.py` & `batou-2.3b6/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_repository.py` & `batou-2.3b6/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_resources.py` & `batou-2.3b6/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_template.py` & `batou-2.3b6/src/batou/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_utils.py` & `batou-2.3b6/src/batou/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/tests/test_vfs.py` & `batou-2.3b6/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/utils.py` & `batou-2.3b6/src/batou/utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou/vfs.py` & `batou-2.3b6/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.3b5/src/batou.egg-info/PKG-INFO` & `batou-2.3b6/src/batou.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.3b5
+Version: 2.3b6
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -105,9 +104,7 @@
 * Run `./develop.sh` to create a local virtualenv with everything set up.
 * Run the test suite using: `bin/tox`
 * Build the documentation using: `cd doc; make`
 * Set up GPG for the examples with `export GNUPGHOME=<DIRECTORY OF BATOU HERE>/src/batou/secrets/tests/fixture/gnupg`
 ## Changelog
 
 See [CHANGES.md](./CHANGES.md).
-
-
```

### Comparing `batou-2.3b5/src/batou.egg-info/SOURCES.txt` & `batou-2.3b6/src/batou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

