# Comparing `tmp/mecapacktools-1.0.0.tar.gz` & `tmp/mecapacktools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.0.0.tar", max compression
+gzip compressed data, was "mecapacktools-1.0.1.tar", max compression
```

## Comparing `mecapacktools-1.0.0.tar` & `mecapacktools-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.0/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6315 2023-04-14 08:17:17.748938 mecapacktools-1.0.0/mecapacktools/libCfg.py
--rw-r--r--   0        0        0    13137 2023-04-14 09:17:25.372964 mecapacktools-1.0.0/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19318 2023-04-14 11:33:45.358196 mecapacktools-1.0.0/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8491 2023-04-14 11:44:47.533597 mecapacktools-1.0.0/mecapacktools/libSql.py
--rw-r--r--   0        0        0    14571 2023-04-14 09:01:09.416597 mecapacktools-1.0.0/mecapacktools/libTool.py
--rw-r--r--   0        0        0    18145 2023-04-27 13:02:40.956437 mecapacktools-1.0.0/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1090 2023-04-27 13:19:17.163828 mecapacktools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      634 2023-04-27 13:19:13.091595 mecapacktools-1.0.0/README.md
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 mecapacktools-1.0.0/setup.py
--rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 mecapacktools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.1/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.1/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.1/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.1/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.1/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.1/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20041 2023-05-22 08:10:44.484275 mecapacktools-1.0.1/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1090 2023-05-22 08:46:34.874177 mecapacktools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      668 2023-04-27 13:23:11.491614 mecapacktools-1.0.1/README.md
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 mecapacktools-1.0.1/setup.py
+-rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 mecapacktools-1.0.1/PKG-INFO
```

### Comparing `mecapacktools-1.0.0/LICENSE` & `mecapacktools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.0/mecapacktools/libCfg.py` & `mecapacktools-1.0.1/mecapacktools/libCfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long
 """Configuration system management."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 
 import os.path
 import sys
@@ -40,15 +40,17 @@
     # //////////////////////////////////////////////////
     def __init__(self, pfilePath=None, plogfileexists="WARNING"):
         """
         Initialization of the class
 
         Args:
             pfilePath (_type_, optional): the cfg file path. Defaults to None.
-            plogfileexists (str, optional): Log level display for check exist file. "None" for no display. Defaults to "WARNING".
+            plogfileexists (str, optional): Log level display for check exist file.
+                "None" for no display.
+                Defaults to "WARNING".
         """
 
         # Base initialization
         UserDict.__init__(self)
 
         # Work variables
         self.__CfgParser = ConfigParser()
@@ -83,20 +85,20 @@
 
         Args:
             pfilePath (str): the cfg file path
 
         Raises:
             self.log.CustomException: Error file path
         """
-
+        # pylint: disable=eval-used,broad-exception-caught
         # Reading file
         if os.path.isfile(pfilePath):
             self.__CfgParser.read(pfilePath)
         else:
-            raise self.log.CustomException("cfg file does not exist : %s", pfilePath)
+            raise self.log.CustomException(f"cfg file does not exist : {pfilePath}")
 
         # Reading section
         for sectionTemp in self.__CfgParser.sections():
             # Reading parameters
             for optionTemp in self.__CfgParser.options(sectionTemp):
                 # Adding section in dictionary if does not exist
                 if sectionTemp not in self:
@@ -141,27 +143,27 @@
 
         Args:
             pfilePath (str): the cfg file path
 
         Raises:
             self.log.CustomException: Error file path
         """
-
+        # pylint: disable-next=consider-using-dict-items
         for sectionTemp in self.keys():
             if sectionTemp not in self.__CfgParser.sections():
                 self.__CfgParser.add_section(sectionTemp)
             for optionTemp in self[sectionTemp].keys():
                 self.__CfgParser.set(sectionTemp, optionTemp, self[sectionTemp][optionTemp])
 
         # Reading file
         if os.path.isfile(pfilePath):
-            with open(pfilePath, "w") as f:
+            with open(pfilePath, "w", encoding="utf-8") as f:
                 self.__CfgParser.write(f)
         else:
-            raise self.log.CustomException("cfg file does not exist : %s", pfilePath)
+            raise self.log.CustomException(f"cfg file does not exist : {pfilePath}")
 
     # //////////////////////////////////////////////////
     #     UpdateKeyDict
     # //////////////////////////////////////////////////
     def UpdateKeyDict(self, pdict):
         """
         Update target dict by common group keys
