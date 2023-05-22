# Comparing `tmp/iamlogic_idm-1.1.tar.gz` & `tmp/iamlogic_idm-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlogic_idm-1.1.tar", last modified: Wed Apr 12 19:12:19 2023, max compression
+gzip compressed data, was "iamlogic_idm-1.2.tar", last modified: Mon May 22 06:34:03 2023, max compression
```

## Comparing `iamlogic_idm-1.1.tar` & `iamlogic_idm-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 19:12:19.672701 iamlogic_idm-1.1/
--rw-rw-rw-   0        0        0      432 2023-04-12 19:12:19.671689 iamlogic_idm-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 19:12:19.656604 iamlogic_idm-1.1/iamlogic_idm.egg-info/
--rw-rw-rw-   0        0        0      432 2023-04-12 19:12:19.000000 iamlogic_idm-1.1/iamlogic_idm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-12 19:12:19.000000 iamlogic_idm-1.1/iamlogic_idm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 19:12:19.000000 iamlogic_idm-1.1/iamlogic_idm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-12 19:12:19.000000 iamlogic_idm-1.1/iamlogic_idm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 19:12:19.000000 iamlogic_idm-1.1/iamlogic_idm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 19:12:19.669211 iamlogic_idm-1.1/idm_operation/
--rw-rw-rw-   0        0        0     9494 2023-04-12 19:11:50.000000 iamlogic_idm-1.1/idm_operation/IDM_Operation.py
--rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm-1.1/idm_operation/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-12 19:12:19.672701 iamlogic_idm-1.1/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-04-12 19:11:09.000000 iamlogic_idm-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:34:03.109250 iamlogic_idm-1.2/
+-rw-rw-rw-   0        0        0      432 2023-05-22 06:34:03.103251 iamlogic_idm-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 06:34:03.065786 iamlogic_idm-1.2/iamlogic_idm.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-05-22 06:34:02.000000 iamlogic_idm-1.2/iamlogic_idm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-22 06:34:02.000000 iamlogic_idm-1.2/iamlogic_idm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:34:02.000000 iamlogic_idm-1.2/iamlogic_idm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-22 06:34:02.000000 iamlogic_idm-1.2/iamlogic_idm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 06:34:02.000000 iamlogic_idm-1.2/iamlogic_idm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 06:34:03.100251 iamlogic_idm-1.2/idm_operation/
+-rw-rw-rw-   0        0        0    15927 2023-05-22 06:24:04.000000 iamlogic_idm-1.2/idm_operation/IDM_Operation.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm-1.2/idm_operation/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:34:03.110248 iamlogic_idm-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      635 2023-05-22 06:25:03.000000 iamlogic_idm-1.2/setup.py
```

### Comparing `iamlogic_idm-1.1/idm_operation/IDM_Operation.py` & `iamlogic_idm-1.2/idm_operation/IDM_Operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from IDMConnector import ConnectorClass
-import time, json, logging, mysql.connector, traceback
+import time, json, logging, mysql.connector, traceback, ast
 from datetime import timedelta
 
 logger = logging.getLogger()
 
 #######################
 #  Initialize_IDM_DB  #
 #######################
@@ -23,14 +23,15 @@
         self.db_cursor = self.db_conn.cursor(dictionary=True)
         return self
 
     # once the with block is over, the __exit__ method would be called
     # with that, you close the connnection
     def __exit__(self, exception_type, exception_val, trace):        
         try:
+           logger.debug("---INSIDE __exit__ close the connnection---")
            self.db_cursor.close()
            self.db_conn.close()
         except AttributeError: # isn't closable           
            return True # exception handled successfully
         
     # To perform operations such as create, update, delete etc. 
     # To retrieve all reconcilation data from IDM database.    
@@ -38,27 +39,42 @@
         logger.setLevel(log_level)     
         logger.debug("inside:Initialize_IDM_DB() , reconciliation_for_operation() func:")    
         self.db_cursor.execute("SELECT * FROM reconcile_sync_data WHERE mapping_id=%s"%(mappingid))
         self.result = self.db_cursor.fetchall()
         return self.result
     
     # To update reconciliation statistics whether success of the operation causes a mid-operation error.
