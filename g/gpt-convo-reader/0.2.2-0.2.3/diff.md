# Comparing `tmp/gpt-convo-reader-0.2.2.tar.gz` & `tmp/gpt-convo-reader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-convo-reader-0.2.2.tar", last modified: Wed May 17 11:38:40 2023, max compression
+gzip compressed data, was "gpt-convo-reader-0.2.3.tar", last modified: Mon May 22 16:44:39 2023, max compression
```

## Comparing `gpt-convo-reader-0.2.2.tar` & `gpt-convo-reader-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.2.2/LICENSE
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     3252 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2662 2023-05-17 11:36:50.000000 gpt-convo-reader-0.2.2/README.md
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/setup.cfg
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1085 2023-05-17 11:37:23.000000 gpt-convo-reader-0.2.2/setup.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/src/
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/src/converter/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.2.2/src/converter/__init__.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     1542 2023-05-17 10:04:19.000000 gpt-convo-reader-0.2.2/src/converter/config.py
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     2391 2023-05-17 10:11:35.000000 gpt-convo-reader-0.2.2/src/converter/convert.py
--rwxrwxr-x   0 romilly   (1000) romilly   (1000)     4488 2023-05-17 11:38:21.000000 gpt-convo-reader-0.2.2/src/converter/gui.py
-drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-17 11:38:40.047485 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/
--rw-rw-r--   0 romilly   (1000) romilly   (1000)     3252 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/PKG-INFO
--rw-rw-r--   0 romilly   (1000) romilly   (1000)      398 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/entry_points.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       23 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/requires.txt
--rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-17 11:38:40.000000 gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/top_level.txt
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-22 16:44:39.029594 gpt-convo-reader-0.2.3/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1072 2023-05-07 14:42:35.000000 gpt-convo-reader-0.2.3/LICENSE
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3252 2023-05-22 16:44:39.029594 gpt-convo-reader-0.2.3/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2662 2023-05-17 11:36:50.000000 gpt-convo-reader-0.2.3/README.md
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      828 2023-05-22 16:44:39.029594 gpt-convo-reader-0.2.3/setup.cfg
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1085 2023-05-22 16:43:52.000000 gpt-convo-reader-0.2.3/setup.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-22 16:44:38.965594 gpt-convo-reader-0.2.3/src/
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-22 16:44:39.029594 gpt-convo-reader-0.2.3/src/converter/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      343 2023-05-08 12:59:31.000000 gpt-convo-reader-0.2.3/src/converter/__init__.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     1542 2023-05-17 10:04:19.000000 gpt-convo-reader-0.2.3/src/converter/config.py
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     2489 2023-05-22 16:41:22.000000 gpt-convo-reader-0.2.3/src/converter/convert.py
+-rwxrwxr-x   0 romilly   (1000) romilly   (1000)     4665 2023-05-18 13:38:50.000000 gpt-convo-reader-0.2.3/src/converter/gui.py
+drwxrwxr-x   0 romilly   (1000) romilly   (1000)        0 2023-05-22 16:44:39.029594 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)     3252 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)      398 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)        1 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       51 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       23 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/requires.txt
+-rw-rw-r--   0 romilly   (1000) romilly   (1000)       10 2023-05-22 16:44:38.000000 gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/top_level.txt
```

### Comparing `gpt-convo-reader-0.2.2/LICENSE` & `gpt-convo-reader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2.2/PKG-INFO` & `gpt-convo-reader-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpt-convo-reader-0.2.2/README.md` & `gpt-convo-reader-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2.2/setup.cfg` & `gpt-convo-reader-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2.2/setup.py` & `gpt-convo-reader-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpt-convo-reader",
-    version="0.2.2",
+    version="0.2.3",
     author="Romilly Cocking",
     author_email="romilly.cocking@gmail.com",
     description="Lets you find, view and format the conversations you've had with ChatGPT in the playground.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/romilly/gpt-convo-reader",
     project_urls={
```

### Comparing `gpt-convo-reader-0.2.2/src/converter/config.py` & `gpt-convo-reader-0.2.3/src/converter/config.py`

 * *Files identical despite different names*

### Comparing `gpt-convo-reader-0.2.2/src/converter/convert.py` & `gpt-convo-reader-0.2.3/src/converter/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,19 @@
     def __repr__(self) -> str:
         return str(self)
 
     @classmethod
     def from_json_dict(cls, json_dict: Dict[str, Any]) -> 'Message':
         author = json_dict['author']
         role = author['role']
-        parts = json_dict['content']['parts']
+        content = json_dict['content']
+        if 'parts' in content:
+            parts = content['parts']
+        else:
+            parts = []
         return cls(role=role, contents=parts)
 
 
 class Conversation:
     def __init__(self, title: str, update_time: float, messages: List[Message]):
         self.title = title
         self.update_time = update_time
```

### Comparing `gpt-convo-reader-0.2.2/src/converter/gui.py` & `gpt-convo-reader-0.2.3/src/converter/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,19 +74,21 @@
             self.conversation_text.append('\n')
 
     def open_function(self):
         file_name = self.select_file(filetypes=[['zip files', '*.zip']],
                                      folder=self.configuration.zip_directory)
         if len(file_name) > 0:
             self.conversations = convert(file_name)
+            self.sort_conversations()
             # Add the conversation titles to the ListBox
             self.show_full_convo_list()
 
     def load_all(self):
         self.conversations = convert_all(self.configuration.zip_directory, self.configuration.prefix)
+        self.sort_conversations()
         self.show_full_convo_list()
 
     def show_full_convo_list(self):
         for title in self.conversations:
             self.conversation_list.append(title)
 
     def save_function(self):
@@ -99,14 +101,17 @@
         with open(file_path, 'w') as mdf:
             mdf.write(f'# {self.selected_conversation.title}\n\n')
             mdf.write(f'{self.selected_conversation.updated()}\n\n')
             for message in self.selected_conversation.messages:
                 mdf.write(message.markdown())
                 mdf.write('\n\n')
 
+    def sort_conversations(self):
+        self.conversations = dict(sorted(self.conversations.items()))
+
 
 if __name__ == "__main__":
     app = ConversationGUI()
     app.font ="Helvetica"
     app.text_size = 12
     # Show the app
     app.display()
```

### Comparing `gpt-convo-reader-0.2.2/src/gpt_convo_reader.egg-info/PKG-INFO` & `gpt-convo-reader-0.2.3/src/gpt_convo_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-convo-reader
-Version: 0.2.2
+Version: 0.2.3
 Summary: Lets you find, view and format the conversations you've had with ChatGPT in the playground.
 Home-page: https://github.com/romilly/gpt-convo-reader
 Author: Romilly Cocking
 Author-email: romilly.cocking@gmail.com
 Project-URL: Bug Tracker, https://github.com/romilly/gpt-convo-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

