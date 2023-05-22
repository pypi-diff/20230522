# Comparing `tmp/Swapsies-1.8.tar.gz` & `tmp/Swapsies-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Swapsies-1.8.tar", last modified: Mon May 18 08:12:59 2020, max compression
+gzip compressed data, was "dist/Swapsies-1.9.tar", last modified: Tue May 26 03:32:14 2020, max compression
```

## Comparing `Swapsies-1.8.tar` & `Swapsies-1.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-18 08:12:59.972246 Swapsies-1.8/
--rw-r--r--   0 dave       (502) staff       (20)      489 2020-05-18 08:12:59.972481 Swapsies-1.8/PKG-INFO
--rw-r--r--   0 dave       (502) staff       (20)      136 2020-04-16 02:31:15.000000 Swapsies-1.8/README.md
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-18 08:12:59.958389 Swapsies-1.8/Swapsies/
--rwxr-xr-x   0 dave       (502) staff       (20)   146424 2020-04-14 11:44:28.000000 Swapsies-1.8/Swapsies/CloudOutlinerXSD.py
--rwxr-xr-x   0 dave       (502) staff       (20)   146424 2020-04-14 11:44:28.000000 Swapsies-1.8/Swapsies/OutlineXSD.py
--rw-r--r--   0 dave       (502) staff       (20)        0 2020-04-16 02:31:15.000000 Swapsies-1.8/Swapsies/__init__.py
--rwxr-xr-x   0 dave       (502) staff       (20)     1713 2020-04-14 11:44:28.000000 Swapsies-1.8/Swapsies/cdata.py
--rwxr-xr-x   0 dave       (502) staff       (20)    24330 2020-04-14 11:44:28.000000 Swapsies-1.8/Swapsies/xmi.py
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-18 08:12:59.961892 Swapsies-1.8/Swapsies.egg-info/
--rw-r--r--   0 dave       (502) staff       (20)      489 2020-05-18 08:12:57.000000 Swapsies-1.8/Swapsies.egg-info/PKG-INFO
--rw-r--r--   0 dave       (502) staff       (20)      520 2020-05-18 08:12:58.000000 Swapsies-1.8/Swapsies.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (502) staff       (20)        1 2020-05-18 08:12:57.000000 Swapsies-1.8/Swapsies.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (502) staff       (20)       94 2020-05-18 08:12:57.000000 Swapsies-1.8/Swapsies.egg-info/requires.txt
--rw-r--r--   0 dave       (502) staff       (20)        9 2020-05-18 08:12:57.000000 Swapsies-1.8/Swapsies.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-18 08:12:59.971600 Swapsies-1.8/bin/
--rw-r--r--   0 dave       (502) staff       (20)        0 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/.gitignore
--rwxr-xr-x   0 dave       (502) staff       (20)    10788 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/COD.py
--rwxr-xr-x   0 dave       (502) staff       (20)    10552 2020-05-18 08:11:19.000000 Swapsies-1.8/bin/OPML.py
--rwxr-xr-x   0 dave       (502) staff       (20)     1201 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/cdata2xml.py
--rwxr-xr-x   0 dave       (502) staff       (20)     3250 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/contact2vcard.py
--rwxr-xr-x   0 dave       (502) staff       (20)     2649 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/email2vcard.py
--rwxr-xr-x   0 dave       (502) staff       (20)      650 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/outlines.py
--rwxr-xr-x   0 dave       (502) staff       (20)      231 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/pdf2text.py
--rwxr-xr-x   0 dave       (502) staff       (20)     3646 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/text2opml.py
--rwxr-xr-x   0 dave       (502) staff       (20)     3385 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/tree2xmi.py
--rwxr-xr-x   0 dave       (502) staff       (20)     2952 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/wsdl2file.py
--rwxr-xr-x   0 dave       (502) staff       (20)     7457 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/xls2dict.py
--rwxr-xr-x   0 dave       (502) staff       (20)     2676 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/xls2opml.py
--rwxr-xr-x   0 dave       (502) staff       (20)      107 2020-04-14 11:44:28.000000 Swapsies-1.8/bin/xml2cdata.py
--rw-r--r--   0 dave       (502) staff       (20)       79 2020-05-18 08:12:59.973257 Swapsies-1.8/setup.cfg
--rwxr-xr-x   0 dave       (502) staff       (20)     1079 2020-05-18 07:54:05.000000 Swapsies-1.8/setup.py
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-26 03:32:14.015676 Swapsies-1.9/
+-rw-r--r--   0 dave       (502) staff       (20)      489 2020-05-26 03:32:14.015868 Swapsies-1.9/PKG-INFO
+-rw-r--r--   0 dave       (502) staff       (20)      136 2020-04-16 02:31:15.000000 Swapsies-1.9/README.md
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-26 03:32:13.425117 Swapsies-1.9/Swapsies/
+-rw-r--r--   0 dave       (502) staff       (20)   114549 2020-05-26 03:31:45.000000 Swapsies-1.9/Swapsies/CloudOutlinerXSD.py
+-rw-r--r--   0 dave       (502) staff       (20)    50763 2020-05-26 03:31:45.000000 Swapsies-1.9/Swapsies/OutlineXSD.py
+-rw-r--r--   0 dave       (502) staff       (20)        0 2020-04-16 02:31:15.000000 Swapsies-1.9/Swapsies/__init__.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1713 2020-04-14 11:44:28.000000 Swapsies-1.9/Swapsies/cdata.py
+-rwxr-xr-x   0 dave       (502) staff       (20)    24330 2020-04-14 11:44:28.000000 Swapsies-1.9/Swapsies/xmi.py
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-26 03:32:13.428038 Swapsies-1.9/Swapsies.egg-info/
+-rw-r--r--   0 dave       (502) staff       (20)      489 2020-05-26 03:32:12.000000 Swapsies-1.9/Swapsies.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (502) staff       (20)      536 2020-05-26 03:32:13.000000 Swapsies-1.9/Swapsies.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (502) staff       (20)        1 2020-05-26 03:32:12.000000 Swapsies-1.9/Swapsies.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (502) staff       (20)       94 2020-05-26 03:32:13.000000 Swapsies-1.9/Swapsies.egg-info/requires.txt
+-rw-r--r--   0 dave       (502) staff       (20)        9 2020-05-26 03:32:13.000000 Swapsies-1.9/Swapsies.egg-info/top_level.txt
+drwxr-xr-x   0 dave       (502) staff       (20)        0 2020-05-26 03:32:14.015037 Swapsies-1.9/bin/
+-rw-r--r--   0 dave       (502) staff       (20)        0 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/.gitignore
+-rwxr-xr-x   0 dave       (502) staff       (20)    10788 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/COD.py
+-rwxr-xr-x   0 dave       (502) staff       (20)    10255 2020-05-26 03:31:45.000000 Swapsies-1.9/bin/OPML.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1201 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/cdata2xml.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     3250 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/contact2vcard.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     2649 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/email2vcard.py
+-rwxr-xr-x   0 dave       (502) staff       (20)      650 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/outlines.py
+-rwxr-xr-x   0 dave       (502) staff       (20)      231 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/pdf2text.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     1488 2020-05-26 03:31:45.000000 Swapsies-1.9/bin/ref2type.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     3646 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/text2opml.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     3385 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/tree2xmi.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     2952 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/wsdl2file.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     7457 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/xls2dict.py
+-rwxr-xr-x   0 dave       (502) staff       (20)     2676 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/xls2opml.py
+-rwxr-xr-x   0 dave       (502) staff       (20)      107 2020-04-14 11:44:28.000000 Swapsies-1.9/bin/xml2cdata.py
+-rw-r--r--   0 dave       (502) staff       (20)       79 2020-05-26 03:32:14.016610 Swapsies-1.9/setup.cfg
+-rwxr-xr-x   0 dave       (502) staff       (20)     1100 2020-05-26 03:31:45.000000 Swapsies-1.9/setup.py
```

### Comparing `Swapsies-1.8/Swapsies/cdata.py` & `Swapsies-1.9/Swapsies/cdata.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/Swapsies/xmi.py` & `Swapsies-1.9/Swapsies/xmi.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/COD.py` & `Swapsies-1.9/bin/COD.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/OPML.py` & `Swapsies-1.9/bin/OPML.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
 	#.............................................................
 	def _createOPML(self, title):
 		opml = OrderedDict([
 			('opml', OrderedDict([
 				('@version', '1.0'),
 				('head', OrderedDict([
-					('title', title),
+					('title', title.replace('&','and')),
 				])),
 				('body', OrderedDict([
 				])) 
 			]))
 		])
 		return opml
 	
