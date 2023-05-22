# Comparing `tmp/lts-mpsmqutils-2.0.2a0.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a0.tar", last modified: Wed Jan 18 21:15:00 2023, max compression
+gzip compressed data, was "lts-mpsmqutils-2.0.2a12.tar", last modified: Sat May 20 01:40:17 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a0.tar` & `lts-mpsmqutils-2.0.2a12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-01-18 21:15:00.565190 lts-mpsmqutils-2.0.2a0/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6713 2023-01-18 21:15:00.564590 lts-mpsmqutils-2.0.2a0/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a0/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-01-18 21:15:00.561779 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6713 2023-01-18 21:15:00.000000 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      343 2023-01-18 21:15:00.000000 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-01-18 21:15:00.000000 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       78 2023-01-18 21:15:00.000000 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-01-18 21:15:00.000000 lts-mpsmqutils-2.0.2a0/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-01-18 21:15:00.563036 lts-mpsmqutils-2.0.2a0/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a0/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27901 2023-01-18 21:13:58.000000 lts-mpsmqutils-2.0.2a0/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7278 2022-11-22 20:44:49.000000 lts-mpsmqutils-2.0.2a0/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-01-18 21:15:00.563830 lts-mpsmqutils-2.0.2a0/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a0/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a0/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-01-18 21:15:00.565410 lts-mpsmqutils-2.0.2a0/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      998 2023-01-18 21:14:32.000000 lts-mpsmqutils-2.0.2a0/setup.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.185020 lts-mpsmqutils-2.0.2a12/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5501 2023-05-20 01:40:17.182383 lts-mpsmqutils-2.0.2a12/PKG-INFO
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5103 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/README.md
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.098631 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5501 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 appuser   (1000) appuser   (1000)      343 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       62 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       11 2023-05-20 01:40:16.000000 lts-mpsmqutils-2.0.2a12/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.139251 lts-mpsmqutils-2.0.2a12/mpsmqutils/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)        0 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/__init__.py
+-rw-r--r--   0 appuser   (1000) appuser   (1000)    29537 2023-05-20 01:23:03.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/messagehandler.py
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     7247 2023-05-12 14:23:30.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/mqutils.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-05-20 01:40:17.177213 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)        0 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     4783 2022-04-07 20:19:50.000000 lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-05-20 01:40:17.186135 lts-mpsmqutils-2.0.2a12/setup.cfg
+-rw-r--r--   0 appuser   (1000) appuser   (1000)      899 2023-05-20 01:23:05.000000 lts-mpsmqutils-2.0.2a12/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a0/README.md` & `lts-mpsmqutils-2.0.2a12/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a0/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a12/mpsmqutils/messagehandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-import datetime, email, json, os, re, smtplib, time, traceback
+import datetime, email, json, os, re, smtplib, time, traceback, sys
 import celery as celeryapp
 
+# https://www.geeksforgeeks.org/python-import-from-parent-directory/
+sys.path.append('../app')
+from app import worker_task
+
 from textwrap import dedent
 
 import mpsmqutils.mqutils as mqutils
 # Job tracker module
 import mpsjobtracker.trackers.jobtracker as jobtracker
 job_tracker = jobtracker.JobTracker()
 
@@ -31,41 +35,90 @@
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 DLQ_QUEUE = os.getenv('MQ_DLQ_QUEUE', '/queue/ActiveMQ.DLQ')
 
 # Email SMTP host for use in notify
 NOTIFY_MAIL_RELAY=os.getenv('MQ_NOTIFY_MAIL_RELAY', None)
 NOTIFY_DEFAULT_EMAIL=os.getenv('MQ_NOTIFY_DEFAULT_EMAIL', None)
 
