# Comparing `tmp/openAIInsight-0.0.4-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5288 bytes, number of entries: 7
+Zip file size: 5400 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx     9644 b- defN 23-May-12 06:15 openAIInsight/OpenAI_PineConeVector.py
--rw-rw-r--  2.0 unx     2200 b- defN 23-May-10 11:41 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      596 b- defN 23-May-12 06:35 openAIInsight-0.0.4.dist-info/RECORD
-7 files, 14228 bytes uncompressed, 4222 bytes compressed:  70.3%
+-rw-rw-r--  2.0 unx     3238 b- defN 23-May-22 07:03 openAIInsight/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      596 b- defN 23-May-22 07:14 openAIInsight-0.0.5.dist-info/RECORD
+7 files, 15266 bytes uncompressed, 4334 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: openAIInsight/OpenAI_PineConeVector.py
 Comment: 
 
 Filename: openAIInsight/__init__.py
 Comment: 
 
-Filename: openAIInsight-0.0.4.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.5.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.4.dist-info/METADATA
+Filename: openAIInsight-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.4.dist-info/WHEEL
+Filename: openAIInsight-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.4.dist-info/top_level.txt
+Filename: openAIInsight-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.4.dist-info/RECORD
+Filename: openAIInsight-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/__init__.py

```diff
@@ -1,57 +1,66 @@
 import requests, json, traceback, openai
 from flask import request
 import loggerutility as logger
+import commonutility as common
 
 class openAI:
     def getCompletionEndpoint(self):
         try:
             jsonData = request.get_data('jsonData', None)
             jsonData = json.loads(jsonData[9:])
-            logger.log(f"jsonData openAI class::: {jsonData}","0")
+            logger.log(f"\njsonData openAI class::: {jsonData}","0")
 
             licenseKey   = jsonData['license_key']
             insightInput = jsonData['insight_input']
             openai.api_key = licenseKey
             openAI_trainingData = open("openAI_trainingData.txt","r").read()
             
-            response = openai.Completion.create(
-            model="code-davinci-001",
-            prompt= openAI_trainingData + insightInput,
-            temperature=0.25,
-            max_tokens=198,
-            top_p=0.5,
-            frequency_penalty=0,
-            presence_penalty=0,
-            stop=["\n"]
-            )
-            logger.log(f"Response openAI completion endpoint::::: {response}","0")
-            finalResult=str(response["choices"][0]["text"])
-            logger.log(f"OpenAI completion endpoint finalResult ::::: {finalResult}","0")
+            # response = openai.Completion.create(
+            # model="code-davinci-001",
+            # prompt= openAI_trainingData + insightInput,
+            # temperature=0.25,
+            # max_tokens=198,
+            # top_p=0.5,
+            # frequency_penalty=0,
+            # presence_penalty=0,
+            # stop=["\n"]
+            # )
+
+            # logger.log(f"Response openAI completion endpoint::::: {response}","0")
+            # finalResult=str(response["choices"][0]["text"])
+            # logger.log(f"OpenAI completion endpoint finalResult ::::: {finalResult}","0")
+            # return finalResult
+        
+            logger.log(f"\n\nopenAI_trainingData before conversion :::::: {type(openAI_trainingData)} \n{openAI_trainingData}","0")
+            openAI_trainingData = openAI_trainingData.replace("<insight_input>", insightInput)
+            logger.log(f"\n\nopenAI_trainingData after replacing <insight_input> :::::: \n{openAI_trainingData} \n{type(openAI_trainingData)}","0")
+            messageList = json.loads(openAI_trainingData)
+            logger.log(f"\n\nmessageList after conversion :::::: {messageList} \n{type(messageList)}","0")
+            
+            logger.log(f"\n\nfinal messageList :::::: {messageList}","0")
+
+            response = openai.ChatCompletion.create(
+                                                        model="gpt-3.5-turbo",
+                                                        messages= messageList,
+                                                        temperature=0.25,
+                                                        max_tokens=350,
+                                                        top_p=0.5,
+                                                        frequency_penalty=0,
+                                                        presence_penalty=0,
+                                                        )
+            logger.log(f"\n\nResponse openAI ChatCompletion endpoint::::: {response} \n{type(response)}","0")
+            finalResult=str(response["choices"][0]["message"]["content"])
+            logger.log(f"\n\nOpenAI ChatCompletion endpoint finalResult ::::: {finalResult} \n{type(finalResult)}","0")
             return finalResult
         
         except Exception as e:
             logger.log(f'\n In getCompletionEndpoint exception stacktrace : ', "1")
             trace = traceback.format_exc()
             descr = str(e)
-            returnErr = self.getErrorXml(descr, trace)
+            returnErr = common.getErrorXml(descr, trace)
             logger.log(f'\n Print exception returnSring inside getCompletionEndpoint : {returnErr}', "0")
             return str(returnErr)
 
-    def getErrorXml(self, descr, trace):
-        errorXml = '''<Root>
-                            <Header>
-                                <editFlag>null</editFlag>
-                            </Header>
-                            <Errors>
-                                <error type="E">
-                                    <message><![CDATA['''+descr+''']]></message>
-                                    <trace><![CDATA['''+trace+''']]></trace>
-                                    <type>E</type>
-                                </error>
-                            </Errors>
-                        </Root>'''
-
-        return errorXml
-
+
```

## Comparing `openAIInsight-0.0.4.dist-info/LICENCE.txt` & `openAIInsight-0.0.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.4.dist-info/METADATA` & `openAIInsight-0.0.5.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.4
+Version: 0.0.5
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