@@ -252,14 +252,18 @@
 		body = opml['opml']['body']
 		body['outline'] = []
 
 		for comment in getElements(doc.ctx, '//w:comment'):
 			print(comment.content)
 			body['outline'].append({
 				'@text': comment.content,
+				'@_note': '%s %s'%(
+					getAttribute(comment, 'date').replace('T',' ').replace('Z',''),
+					getAttribute(comment, 'author')
+				),
 			})					
 
 		name = os.path.join(os.path.dirname(path), 'comments.opml')
 		with open(name, 'w') as output:
 			xmltodict.unparse(opml, output, encoding='UTF8', pretty=True)
 		print(name)			
 
@@ -274,100 +278,80 @@
 
 		path =os.path.expanduser(file)
 		doc = Document(path)
 
 		opml = self._createOPML(file)
 		
 		body = opml['opml']['body']
-		# stack[-1] is the current parent
+		body['outline'] = []
 		stack = [ body ]
-
-		patterns = [
-			'Norm', 
-			'Body',
-			'List',
-		]
+		level = 0
+		
 		highlites = { 
 			1: colours.Green, 
 			2: colours.Blue, 
 			3: colours.White 
 		}
 
 		for paragraph in doc.paragraphs:
 			ps = paragraph.style
 			text = paragraph.text.strip().replace('\t',' ').replace('\n',' ')