+# Logging
+#import logging as logger
+#logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'DEBUG'))
+# https://stackoverflow.com/questions/15727420/using-logging-in-multiple-modules
+#logger = logging.getLogger(__name__)
+#app_name = __name__
+
+def call_worker_do_task(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
+    print("************************ PRINT MQUTILS MQLISTENER - CALL WORKER DO TASK *******************************")
+    '''Call the worker task class do task method and process the response in a standard format'''
+
+    result = {
+      'success': False,
+      'error': None,
+      'message': None
+    }
+    job_ticket_id_str = f" job_ticket_id: {job_ticket_id}" if job_ticket_id else ""
+    parent_job_ticket_id_str = f" parent_job_ticket_id: {parent_job_ticket_id}" if parent_job_ticket_id else ""
+    print(f'mqlistener call_worker_do_task START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
+
+    """
+      Call worker task class do task method
+    """
+    try:
+        message_data = { 'task_name': task_name }
+        if add_params:
+            message_data = {**json_params, **add_params}
+        if job_ticket_id:
+            message_data['job_ticket_id'] = job_ticket_id
+        if parent_job_ticket_id:
+            message_data['parent_job_ticket_id'] = parent_job_ticket_id
+        print(message_data)
+        wt = worker_task.WorkerTask()
+        response_json = wt.do_task(message_data)
+    except Exception as e:
+        print(e)
+        raise Exception(e)
+
+    print(f'mqlistener call_worker_do_task COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
+
+    print(response_json)
+
+    success = False if not response_json.get('success') else True
+    print("success:")
+    print(success)
+    result['success'] = success
+    result['error'] = response_json.get('error', None)
+    result['message'] = response_json.get('message', None)
+
+    return result
+
 def call_worker_api(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
     print("************************ MQUTILS MQLISTENER - CALL WORKER API *******************************")
     '''Call the worker API and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None
     }
-    print("result:")
-    print(result)
     job_ticket_id_str = f" job_ticket_id: {job_ticket_id}" if job_ticket_id else ""
     parent_job_ticket_id_str = f" parent_job_ticket_id: {parent_job_ticket_id}" if parent_job_ticket_id else ""
     print(f'mqlistener call_worker_api START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
 
     """
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
 
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg, flush=True)
+            print(error_msg)
             raise Exception(error_msg)
         url = worker_url + '/' + worker_url_endpoint
-        print('mqlistener call_worker_api url {}'.format(url), flush=True)
+        print('mqlistener call_worker_api url {}'.format(url))
         json_params = { 'task_name': task_name }
         if add_params:
             json_params = {**json_params, **add_params}
         if job_ticket_id:
             json_params['job_ticket_id'] = job_ticket_id
         if parent_job_ticket_id:
             json_params['parent_job_ticket_id'] = parent_job_ticket_id
@@ -77,30 +130,30 @@
         print(response)
     except Exception as e:
         print(e)
         if job_ticket_id:
             job_tracker.append_error(job_ticket_id, 'mqlistener call_worker_api API call failed', traceback.format_exc(), True)
         raise Exception(e)
 
-    print(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}', flush=True)
+    print(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}')
 
     response_json = response.json()
     print(response_json)
 
     success = False if not response_json.get('success') else True
     print("success:")
     print(success)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
 
     return result
 
 def call_generic_worker_api(message_data, worker_endpoint):
-    print("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************", flush=True)
+    print("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************")
     '''Call the worker API and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None,
       'next_queue': None
@@ -110,34 +163,33 @@
     """
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg, flush=True)
+            print(error_msg)
             raise Exception(error_msg)
         url = worker_url
-        print('mqlistener call_generic_worker_api url {}'.format(url), flush=True)
+        print('mqlistener call_generic_worker_api url {}'.format(url))
         # The worker uses a self-signed certificate and it does not need to be verified since the listener makes a request to the worker inside the same container internally
         response = http_client.post(url, json = message_data, verify=False)
-        print('made request', flush=True)
         response.raise_for_status()
-        print('response.raise_for_status', flush=True)
-        print(response, flush=True)
+        print('response.raise_for_status')
+        print(response)
     except Exception as e:
         print(e)
         raise Exception(e)
 
     response_json = response.json()
-    print(response_json, flush=True)
+    print(response_json)
 
     success = False if not response_json.get('success') else True
-    print("success:", flush=True)
-    print(success, flush=True)
+    print("success:")
+    print(success)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
     result['next_queue'] = response_json.get('next_queue', None)
 
     return result
 
@@ -182,15 +234,15 @@
         print('job_tracker_doc {}'.format(job_tracker_doc))
         status = job_tracker_doc['job_management']['job_status']
         if status in completed_statuses:
             print(f'Status {status} counts as completed, assuming job is complete')
             #Assume if the tracker is completed or not there, that this job is no longer running
             return
 
-        print(f"Dispatching based on category: {category}", flush=True)
+        print(f"Dispatching based on category: {category}")
         if (category == "ingest"):
             task_success = self.__ingest_message_handler(self.message)
         elif (category == "task_management"):
             task_success = self.__task_management_message_handler(self.message)
         elif (category == "service"):
             task_success = self.__service_message_handler(self.message)
         elif (category == "cache_management"):
@@ -198,23 +250,22 @@
 
         #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
                 # TODO: ack is sent automatically after task completes
                 # TODO: unsure how nack works in the case of celery
                 job_tracker.set_job_status('failed', job_ticket_id, "failed")
-                print('Task unsuccessful')
+                logger.warning('Task unsuccessful')
                 # self.conn.nack(message_id, self._sub_id)
 
         #TODO- Handle
         print('processed message for job id {}'.format(job_ticket_id))
 
     def __ingest_message_handler(self, message_data):
         print("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
-        print('ingest message')
         job_ticket_id = message_data.get('job_ticket_id')
         print('job_ticket_id {}'.format(job_ticket_id))
         parent_job_ticket_id = message_data.get('parent_job_ticket_id', None)
         print('parent_job_ticket_id {}'.format(parent_job_ticket_id))
         task_name = message_data.get('task_name')
         print('task_name {}'.format(task_name))
         previous_step_status = message_data.get('previous_step_status', 'success')
@@ -263,18 +314,17 @@
             #Update the timestamp
             job_tracker.update_timestamp(job_ticket_id)
             print("SUCCESSFULLY UPDATED TIMESTAMP job_ticket_id {} parent_job_ticket_id {}".format(job_ticket_id, parent_job_ticket_id))
         except Exception as e:
             print(e)
             return False
 
-
-        # Call task
+        # Call worker class do task method
         try:
-            worker_response = call_worker_api(task_name, job_ticket_id, parent_job_ticket_id, worker_url_endpoint)
+            worker_response = call_worker_do_task(task_name, job_ticket_id, parent_job_ticket_id, worker_url_endpoint)
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
             print("SUCCESS IN WORKER RESPONSE TRY BLOCK")
         except Exception as e:
             print(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
@@ -287,15 +337,14 @@
                 #There are no more items to queue so the job is actually finished.
                 #TODO: LTSIIIF-499 Call manifest services at the end of the workflow
                 print('******** LAST TASK COMPLETED ********')
                 print('previous_step_status {} job_ticket_id {} parent_job_ticket_id {}'.format(previous_step_status, job_ticket_id, parent_job_ticket_id))
             else:
                 try:
                     json_message = json.loads(nextmessage)
-                    print('json_message {}'.format(json_message))
                     print(json_message)
                 except ValueError as e:
                     print(e)
                     job_tracker.append_error(job_ticket_id, 'Unable to get parse the next queue message',  traceback.format_exc(), False)
                     raise e
 
                 # Set the queue name to match the worker type
@@ -310,16 +359,16 @@
                 tracker_doc["job_management"]["previous_step_status"] = json_message["previous_step_status"]
                 try:
                     print('******** UPDATE TRACKER FILE ********')
                     updated_tracker_doc = job_tracker.replace_tracker_doc(tracker_doc)
                     print('updated_tracker_doc {}'.format(updated_tracker_doc))
                 except Exception as e:
                     #TODO what to do here - what does this mean if the tracker retrieval fails?
-                    print("TRACKER RETRIEVAL FAILS")
-                    print(e, flush=True)
+                    print("TRACKER RETRIEVAL FAILED")
+                    print(e)
                     raise e
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[nextmessage], kwargs={}, queue=queue)
         print('task_success')
         print(task_success)
         return task_success
 
     def __task_management_message_handler(self, message_data):
@@ -343,39 +392,37 @@
 
         try:
             job_tracker.set_job_status('running', job_ticket_id)
             # Run the service
             # Update timestamp file before do task
             print('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
-            print('CALLING DO TASK')
-            print('job_ticket_id {} task_name {} category task_management'.format(job_ticket_id, task_name))
         except Exception as e:
             print(e)
             task_success = False
 
         # Call do task
         print("******************* CALLING WORKER API DO TASK __task_management_message_handler *******************")
         try:
             print("call_worker_api task_name {} job_ticket_id {} parent_job_ticket_id {} do_task")
             worker_response = call_worker_api(task_name, job_ticket_id, parent_job_ticket_id, 'do_task')
             print("worker_response")
             print(worker_response)
         except Exception as e:
-            print(e)
             print("CALLING WORKER API DO TASK FAILED")
+            print(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
         print("******************* HANDLE WORKER RESPONSE *******************")
         try:
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
         except Exception as e:
-            print(e)
             print("HANDLE WORKER RESPONSE FAILED")
+            print(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
         print("task_success")
         print(task_success)
 
         #Ack message was already handled above
@@ -402,15 +449,15 @@
     def __cache_management_message_handler(self, message_data, message_id):
         print('cache management message')
         try:
             worker_response = call_worker_api('update_cache')
         except Exception as e:
             import traceback;
             print('Failure in cache management handler')
-            print(traceback.format_exc(), flush=True)
+            print(traceback.format_exc())
             # print('Nack message_id {}'.format(message_id))
             # self.conn.nack(message_id, self._sub_id)
             # TODO: HOW DO WE NACK IN CELERY?
             return False
         return True
 
 # Generalized listener based on MQListener for use with components that do not use jobtracker
@@ -425,17 +472,17 @@
         task_success = False
 
         task_success = self.__generic_message_handler(self.message, self.worker_endpoint)
 
         # #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
-                print('Task unsuccessful')
+                logger.warning('Task unsuccessful')
                 # TODO: HOW TO NACK A TASK?
-        # print('processed message message_id {}'.format(message_id), flush=True)
+        # print('processed message message_id {}'.format(message_id))
 
     def __generic_message_handler(self, message_data, worker_endpoint):
         print("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
         task_success = False
 
         # Call task
         try:
@@ -475,15 +522,15 @@
 #         print("Handling message from notification queue")
 #         message = json.loads(frame.body)
 
 #         if not 'to' in message:
 #             message['to'] = [NOTIFY_DEFAULT_EMAIL]
 
 #         if message['method'] == "email":
-#             print("Method is email", flush=True)
+#             print("Method is email")
 #             if isinstance(message['to'], str):
 #                 message['to'] = recipient_separators.split(message['to'])
 #             msg = dedent(f"""\
 #             From: {message['from']}
 #             Subject: {message['subject']}
 
 #             """) + message["message"]
@@ -496,15 +543,15 @@
 #                         to_addrs=message['to'],
 #                         msg = msg
 #                     )
 #                 except Exception as e:
 #                     print(f"Sendmail failed with exception {e}")
 #                     import traceback
 #                     print(traceback.format_exc())
-#                 print(f"Result of sendmail: {result}", flush=True)
+#                 print(f"Result of sendmail: {result}")
 #         else:
 #             raise RuntimeError('Unknown method for notification')
 
 
 #     def handle_dlq(self, frame):
 #         print('Handling DLQ notification')
 #         message = json.loads(frame.body)
@@ -529,15 +576,15 @@
 #                     msg = msg
 #                 )
 #             except Exception as e:
 #                 print(f"Sendmail failed with exception {e}")
 #                 import traceback
 #                 print(traceback.format_exc())
 #                 raise(e)
-#             print(f"Result of sendmail: {result}", flush=True)
+#             print(f"Result of sendmail: {result}")
 
 #     def on_message(self, frame):
 #         headers, body = frame.headers, frame.body
 #         message_id = headers.get('message-id')
 #         sub_id = int(headers.get('subscription'))
 #         print(f'handling message {message_id} from sub {sub_id}')
 #         try:
@@ -572,27 +619,27 @@
 #         time.sleep(2)
 #         if not conn.is_connected():
 #             print('Disconnected in loop, reconnecting')
 #             connect_and_subscribe(conn)
 
 # def initialize_generic_listener(worker_endpoint='do_task'):
 #     if _failback_host and _failback_port:
-#         print('failback host and port in use', flush=True)
+#         print('failback host and port in use')
 #         conn = stomp.Connection([(_host, _port),(_failback_host, _failback_port)], heartbeats=(40000, 40000), keepalive=True)
 #     else:
-#         print('failback host and port not in use', flush=True)
+#         print('failback host and port not in use')
 #         conn = stomp.Connection([(_host, _port)], heartbeats=(40000, 40000), keepalive=True)
 #     conn.set_listener('', GenericListener(conn, worker_endpoint))
 #     conn_list.append(conn)
 #     connect_and_subscribe(conn)
 #     # http_clients://github.com/jasonrbriggs/stomp.py/issues/206
 #     while True:
 #         time.sleep(2)
 #         if not conn.is_connected():
-#             print('Disconnected in loop, reconnecting', flush=True)
+#             print('Disconnected in loop, reconnecting')
 #             connect_and_subscribe(conn)
 
 # def initialize_notify_listener():
 #     if _failback_host and _failback_port:
 #         print('failback host and port in use')
 #         conn = stomp.Connection([(_host, _port),(_failback_host, _failback_port)], heartbeats=(40000, 40000), keepalive=True)
 #     else:
@@ -603,8 +650,8 @@
 #     connect_and_subscribe(conn, DLQ_QUEUE, sub_id=DLQ_SUB)
 #     # http_clients://github.com/jasonrbriggs/stomp.py/issues/206
 #     while True:
 #         time.sleep(2)
 #         if not conn.is_connected():
 #             print('Disconnected in loop, reconnecting')
 #             connect_and_subscribe(conn, NOTIFY_QUEUE, sub_id=NOTIFY_SUB)
-#             connect_and_subscribe(conn, DLQ_QUEUE, sub_id=DLQ_SUB)
+#             connect_and_subscribe(conn, DLQ_QUEUE, sub_id=DLQ_SUB)
```

### Comparing `lts-mpsmqutils-2.0.2a0/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a12/mpsmqutils/mqutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, json, time, datetime, stomp
+import os, json, time, datetime
 from contextlib import contextmanager
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from traceback import format_exc
 # Job tracker module
 import mpsjobtracker.trackers.jobtracker as jobtracker
 
 jt = None
@@ -24,153 +24,148 @@
 _hosts = [(_host, _port,)]
 
 if _failback_host and _failback_port:
     _hosts.append((_failback_host, _failback_port,))
 
 _max_reconnects = 1000
 
+# Logging
+import logging
+logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'INFO'))
+logger = logging.getLogger(__name__)
+
 def create_initial_queue_message(job_ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message to be picked up by the worker'''
-    print("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
     try:
         message = __create_ingest_message(job_ticket_id, 0, "success", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_initial_queue_message")
-        print(message)
+        logger.debug("MESSAGE TO QUEUE create_initial_queue_message")
+        logger.debug(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_next_queue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a message for the next task in the job'''
-    print("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
     message = None
     try:
         message = __create_ingest_message(ticket_id, 1, "success", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_next_queue_message")
-        print(message)
+        logger.debug("MESSAGE TO QUEUE create_next_queue_message")
+        logger.debug(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_requeue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message for the current task to be requeued'''
-    print("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
     try:
         jt = get_jt()
         job_tracker_file = jt.get_tracker_document(ticket_id)
         job_management = job_tracker_file.get("job_management")
         if (job_management is None):
             raise Exception ('Tracker File is malformed, missing job_management')
         prev_step_status = job_management["previous_step_status"]
         message = __create_ingest_message(ticket_id, 0, prev_step_status, parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_requeue_message")
-        print(message)
+        logger.debug("MESSAGE TO QUEUE create_requeue_message")
+        logger.debug(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_revert_message(ticket_id, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
     '''Creates a queue json message to revert the previous task
          Returns None if there is no previous message'''
     message = None
     try:
         message = __create_ingest_message(ticket_id, -1, "failed", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_revert_message")
-        print(message)
+        logger.debug("MESSAGE TO QUEUE create_revert_message")
+        logger.debug(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "task_manager_worker_inprocess",
         "previous_step_status" : "success",
         "category": "task_management"
     }
-    print(json_message)
-    print("parent job ticket id:")
-    print(parent_job_ticket_id)
     if parent_job_ticket_id:
         json_message["parent_job_ticket_id"] = parent_job_ticket_id
     message = json.dumps(json_message)
-    print(message)
+    logger.debug(message)
     return message
 
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 def create_notification(sender, recipients, subject, message, method="email", **opts):
-    print("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
+    logger.debug("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
     jt=get_jt()
     message = json.dumps({
         "from": sender,
         "to": recipients,
         "subject": subject,
         "message": message,
         "options": opts,
         "timestamp": jt.get_timestamp_utc_now(),
         "method": method
     })
-    print(message)
+    logger.debug(message)
 
     with managed_mq_connect() as conn:
         conn.send(NOTIFY_QUEUE, message, headers = {"persistent": "true"})
 
 CACHE_MANAGER_QUEUE = os.getenv('MQ_CACHE_MANAGER_QUEUE', '/queue/mps-asset-db-cache')
 def create_cache_refresh_message(**opts):
-    print("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
     jt = get_jt()
     message = json.dumps({
         "category": "cache_management",
         "timestamp": jt.get_timestamp_utc_now(),
         "options": opts
     })
-    print(message)
+    logger.debug(message)
     with managed_mq_connect() as conn:
         conn.send(CACHE_MANAGER_QUEUE, message, headers = {"persistent": "true"})
 
 def create_multi_asset_ingest_queue_message(job_ticket_id):
-    print("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "multi_asset_ingest",
         "previous_step_status" : "success",
         "category": "task_management"
     }
-    print(json_message)
+    logger.debug(json_message)
     message = json.dumps(json_message)
     return message
 
 def __create_ingest_message(ticket_id, step_number_increment, prev_step_status, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
+    logger.debug("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
     '''Helper method for the create messages above'''
     jt = get_jt()
-    print(ticket_id)
-    print(parent_job_ticket_id)
     job_tracker_file = jt.get_tracker_document(ticket_id)
 
     timestamp = jt.get_timestamp_utc_now()
 
     job_management = job_tracker_file.get("job_management")
     if (job_management is None):
-        print("Malformed Tracker File")
+        logger.error("Malformed Tracker File")
         raise Exception ('Tracker File is malformed, missing job_management.')
 
     current_step = int(job_management["current_step"])
-    print("current step:")
-    print(current_step)
     step_number = current_step + step_number_increment
-    print("step number:")
-    print(step_number)
-
     steps_list = job_management["steps"]
     # Get step by looking up the step by step number
     event = jt.filter_element_by_property(steps_list, "step_number", step_number)
     if not event:
         return None
     task_name = event[0]["task_name"]
     event_name = event[0]["worker_type"]
@@ -181,15 +176,12 @@
         "job_ticket_id": str(ticket_id),
         "task_name": task_name,
         "current_step": step_number,
         "previous_step_status": prev_step_status,
         "category": "ingest"
     }
     if parent_job_ticket_id:
-        print("parent job ticket id:")
-        print(parent_job_ticket_id)
         msg_json["parent_job_ticket_id"] = parent_job_ticket_id
 
-    print("msg json:")
-    print(msg_json)
+    logger.debug(msg_json)
     message = json.dumps(msg_json)
     return message
```

### Comparing `lts-mpsmqutils-2.0.2a0/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a12/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a0/setup.py` & `lts-mpsmqutils-2.0.2a12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a",
-    author="Katie Amaral",
-    author_email="kathryn_amaral@harvard.edu",
+    version="2.0.2a12",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
-        'stomp.py==8.0.1',
         'lts-mpsjobtracker-mongo',
         'requests',
         'pytest',
         'tenacity',
         'cryptography'
     ],
     classifiers=[
```