```

### Comparing `mecapacktools-1.0.0/mecapacktools/libLog.py` & `mecapacktools-1.0.1/mecapacktools/libLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long
 """Log system management."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 
 import logging
 import logging.handlers
@@ -239,19 +239,15 @@
         if self.hshParam["relativeProfilDirectory"]:
             headDirectory = os.path.join(os.getenv("HOMEDRIVE"), os.getenv("HOMEPATH"))
 
         # Build the specify log directory if need
         if self.hshParam["oneLogByLaunch"]:
             dirPath_temp = os.path.join(
                 dirPath_temp,
-                "%s_%s"
-                % (
-                    self.hshParam["process"],
-                    time.strftime("%Y%m%d_%H%M%S", self.hshParam["startDateTime"]),
-                ),
+                f"{self.hshParam['process']}_{time.strftime('%Y%m%d_%H%M%S', self.hshParam['startDateTime'])}",
             )
 
         # Get absolute path
         if not os.path.isabs(dirPath_temp):
             dirPath_temp = os.path.abspath(os.path.join(headDirectory, dirPath_temp))
 
         # Creation of the log directory if does not exist
@@ -320,15 +316,15 @@
                     self.__args[i] = arg.message
                 else:
                     self.__args[i] = str(arg)
         if isinstance(self.__msg, Exception):
             if hasattr(self.__msg, "message"):
                 self.__msg = self.__msg.message
             else:
-                self.__msg = self.str(self.__msg)
+                self.__msg = str(self.__msg)
         self.__args = tuple(self.__args)
 
         # Build the logger name hierarchical
         if len(self.hshParam["process"]) == 0:
             # Get the logger root
             loggerMaster = logging.getLogger()
             loggerTemp = loggerMaster
```

### Comparing `mecapacktools-1.0.0/mecapacktools/libMail.py` & `mecapacktools-1.0.1/mecapacktools/libMail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long,dangerous-default-value
 """Mail system management."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 
 import mimetypes
 import os.path
 from collections import UserList
 from email import encoders
+from email.mime.audio import MIMEAudio
+from email.mime.image import MIMEImage
+from email.mime.multipart import MIMEBase, MIMEMultipart
+from email.mime.text import MIMEText
 from smtplib import SMTP, SMTPServerDisconnected
 
 from . import libLog
 
 try:
     # some systems
+    # pylint: disable-next=ungrouped-imports
     from email import charset as Charset
 except ImportError:
     from email import Charset
 
-from email.mime.audio import MIMEAudio
-from email.mime.image import MIMEImage
-from email.mime.multipart import MIMEBase, MIMEMultipart
-from email.mime.text import MIMEText
-
 # ============================================================
 #    Variables and Constants
 # ============================================================
 
 Charset.add_charset("utf-8", Charset.QP, Charset.QP, "utf-8")
 
 
@@ -60,14 +60,20 @@
         self.__val = valTemp
 
     # //////////////////////////////////////////////////
     #     Value
     # //////////////////////////////////////////////////
     @property
     def Value(self):
+        """
+        return Value
+
+        Returns:
+            str: value
+        """
         return self.__val
 
     # //////////////////////////////////////////////////
     #     __add__
     # //////////////////////////////////////////////////
     def __add__(self, pval):
         valTemp = self.__val