-
-			if len(text) == 0: continue
-			
-			if any(map(lambda x: ps.name.startswith(x), patterns)):
-				#sys.stdout.write('%s   "%s\n"'%('  '*(level-1), text))
-
-				if not 'outline' in stack[-1].keys():
-					stack[-1]['outline'] = [{
-						'@text': text,
-					}]
-				parent = stack[-1]['outline'][-1]
-				
-				if '@_note' not in parent.keys():
-					parent['@_note'] = ''
-
-				if note:
-					lines = list(filter(lambda x: len(x), parent['@_note'].split('\n')))
-					lines.append(text)
-					parent['@_note'] = '\n'.join(lines)
-				else: 
-					outline = {
-						'@text': text,
-					}
-					if 'outline' not in parent.keys():
-						parent['outline'] = []
-					parent['outline'].append(outline)
-					
+			if len(text) == 0:
 				continue
-			
-			if not ps.name.startswith('Heading'):
-				sys.stderr.write(colours.Red)
-				sys.stderr.write('%s\n'%ps.name)
-				sys.stderr.write(colours.Off)
-				continue
-
-			heading = ps.name.replace('Heading ','').split(' ')[0]
-			level=int(heading)
 
-			if level in highlites.keys():
-				sys.stdout.write(highlites[level])
+			parent = stack[-1]
 
-			sys.stdout.write('%s %s\n'%('  '*(level-1), text))
+			if ps.name.startswith('Heading'):
+				heading = ps.name.replace('Heading ','').split(' ')[0]
+				level=int(heading)
+
+				if level in highlites.keys():
+					sys.stdout.write(highlites[level])
+				sys.stdout.write('%s%s\n'%('  '*(level-1), text))
+
+				if level < len(stack):
+					parent = stack.pop()
+				if level > len(stack):
+					parent['outline'] = []
+					stack.append(parent)
+					parent = stack[-1]
+					
+				parent['@text'] = text
 
+			else:
+				sys.stdout.write('%s%s\n'%('  '*(level), text))
+				
+				
 			sys.stdout.write(colours.Off)
 
-			outline = {
-				'@text': text,
-			}
-
-			if level > len(stack):
-				parent = stack[-1]['outline'][-1]
-				stack.append(parent)
-
-			if level < len(stack):
-				stack.pop()
-				
-			if 'outline' not in stack[-1].keys():
-				stack[-1]['outline'] = []
-			stack[-1]['outline'].append(outline)				
+			if 'outline' not in parent.keys():
+				parent['outline'] = []
+			if '@_note' not in parent.keys():
+				parent['@_note'] = ''
+
+			if note:
+				lines = list(filter(lambda x: len(x), parent['@_note'].split('\n')))
+				lines.append(text)
+				parent['@_note'] = '\n'.join(lines)
+			else: 
+				parent['outline'].append({
+					'@text': text,
+				})
+					
 		
 		name = os.path.join(os.path.dirname(path), 'outline.opml')
 		with open(name, 'w') as output:
 			xmltodict.unparse(opml, output, encoding='UTF8', pretty=True)
 		print(name)
-		
-		name = os.path.join(os.path.dirname(path), 'outline.json')
-		with open(name, 'w') as output:
-			json.dump(opml, output, indent=4)
-		print(name)
+
+		if False:
+			name = os.path.join(os.path.dirname(path), 'outline.json')
+			with open(name, 'w') as output:
+				json.dump(opml, output, indent=4)
+			print(name)
 
 		
 	#.............................................................
 	@args.operation
 	def docxIndented2opml(self, file):
 		if not file.endswith('docx'):
 			sys.stderr.write('not a docx file\n')
@@ -414,15 +398,17 @@
 
 			
 		name = os.path.join(os.path.dirname(path), 'outline.opml')
 		with open(name,'w') as output:
 			xmltodict.unparse(opml, output)
 		print(name)
 
-		name = os.path.join(os.path.dirname(path), 'outline.json')
-		with open(name,'w') as output:
-			json.dump(opml, output, indent=4)
+		if False:
+			name = os.path.join(os.path.dirname(path), 'outline.json')
+			with open(name,'w') as output:
+				json.dump(opml, output, indent=4)
+			print(name)
 
 
 #_________________________________________________________________
 if __name__ == '__main__': args.execute()
```

### Comparing `Swapsies-1.8/bin/cdata2xml.py` & `Swapsies-1.9/bin/cdata2xml.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/contact2vcard.py` & `Swapsies-1.9/bin/contact2vcard.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/email2vcard.py` & `Swapsies-1.9/bin/email2vcard.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/outlines.py` & `Swapsies-1.9/bin/outlines.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/text2opml.py` & `Swapsies-1.9/bin/text2opml.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/tree2xmi.py` & `Swapsies-1.9/bin/tree2xmi.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/wsdl2file.py` & `Swapsies-1.9/bin/wsdl2file.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/xls2dict.py` & `Swapsies-1.9/bin/xls2dict.py`

 * *Files identical despite different names*

### Comparing `Swapsies-1.8/bin/xls2opml.py` & `Swapsies-1.9/bin/xls2opml.py`

 * *Files identical despite different names*

