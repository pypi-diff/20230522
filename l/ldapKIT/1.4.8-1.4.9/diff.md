# Comparing `tmp/ldapKIT-1.4.8.tar.gz` & `tmp/ldapKIT-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldapKIT-1.4.8.tar", last modified: Fri Dec 17 10:28:18 2021, max compression
+gzip compressed data, was "ldapKIT-1.4.9.tar", last modified: Thu Aug 18 13:40:18 2022, max compression
```

## Comparing `ldapKIT-1.4.8.tar` & `ldapKIT-1.4.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0       35 2021-11-02 14:52:15.581921 ldapKIT-1.4.8/.gitignore
--rw-r--r--   0        0        0    32422 2021-11-02 14:52:15.585921 ldapKIT-1.4.8/LICENSE
--rw-r--r--   0        0        0     2487 2021-11-02 14:52:15.585921 ldapKIT-1.4.8/README.md
--rw-r--r--   0        0        0     2412 2021-11-02 14:52:15.589921 ldapKIT-1.4.8/example/config.yml
--rw-r--r--   0        0        0     3520 2021-11-02 14:52:15.593921 ldapKIT-1.4.8/example/userdir.yml
--rw-r--r--   0        0        0      153 2021-12-17 10:27:39.553572 ldapKIT-1.4.8/ldapKIT/__init__.py
--rw-r--r--   0        0        0      684 2021-11-02 14:52:15.597921 ldapKIT-1.4.8/ldapKIT/config.py
--rw-r--r--   0        0        0    21362 2021-12-17 10:25:13.093747 ldapKIT-1.4.8/ldapKIT/ldapKIT.py
--rw-r--r--   0        0        0     4788 2021-11-02 14:52:15.601921 ldapKIT-1.4.8/ldapKIT/particleldapchangemail.py
--rw-r--r--   0        0        0     2392 2021-11-02 14:52:15.605921 ldapKIT-1.4.8/ldapKIT/particleldapgroup.py
--rw-r--r--   0        0        0     1092 2021-11-02 15:28:04.037068 ldapKIT-1.4.8/ldapKIT/particleldapresetpassword.py
--rw-r--r--   0        0        0    10106 2021-12-17 10:25:54.565697 ldapKIT-1.4.8/ldapKIT/particleldapuseradd.py
--rw-r--r--   0        0        0     7322 2021-11-02 14:52:15.613921 ldapKIT-1.4.8/ldapKIT/particleldapuserdel.py
--rw-r--r--   0        0        0      790 2021-11-02 14:52:15.613921 ldapKIT-1.4.8/pyproject.toml
--rw-r--r--   0        0        0       48 2021-11-02 14:52:15.613921 ldapKIT-1.4.8/requirements.txt
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 ldapKIT-1.4.8/setup.py
--rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 ldapKIT-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0       35 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/.gitignore
+-rw-r--r--   0        0        0    32422 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/LICENSE
+-rw-r--r--   0        0        0     2487 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/README.md
+-rw-r--r--   0        0        0     2412 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/example/config.yml
+-rw-r--r--   0        0        0     3520 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/example/userdir.yml
+-rw-r--r--   0        0        0      153 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/ldapKIT/__init__.py
+-rw-r--r--   0        0        0      684 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/ldapKIT/config.py
+-rw-r--r--   0        0        0    21362 2022-08-18 13:39:59.202893 ldapKIT-1.4.9/ldapKIT/ldapKIT.py
+-rw-r--r--   0        0        0     4788 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/ldapKIT/particleldapchangemail.py
+-rw-r--r--   0        0        0     2392 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/ldapKIT/particleldapgroup.py
+-rw-r--r--   0        0        0     1092 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/ldapKIT/particleldapresetpassword.py
+-rw-r--r--   0        0        0    10111 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/ldapKIT/particleldapuseradd.py
+-rw-r--r--   0        0        0     7322 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/ldapKIT/particleldapuserdel.py
+-rw-r--r--   0        0        0      790 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0       48 2022-08-18 13:39:59.206893 ldapKIT-1.4.9/requirements.txt
+-rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 ldapKIT-1.4.9/PKG-INFO
```

### Comparing `ldapKIT-1.4.8/LICENSE` & `ldapKIT-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/README.md` & `ldapKIT-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/example/config.yml` & `ldapKIT-1.4.9/example/config.yml`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/example/userdir.yml` & `ldapKIT-1.4.9/example/userdir.yml`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/config.py` & `ldapKIT-1.4.9/ldapKIT/config.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/ldapKIT.py` & `ldapKIT-1.4.9/ldapKIT/ldapKIT.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/particleldapchangemail.py` & `ldapKIT-1.4.9/ldapKIT/particleldapchangemail.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/particleldapgroup.py` & `ldapKIT-1.4.9/ldapKIT/particleldapgroup.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/particleldapresetpassword.py` & `ldapKIT-1.4.9/ldapKIT/particleldapresetpassword.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/ldapKIT/particleldapuseradd.py` & `ldapKIT-1.4.9/ldapKIT/particleldapuseradd.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 welcome_mail,
                 ldapcon.config['email_smtp_host']
                 )
 
     if not isinstance(mailinglist, list):
         mailinglist = [mailinglist]
     for ml in mailinglist:
-        if attr['mail'] and ml and ldapKIT.yesno('Adding user %s to email list %s ?' % (attr['uid'], group), default='y'):
+        if attr['mail'] and ml and ldapKIT.yesno('Adding user %s to email list %s ?' % (attr['uid'], ml['list']), default='y'):
             if not args.dryrun:
                 ldapKIT.addtolist(attr['mail'], ml)
             else:
                 print('(dryrun enabled)')
 
     runansible = 'ansible' in ldapcon.config
     if not runansible or \
```

### Comparing `ldapKIT-1.4.8/ldapKIT/particleldapuserdel.py` & `ldapKIT-1.4.9/ldapKIT/particleldapuserdel.py`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/pyproject.toml` & `ldapKIT-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ldapKIT-1.4.8/PKG-INFO` & `ldapKIT-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldapKIT
-Version: 1.4.8
+Version: 1.4.9
 Summary: Collection of useful scripts for ldap based user management.
 Home-page: https://github.com/particleKIT/ldapKIT.git
 Author: Martin Gabelmann, Robin Roth
 Author-email: martin@gabelmann.biz
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: python_gitlab
```