@@ -182,21 +188,21 @@
             self.log.CustomException: Some mails were not sent
             self.log.CustomException: All sending mails failed
             self.log.CustomException: No mail to send
         """
 
         self.log.setStep = "SMTP_initialization"
         # Setting work variables
-        if not pserver == "":
+        if pserver != "":
             self.hshParam["server"] = pserver
-        if not pport == 0:
+        if pport != 0:
             self.hshParam["port"] = pport
-        if not puser == "":
+        if puser != "":
             self.hshParam["user"] = puser
-        if not ppassword == "":
+        if ppassword != "":
             self.hshParam["password"] = ppassword
         # Initialization of the SMTP management
         SMTP_management = SMTP(self.hshParam["server"], self.hshParam["port"], timeout=300)
         if self.hshParam["user"]:
             SMTP_management = self.TLS_Connect()
 
         # Log
@@ -220,20 +226,22 @@
                 try:
                     SMTP_management.sendmail(mailSender, mailReceivers, msg_temp.msg.as_string())
                     mailSentOk += 1
                     self.log.Info("Mail sent to %s with success", mailReceivers)
                 except SMTPServerDisconnected:  # Retry to connect one time to mail server in case of timout
                     try:
                         SMTP_management.quit()  # Ensure that previus session was disconected
+                    # pylint: disable-next=broad-exception-caught
                     except Exception:
                         pass  # Deal with alea of deconnexion by office365
                     SMTP_management = self.TLS_Connect()
                     SMTP_management.sendmail(mailSender, mailReceivers, msg_temp.msg.as_string())
                     mailSentOk += 1
                     self.log.Info("Mail sent to %s with success", mailReceivers)
+                # pylint: disable-next=broad-exception-caught
                 except Exception as e:
                     self.log.Warning("Mail not sent to %s : %s", mailReceivers, e, exc_info=1)
                     mailSentKo += 1
             else:
                 self.log.Warning("Mail definition is not valid : %s", Mail, exc_info=1)
                 mailSentKo += 1
         # Assessment
@@ -491,15 +499,15 @@
                 # Determine type and encoding of file
                 ctype, encoding = mimetypes.guess_type(pAttachFile_path)
                 if ctype is None or encoding is not None:
                     ctype = "application/octet-stream"
                 maintype, subtype = ctype.split("/", 1)
                 # Loading file
                 if maintype == "text":
-                    fileTemp = open(pAttachFile_path)
+                    fileTemp = open(pAttachFile_path, encoding="utf-8")
                     msg_attach_temp = MIMEText(fileTemp.read(), _subtype=subtype)
                     fileTemp.close()
                 elif maintype == "image":
                     fileTemp = open(pAttachFile_path, "rb")
                     msg_attach_temp = MIMEImage(fileTemp.read(), _subtype=subtype)
                     fileTemp.close()
                 elif maintype == "audio":
```

### Comparing `mecapacktools-1.0.0/mecapacktools/libSql.py` & `mecapacktools-1.0.1/mecapacktools/libSql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long
 """Sql system management."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 try:
     import pypyodbc as pyodbc
 except ImportError:
+    # pylint: disable-next=broad-exception-raised,raise-missing-from
     raise Exception(
         """Could not load libSql due to import Error
         Are you sure to installed Extras : pip install mecapacktools[Sql] ?"""
     )
 from sortedcontainers import SortedDict
 
 from . import libLog
@@ -47,14 +48,15 @@
             dict: datas
         """
         return self.hshData
 
     # //////////////////////////////////////////////////
     #     INITIALIZATION
     # //////////////////////////////////////////////////
+    # pylint: disable-next=dangerous-default-value
     def __init__(self, phshParam={}):
         # Work variables
         self.connections = {}
         self.cursors = {}
         self._last_count = None
         self._data_flag = False
         self._at_least_one_change = False
@@ -103,35 +105,40 @@
         """
         Execute SQL request
 
         Args:
             pqueryfilter (str): filter string in queries dictionary
             pbind (str, optional): the bind variables of queries. Defaults to None.
             pformat (str, optional): the ? info to replace into queries. Defaults to None.
-            ptransaction (str, optional): Validation of transaction : "commit", "rollback", "standby" and, "None" (default) for select statement. Defaults to None.
+            ptransaction (str, optional): Validation of transaction :
+                "commit", "rollback", "standby" and, "None" (default)
+                for select statement. Defaults to None.
             **pcnxname -- Name of connection (default=value between point in query key)
             **pcursorname -- Name of cursor (default=value between point in query key)
             **pfetchtype -- Type of data fetch ; "fetchall" (default), fetchone
             **plogrequest -- Log level display for request. "None" for no display (default=DEBUG)