-    # Passing the statics message and update the message for each reconcilation operations.
+    # Passing the statistics message and update the message for each reconcilation operations.
     def update_reconciliation_statistics(self, mappingid, json_data, actions, data):
         logger.debug("inside:Initialize_IDM_DB() , update_reconciliation_statistics() func:")        
         update_query = "UPDATE reconcile_sync_data SET statistics=%s WHERE mapping_id = %s AND reconcile_data = %s AND actions = %s"
-        values = (       
-            data,          
+        values = (
+            data,
             mappingid,
             json_data,
             actions
         )
         self.db_cursor.execute(update_query, values)
         self.db_conn.commit()
+
+    # To update reconciliation role sync statistics whether success of the operation causes a mid-operation error.
+    # Passing the role statistics message and update the message for each reconcilation operations.
+    def update_reconcile_role_sync_data_statistics(self, mappingid, json_str_data, action, msg_data):
+        logger.debug("inside:Initialize_IDM_DB() , update_reconcile_role_sync_data_statistics() func:")
+        update_role_query = "UPDATE reconcile_role_sync_data SET role_statistics=%s WHERE mapping_id = %s AND role_reconcile_data = %s AND role_actions = %s"
+        value = (
+                msg_data,
+                mappingid,  
+                json_str_data,              
+                action
+            )
         
+        self.db_cursor.execute(update_role_query, value)
+        self.db_conn.commit()
+    
 #######################
 #  IDMOperationClass  #
 #######################
 class IDMOperationClass(object):
 
     # This initialization is used to create an object for the IDMConnector to call the inside of the class methods.
     def __init__(self, configobject):
@@ -110,28 +126,86 @@
                 logger.debug(f"Processed Operation:{processed_operation}")
                 try:
                     logger.debug(f"obj{obj['id']}_currentObj{current_obj_id}")
                     if(obj['actions'] == "create"):
                         json_create_data = obj['reconcile_data']
                         logger.debug("inside:ConnectorClass() , sync() func if create try:")
                         createOp_response = self.idm_operation_obj.create(json.loads(obj['reconcile_data']))
+                        logger.debug(createOp_response)
+                        
                         with Initialize_IDM_DB(db_config) as dbObj:
                             dbObj.update_reconciliation_statistics(mappingid, json_create_data, obj['actions'], msg)
+                        # Role Operation for User
+                        if "user_role_data" in json.loads(obj['reconcile_data']):
+                            logger.debug("inside:ConnectorClass() , sync() func if create try: inside role operation create")
+                            json_create_load_reconcile_data = json.loads(obj['reconcile_data'])
+                            if json_create_load_reconcile_data["role_operation"] == "ADD":
+                                logger.debug("inside:ConnectorClass() , sync() func if create try: inside role operation create: ADD")
+                                for create_groups in json_create_load_reconcile_data["user_role_data"]["group"]:                                    
+                                    json_create_str_reconcile_data = str(json_create_load_reconcile_data["user_role_data"])
+                                    # Assign user to role call
+                                    self.idm_operation_obj.assignUserToRole(json_create_load_reconcile_data["user_role_data"]["username"], create_groups)
+                                    # Role Statistics Update
+                                    with Initialize_IDM_DB(db_config) as grpObj:
+                                        grpObj.update_reconcile_role_sync_data_statistics(mappingid, json_create_str_reconcile_data, "ADD", "role_added_to_user_success")
+
                     elif(obj['actions'] == "update"):
                         json_update_data = obj['reconcile_data']
                         logger.debug("inside:ConnectorClass() , sync() func elif update try:")
                         updateOp_response = self.idm_operation_obj.update(json.loads(obj['reconcile_data']))
                         with Initialize_IDM_DB(db_config) as dbObj:
                             dbObj.update_reconciliation_statistics(mappingid, json_update_data, obj['actions'], msg)
+                        # Role Operation for User
+                        if "user_role_data" in json.loads(obj['reconcile_data']):
+                            logger.debug("inside:ConnectorClass() , sync() func elif update try: inside role operation update")
+                            json_load_reconcile_data = json.loads(obj['reconcile_data'])
+                            if json_load_reconcile_data["role_operation"] == "ADD":
+                                logger.debug("inside:ConnectorClass() , sync() func elif update try: inside role operation update: ADD")
+                                for add_groups in json_load_reconcile_data["user_role_data"]["group"]:
+                                    # logger.debug(json_load_reconcile_data["user_role_data"]["username"])
+                                    # logger.debug(add_groups)
+                                    json_str_reconcile_data = str(json_load_reconcile_data["user_role_data"])
+                                    # Assign user to role call
+                                    self.idm_operation_obj.assignUserToRole(json_load_reconcile_data["user_role_data"]["username"], add_groups)
+                                    # Role Statistics Update
+                                    with Initialize_IDM_DB(db_config) as grpObj:
+                                        grpObj.update_reconcile_role_sync_data_statistics(mappingid, json_str_reconcile_data, "ADD", "role_added_to_user_success")
+
+                            elif json_load_reconcile_data["role_operation"] == "REMOVE":
+                                logger.debug("inside:ConnectorClass() , sync() func elif update try: inside role operation update: REMOVE")
+                                for rem_groups in json_load_reconcile_data["user_role_data"]["group"]:
+                                    logger.debug(json_load_reconcile_data["user_role_data"]["username"])
+                                    logger.debug(rem_groups)
+                                    json_str_reconcile_data = str(json_load_reconcile_data["user_role_data"])
+                                    # Remove user to role call
+                                    self.idm_operation_obj.RemoveUserToRole(json_load_reconcile_data["user_role_data"]["username"], rem_groups)
+                                    # Role Statistics Update
+                                    with Initialize_IDM_DB(db_config) as grpObj:
+                                        grpObj.update_reconcile_role_sync_data_statistics(mappingid, json_str_reconcile_data, "REMOVE", "role_removed_to_user_success")
+                                        
                     elif(obj['actions'] == "delete"):
                         json_delete_data = obj['reconcile_data']
                         logger.debug("inside:ConnectorClass() , sync() func elif delete try:")
                         deleteOp_response = self.idm_operation_obj.delete(json.loads(obj['reconcile_data']))
                         with Initialize_IDM_DB(db_config) as dbObj:
-                            dbObj.update_reconciliation_statistics(mappingid, json_delete_data, obj['actions'], msg)                  
+                            dbObj.update_reconciliation_statistics(mappingid, json_delete_data, obj['actions'], msg)
+                        # Role Operation for User
+                        if "user_role_data" in json.loads(obj['reconcile_data']):
+                            logger.debug("inside:ConnectorClass() , sync() func elif delete try: inside role operation delete")
+                            json_delete_load_reconcile_data = json.loads(obj['reconcile_data'])
+                            if json_delete_load_reconcile_data["role_operation"] == "REMOVE":
+                                logger.debug("inside:ConnectorClass() , sync() func elif delete try: inside role operation delete: REMOVE")
+                                for remove_groups in json_delete_load_reconcile_data["user_role_data"]["group"]:                                    
+                                    json_del_str_reconcile_data = str(json_delete_load_reconcile_data["user_role_data"])
+                                    # Assign user to role call
+                                    self.idm_operation_obj.assignUserToRole(json_delete_load_reconcile_data["user_role_data"]["username"], remove_groups)
+                                    # Role Statistics Update
+                                    with Initialize_IDM_DB(db_config) as grpObj:
+                                        grpObj.update_reconcile_role_sync_data_statistics(mappingid, json_del_str_reconcile_data, "REMOVE", "role_removed_to_user_success")
+
                     elif(obj['actions'] == "ignore"):
                         json_ignore_data = obj['reconcile_data']
                         logger.debug("inside:ConnectorClass() , sync() func elif ignore try:")
                         ignore_msg = "No operation can be performed which is ignored by behaviour" 
                         with Initialize_IDM_DB(db_config) as dbObj:
                             dbObj.update_reconciliation_statistics(mappingid, json_ignore_data, obj['actions'], ignore_msg)
                     processed_operation.add(obj['id'])
```

### Comparing `iamlogic_idm-1.1/setup.py` & `iamlogic_idm-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iamlogic_idm',
-    version='1.1',
+    version='1.2',
     description='IAMLOGIC IDM package',   
     author_email='info@iamlogic.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'cryptography',
         'sqlalchemy',
         'mysql-connector-python',
-        'hvac'       
+        'hvac'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

