# Comparing `tmp/deklinacija-0.0.2.tar.gz` & `tmp/deklinacija-0.0.3.tar.gz`

## Comparing `deklinacija-0.0.2.tar` & `deklinacija-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/module.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 deklinacija-0.0.2/deklinacija/utils.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-0.0.2/LICENSE
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 deklinacija-0.0.2/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 deklinacija-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/__init__.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/module.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/utils.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 deklinacija-0.0.3/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 deklinacija-0.0.3/PKG-INFO
```

### Comparing `deklinacija-0.0.2/.github/workflows/python-package.yml` & `deklinacija-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.2/deklinacija/module.py` & `deklinacija-0.0.3/deklinacija/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import deklinacija.utils as utils
 
 VOWELS = ["a", "а", "e", "е", "i", "и", "o", "о",
           "u", "у"]  # used for identifying consonants
 
-NEP_A_EXCEPT = ["an", "av", "al", "aš", "ag", "af", "ač"] # words ending with these letters aren't prone to the nepostojano a sound change, the majority of names end like this
+NEP_A = ["ар","ај","ађ"] # words ending with these letters aren't prone to the nepostojano a sound change, the majority of names end like this
 
-PREDNJONEPCANI = ["ј", "љ", "њ", "ђ", "ћ", "ч", "џ", "ш", "ж", "и"] # used for instrumental, letter и added only because of the letter "J" which is added inbetween "i" and "a", like in names "Miki" - "od MikiJa"
+INSTRUMENTAL_LETTERS = ["ј", "љ", "њ", "ђ", "ћ", "ч", "џ", "ш", "ж"]
 SOUND_CHANGE = {"k": "č", "g": "ž", "h": "š", }
 
 
 def genitiv(name, gender, latin=True):
     utils.check(name, gender, latin)
 
     name = list(name.strip())
@@ -67,15 +67,18 @@
                     return "".join(name)
 
             if lastChar not in VOWELS and trdToLastChar not in VOWELS:
                 # nepostojano a
                 if len(name) >= 4:
                     if secToLastChar in ["a", "A"]:
                         # od Stefana, od Miroslava, od Miodraga...
-                        if (secToLastChar.lower() + lastChar.lower()) in NEP_A_EXCEPT:
+                        
+                        lastTwo = name[-2]+name[-1]
+
+                        if utils.toCyrillic(lastTwo) not in NEP_A:
                             if lastChar.isupper():
                                 name.append("A")
                             else:
                                 name.append("a")
                         else:  # od Petra, od Aleksandra...
                             if name[-1].isupper():
                                 name[-2] = name[-1]
@@ -139,27 +142,36 @@
 
     return "".join(name)
 
 
 def instrumental(name, gender, latin=True):
     utils.check(name, gender, latin)
     name = name.strip()
-    nameGenitiv = list(genitiv(name, gender, latin))
-    name = list(name)
+    
     lastChar = name[-1]
     secToLastChar = name[-2]
+    nameGenitiv = utils.separateLetters(genitiv(name, gender, latin))
+    name = list(name)
 
     if latin == True:
         if gender.lower() == "female":
             if lastChar not in VOWELS:
                 return "".join(name)
 
         nameGenitiv.pop(-1)
 
-        if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1] in PREDNJONEPCANI:
+        if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1] in INSTRUMENTAL_LETTERS:
+            if nameGenitiv[-2].lower() == "e":
+                if lastChar.isupper():
+                    nameGenitiv.append("OM")
+                    return "".join(nameGenitiv)
+                else:
+                    nameGenitiv.append("om")
+                    return "".join(nameGenitiv)
+
             if lastChar.isupper():
                 nameGenitiv.append("EM")
                 return "".join(nameGenitiv)
             else:
                 nameGenitiv.append("em")
                 return "".join(nameGenitiv)
```

### Comparing `deklinacija-0.0.2/deklinacija/utils.py` & `deklinacija-0.0.3/deklinacija/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 alphabet = {
     'a': 'а', 'b': 'б', 'c': 'ц', 'č': 'ч', 'ć': 'ћ', 'd': 'д', 'đ': 'ђ', 'dj': 'ђ', 'e': 'е', 'f': 'ф', 'g': 'г',
     'h': 'х', 'i': 'и', 'j': 'ј', 'k': 'к', 'l': 'л', 'lj': 'љ', 'm': 'м', 'n': 'н', 'nj': 'њ', 'o': 'о',
     'p': 'п', 'r': 'р', 's': 'с', 'š': 'ш', 't': 'т', 'u': 'у', 'v': 'в', 'z': 'з', 'ž': 'ж', 'dž': 'џ', 'dz': 'џ'}
 
+alphabet_latin = {
+    'а': 'a', 'б': 'b', 'ц': 'c', 'ч': 'č', 'ћ': 'ć', 'д': 'd', 'ђ': 'đ', 'е': 'e', 'ф': 'f', 'г': 'g',
+    'х': 'h', 'и': 'i', 'ј': 'j', 'к': 'k', 'л': 'l', 'љ': 'lj', 'м': 'm', 'н': 'n', 'њ': 'nj', 'о': 'o',
+    'п': 'p', 'р': 'r', 'с': 's', 'ш': 'š', 'т': 't', 'у': 'u', 'в': 'v', 'з': 'z', 'ж': 'ž', 'џ': 'dž'}
+
 latExceptions = []
 
 def toCyrillic(word):
 
     wordArray = []
     word = list(word)
     wordText = "".join(word)
@@ -55,20 +60,67 @@
             wordArray[n] = i
             n += 1
 
     word = "".join(wordArray)
 
     return word
 
+def toLatin(word):
+    word = list(word)
+
+    n = 0
+    for i in word:
+        if i.lower() in alphabet_latin:
+            if i[0].isupper() and i.lower() in ['љ','њ','џ']:
+                letter = alphabet_latin[i.lower()][0].upper() + alphabet_latin[i.lower()][1]
+                word[n] = letter
+            elif i[0].isupper():
+                word[n] = alphabet_latin[i.lower()].upper()
+            else:
+                word[n] = alphabet_latin[i]
+
+        else:
+            word[n] = i
+        n += 1
+    
+    return "".join(word)
+
 def check(name,gender,latin):
     if type(name) != str or type(name) != str or type(gender) != str or type(latin) != bool:
         raise TypeError("name and gender params must be a string, param latin must be a boolean")
     
     gender = gender.strip()
     name = name.strip()
 
     if gender.lower() not in ["male","female"]:
         raise ValueError('gender param must be either "male" or "female"')
 
     if len(name) < 3:
         raise ValueError("name param must be at least 3 characters long")
     
+def separateLetters(word):
+    word = list(word)
+    wordText = "".join(word)
+    wordArray = []
+    
+
+    n = 0
+    while n <= (len(word)-1):
+
+        if n == len(word)-1:
+            wordArray.append(word[n])
+            break
+
+        if word[n] in ["d", "D", "l", "L", "n", "N"] and word[n+1] in ["j", "J"]:
+            wordArray.append(word[n]+word[n+1])
+            word.pop(n+1)
+            n += 1
+        elif word[n] in ["d", "D"] and word[n+1] in ["ž", "Ž", "z", "Z"]:
+            wordArray.append(word[n]+word[n+1])
+            word.pop(n+1)
+            n += 1
+        else:
+            wordArray.append(word[n])
+            n += 1
+    
+    return wordArray
+
```

### Comparing `deklinacija-0.0.2/LICENSE` & `deklinacija-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.2/README.md` & `deklinacija-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.2/pyproject.toml` & `deklinacija-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-0.0.2/PKG-INFO` & `deklinacija-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