-            **plogcolumn -- Log level display for column. "None" for no display (default=DEBUG)
+            **plogcolumn -- Log level display for column. "None" for no display (default=None)
             **plogrow -- Log level display for row. "None" for no display (default=DEBUG)
             **plogcount -- Log level display for count. "None" for no display (default=DEBUG)
-            **perrnochange -- Raise exception if no change with the request. Value expected, message or CustomException code. "None" for no display (default=None)
+            **perrnochange -- Raise exception if no change with the request.
+                Value expected, message or CustomException code.
+                "None" for no display (default=None)
             **perrrequest -- Log level display for request in error. "None" for no display (default=INFO)
 
         Raises:
-            self.log.CustomException: Raise exception if no change with the request. Value expected, message or CustomException code
+            self.log.CustomException: Raise exception if no change with the request.
+                Value expected, message or CustomException code
         """
 
         hshOption = {
             "pcnxname": None,
             "pcursorname": None,
             "pfetchtype": "fetchall",
             "plogrequest": "DEBUG",
-            "plogcolumn": "DEBUG",
+            "plogcolumn": None,
             "plogrow": "DEBUG",
             "plogcount": "DEBUG",
             "perrnochange": None,
             "perrrequest": "INFO",
         }
         _transaction = {
             "commit": "commit",
@@ -148,15 +155,15 @@
         self._data_flag = False
         self._at_least_one_change = False
 
         for k, v in filter(
             lambda x: pqueryfilter == x[0][: len(pqueryfilter)],
             self.hshParam["Queries"].items(),
         ):
-            self.log.setStep = "Q[%s]" % k
+            self.log.setStep = f"Q[{k}]"
             cnxname = hshOption["pcnxname"] or k.split(".")[1]
             cursorname = hshOption["pcursorname"] or k.split(".")[1]
             if pbind:
                 SQL0 = v.format(**pbind)
             else:
                 SQL0 = v
             if hshOption["plogrequest"]:
@@ -196,13 +203,13 @@
                 count0 = len(rows0 or [])
                 if hshOption["plogcount"]:
                     self.log.Write(self.log.LEVEL[hshOption["plogcount"]], "Rowcount : %s", count0)
                 if hshOption["plogcolumn"]:
                     self.log.Write(self.log.LEVEL[hshOption["plogcolumn"]], "Columns : %s", column0)
                 if hshOption["plogrow"]:
                     self.log.Write(self.log.LEVEL[hshOption["plogrow"]], "Rows : %s", rows0)
-                self.hshData["%s.H" % self.hshParam["Dataname"].get(k, k)] = column0
-                self.hshData["%s.R" % self.hshParam["Dataname"].get(k, k)] = rows0
+                self.hshData[f"{self.hshParam['Dataname'].get(k, k)}.H"] = column0
+                self.hshData[f"{self.hshParam['Dataname'].get(k, k)}.R"] = rows0
                 if not count0 == 0:
                     self._data_flag = True
             self._last_count = count0
             self.log.setStep = ""
```

### Comparing `mecapacktools-1.0.0/mecapacktools/libTool.py` & `mecapacktools-1.0.1/mecapacktools/libTool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long
 """Tools python."""
 # ============================================================
 #    Linux python path and Library import
 # ============================================================
 
 import calendar
 import datetime
@@ -120,14 +120,15 @@
     isoWEEK = str(isoWEEK).rjust(2, "0")
     return (isoYEAR, isoWEEK)
 
 
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
 #    convertHeaders_ToList
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
+# pylint: disable-next=dangerous-default-value
 def convertHeaders_ToList(
     pheaders,
     pdecoding=None,
     pencoding=None,
     pdoublequote=False,
     ptobind=False,
     pnone=None,
@@ -366,14 +367,15 @@
         new_list.append(v)
     return new_list
 
 
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
 #    convertDict_ToDict
 # ||||||||||||||||||||||||||||||||||||||||||||||||||
+# pylint: disable-next=dangerous-default-value
 def convertDict_ToDict(
     pdict,
     pdecoding=None,
     pencoding=None,
     pdoublequote=False,
     ptobind=False,
     pnone=None,
@@ -401,14 +403,15 @@
     """
     new_dict = OrderedDict()
     for k, v in pdict.items():
         v = val_convert(
             v,
             pdecoding=pdecoding,
             pdoublequote=pdoublequote,
+            pencoding=pencoding,
             ptobind=ptobind,
             pnone=pnone,
             pcase=pcase,
             pstrip=pstrip,
             pisdttutc=pisdttutc,
         )
         new_dict[pdictconv.get(k, k)] = v
@@ -456,26 +459,28 @@
     if pdoublequote:
         if isinstance(v, str):
             v = v.replace("'", "''")
     if ptobind:
         if v is None:
             v = "NULL"
         elif isinstance(v, str):
-            v = "'%s'" % v
+            v = f"'{v}'"
     if pisdttutc:
         if isinstance(v, datetime.date):
             v = arrow.get(v).datetime
     if pdecoding is not None:
         try:
             v = v.decode(pdecoding)
+        # pylint: disable-next=broad-exception-caught
         except Exception:
             pass
     if pencoding is not None:
         try:
             v = v.encode(pencoding)
+        # pylint: disable-next=broad-exception-caught
         except Exception:
             pass
     if pcase is not None:
         if isinstance(v, str):
             if "UP" in pcase.upper():
                 v = v.upper()
             if "LOW" in pcase.upper():
```

### Comparing `mecapacktools-1.0.0/mecapacktools/libWebServices.py` & `mecapacktools-1.0.1/mecapacktools/libWebServices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 #! /usr/bin/env python
 # -*- coding:Utf-8 -*-
-
+# pylint: disable=fixme,invalid-name,line-too-long
 """ WebServices system management."""
 
+import time
 from datetime import datetime
 
 import requests
 import xmltodict
 from requests.auth import HTTPBasicAuth
 from suds.client import Client
+from urllib3.exceptions import MaxRetryError
 from urllib3.util import SKIP_HEADER
 
 from . import libLog
 
 
 class webServices_WSDL:
     """Class to manage SOAP Webservice (ie: Kelio)"""
 
     hshParam = {}
     __hshData = {}
 
     @property
     def data(self):
+        """
+        return data
+
+        Returns:
+            dict: data
+        """
         return self.__hshData
 
+    # pylint: disable-next=dangerous-default-value
     def __init__(self, phshParam={}):
         # Work variables
         self.token = ""
         self.login = ""
 
         # Start log manager
         self.log = libLog.Log()
@@ -59,53 +68,76 @@
     """Class Webservices Sylob"""
 
     #: Variables
     hshParam = {}
     hshParam["auth_cognito"] = {"address": "", "login": "", "pwd": ""}
     hshParam["auth"] = {"adress": "", "societe": ""}
     hshParam["request"] = {}
+    hshParam["MaxRetryError"] = {"IterationMax": 2, "timeSleep": 120}
     __hshData = {}
 
     @property
     def data(self):
+        """
+        return data
+
+        Returns:
+            dict: data
+        """
         return self.__hshData
 
+    # pylint: disable-next=dangerous-default-value
     def __init__(self, phshParam={}):
         # Work variables
         self.token = ""
         self.login = ""
         self.auth = None
+        self.__NbIteration = 0
         self.session = requests.Session()
         # Start log manager
         self.log = libLog.Log()
 
         # Update of parameters
         self.hshParam.update(phshParam)
 
     def __Authentification(self, **kw):
+        # pylint: disable=broad-exception-raised
         hshOption = {"plogconnect": "DEBUG"}
         # Setting dictionary option
         if isinstance(kw, dict):
             hshOption.update(kw)
         address = self.hshParam["auth_cognito"]["address"]
         params = {
             "grant_type": "client_credentials",
             "scope": "ClientExterne/rest_read",
         }
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         auth = HTTPBasicAuth(
             self.hshParam["auth_cognito"]["login"],
             self.hshParam["auth_cognito"]["pwd"],
         )
-        resp = self.session.post(
-            address,
-            headers=headers,
-            params=params,
-            auth=auth,
-        )
+        try:
+            resp = self.session.post(
+                address,
+                headers=headers,
+                params=params,
+                auth=auth,
+            )
+            self.__NbIteration = 0
+        # TODO : Gestion en paramètre de 2 infos : waitingtime et nbiteration
+        #   avant déclenchement de l'erreur Max retries exceeded with url = urllib3.exceptions.MaxRetryError
+        except MaxRetryError as e:
+            if self.__NbIteration < self.hshParam["MaxRetryError"]["IterationMax"]:
+                time.sleep(self.hshParam["MaxRetryError"]["timeSleep"])
+                self.__NbIteration += 1
+                self.__Authentification(**kw)
+            else:
+                self.__NbIteration = 0
+                raise Exception(f"POST /auth/ {e}") from e
+
         if resp.status_code != 200:
             raise Exception(f"POST /auth/ {resp.status_code}")
         if hshOption["plogconnect"]:
             self.log.Write(
                 self.log.LEVEL[hshOption["plogconnect"]],
                 f"Connection {self.log.setStep} successfully",
             )
@@ -173,16 +205,18 @@
                         "plimit": hshOption["plimit"],
                     },
                 )
                 return None
             if resp.status_code != 200:
                 try:
                     msg = resp.json()["errors"][0]["detail"]
+                # pylint: disable-next=broad-exception-caught
                 except Exception:
                     msg = ""
+                # pylint: disable-next=broad-exception-raised
                 raise Exception(f"get /{pqueryfilter}/ {resp.status_code} : {msg}")
             self.__hshData[k] = self._mef_data_s9(resp.json())
             self.log.setStep = ""
 
     # //////////////////////////////////////////////////
     #     Action
     # //////////////////////////////////////////////////
@@ -317,31 +351,31 @@
         Args:
             data (json): Données json transmises par Sylob 9
 
         Returns:
             lst(dict): Tous les éléments mis en forme
         """
         ordre_colonne = []
-        format = {}
+        tmp_format = {}
         modele = {}
         retour = []
         # Déclaration des colonnes dans l'ordre
         ordre_colonne = data["colonne"]
         # Récupération des types attendus
         for col in data["colonneQueryWS"]:
-            format[col["libelle"]] = col["type"]
+            tmp_format[col["libelle"]] = col["type"]
         # enregistrement d'un dictionnaire modèle
         for k in ordre_colonne:
             modele[k] = ""
         # enregistrement de toutes les lignes
         for lig in data["ligneResultatWS"]:
             val = modele.copy()
             for idx, e in enumerate(lig["valeur"]):
                 k = ordre_colonne[idx]
-                if format[k] == "Boolean":
+                if tmp_format[k] == "Boolean":
                     val[k] = True if e == "Vrai" else False
                 else:
                     val[k] = e
             retour.append(val)
         return retour
 
 
@@ -353,16 +387,23 @@
     """Class Webservices S9000"""
 
     hshParam = {}
     __hshData = {}
 
     @property
     def data(self):
+        """
+        return data
+
+        Returns:
+            dict: data
+        """
         return self.__hshData
 
+    # pylint: disable-next=dangerous-default-value
     def __init__(self, phshParam={}):
         # Work variables
         self.token = ""
         self.login = ""
 
         # Start log manager
         self.log = libLog.Log()
@@ -371,40 +412,48 @@
         self.headers = {
             "Content-Type": "text/xml; charset=ISO-8859-1",
             "SOAPAction": "{address}/{request}",
             "Except": "100-continue",
             "Cache-Control": "no-cache",
             "Accept-Encoding": SKIP_HEADER,
         }
-        self.body = """<?xml version="1.0" encoding="ISO-8859-1"?>
-            <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope" xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" xmlns:tns="http://s9.mecapack.com:8091/webservice_test/ws_complet.php" xmlns:types="http://s9.mecapack.com:8091/webservice_test/ws_complet.php/encodedTypes" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
+        self.body = (
+            """<?xml version="1.0" encoding="ISO-8859-1"?>
+            <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope" """
+            + """xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" """
+            + """xmlns:tns="http://s9.mecapack.com:8091/webservice_test/ws_complet.php" """
+            + """xmlns:types="http://s9.mecapack.com:8091/webservice_test/ws_complet.php/encodedTypes" """
+            + """xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
                 <soap:Body soap:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
                     <q1:{request} xmlns:q1="http://s9.mecapack.com:8091/webservice_test/ws_complet.php?wsdl">
                         <Login xsi:type="xsd:string">{user}</Login>
                         <Password xsi:type="xsd:string">{password}</Password>
                         {param}
                     </q1:{request}>
                 </soap:Body>
             </soap:Envelope>
             """
+        )
 
         self.hshParam.update(phshParam)
 
+    # pylint: disable-next=unused-argument
     def Call(self, pqueryfilter, pbind=None, pparameters=None, **kw):
         """
         Lancement du web services avec infos à passer et résultats stockés dans data
 
         Args:
             pqueryfilter (str): filter string in queries dictionary
             pparameters (xml, optional): dict of key, value to send. Defaults to None.
             **plogrequest (LOG_LEVEL): Log level display for request. "None" for no display (default=DEBUG)
 
         Raises:
             Exception: No connection
         """
+        # pylint: disable=possibly-unused-variable
         hshOption = {"plogrequest": "DEBUG"}
         # Setting dictionary option
         if isinstance(kw, dict):
             hshOption.update(kw)
         address = self.hshParam["address"]
         site = f"{address}?wsdl"
         user = self.hshParam["user"]
@@ -440,23 +489,26 @@
             # prepared = self.session.prepare_request(req)
             # del prepared.headers["accept-encoding"]
             # resp = self.session.send(prepared)
             if resp.status_code != 200:
                 try:
                     # Récupérer le message contenu dans le xml
                     msg = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"]["SOAP-ENV:Fault"]
+                # pylint: disable-next=broad-exception-caught
                 except Exception:
                     msg = resp.text
+                # pylint: disable-next=broad-exception-raised
                 raise Exception(f"get /{pqueryfilter}/ {resp.status_code} : {msg}")
             # Transcrire le XML et récupérer le contenu significatif
             content = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"][f"ns1:{request}Response"][
                 "return"
             ]
             if content["type_erreur"]["#text"] != "000":
                 # ERREUR d'envoi
+                # pylint: disable-next=broad-exception-raised
                 raise Exception(f"retour /{pqueryfilter}/: {content['msg_erreur']['#text']}")
             else:
                 # décoder HTML
                 if "xml" in content:
                     self.__hshData[key] = xmltodict.parse(content["xml"]["#text"])
                 else:
                     res = {}
```

### Comparing `mecapacktools-1.0.0/pyproject.toml` & `mecapacktools-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
```

### Comparing `mecapacktools-1.0.0/README.md` & `mecapacktools-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Tools for Mecapack
 
 La doc est disponible en Html ou en MD
 
 ## installation par pip
 
 `pip install mecapacktools`
+
 Installer les extensions :
 
 `pip install mecapacktools[excel,sql,webservices]`
 
 ### Extensions diponibles :
 
-excel 
-Sql 
-WebServices 
+- excel 
+- Sql 
+- WebServices 
 
 ## Notes pour le développement:
 
 ### Installation
 
 `poetry install --with dev --all-extras`
 
@@ -31,11 +32,11 @@
 Changer la version :
 Dans le fichier pyproject.toml modifier :
 ```
 [tool.poetry]
 version = "1.0.0"
  ```
 
-Publier ... ` `
+Publier sur pypi `poetry publish --build`
```

### Comparing `mecapacktools-1.0.0/setup.py` & `mecapacktools-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '',
-    'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\nexcel \nSql \nWebServices \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier ... ` `\n\n\n\n',
+    'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mecapacktools-1.0.0/PKG-INFO` & `mecapacktools-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -26,23 +26,24 @@
 # Tools for Mecapack
 
 La doc est disponible en Html ou en MD
 
 ## installation par pip
 
 `pip install mecapacktools`
+
 Installer les extensions :
 
 `pip install mecapacktools[excel,sql,webservices]`
 
 ### Extensions diponibles :
 
-excel 
-Sql 
-WebServices 
+- excel 
+- Sql 
+- WebServices 
 
 ## Notes pour le développement:
 
 ### Installation
 
 `poetry install --with dev --all-extras`
 
@@ -56,12 +57,12 @@
 Changer la version :
 Dans le fichier pyproject.toml modifier :
 ```
 [tool.poetry]
 version = "1.0.0"
  ```
 
-Publier ... ` `
+Publier sur pypi `poetry publish --build`
```

