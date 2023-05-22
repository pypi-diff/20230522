# Comparing `tmp/selenium-recaptcha-solver-1.8.0.tar.gz` & `tmp/selenium-recaptcha-solver-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-recaptcha-solver-1.8.0.tar", last modified: Wed May  3 07:26:43 2023, max compression
+gzip compressed data, was "selenium-recaptcha-solver-1.8.1.tar", last modified: Mon May 22 08:13:23 2023, max compression
```

## Comparing `selenium-recaptcha-solver-1.8.0.tar` & `selenium-recaptcha-solver-1.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.464227 selenium-recaptcha-solver-1.8.0/
--rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     3280 2023-05-03 07:26:43.463225 selenium-recaptcha-solver-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2023-05-03 07:15:11.000000 selenium-recaptcha-solver-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.457989 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/
--rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/__init__.py
--rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/delay_config.py
--rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/exceptions.py
--rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/services.py
--rw-rw-rw-   0        0        0     8881 2023-05-03 07:23:51.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/solver.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:26:43.462226 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/
--rw-rw-rw-   0        0        0     3280 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 07:26:43.000000 selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 07:26:43.464227 selenium-recaptcha-solver-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-05-03 07:26:38.000000 selenium-recaptcha-solver-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:13:23.747007 selenium-recaptcha-solver-1.8.1/
+-rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     3375 2023-05-22 08:13:23.747007 selenium-recaptcha-solver-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2949 2023-05-22 08:12:23.000000 selenium-recaptcha-solver-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:13:23.741498 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/
+-rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/delay_config.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/exceptions.py
+-rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/services.py
+-rw-rw-rw-   0        0        0     8881 2023-05-19 09:58:12.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/solver.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:13:23.747007 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/
+-rw-rw-rw-   0        0        0     3375 2023-05-22 08:13:23.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-22 08:13:23.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:13:23.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-22 08:13:23.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-22 08:13:23.000000 selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:13:23.747007 selenium-recaptcha-solver-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-05-22 08:11:12.000000 selenium-recaptcha-solver-1.8.1/setup.py
```

### Comparing `selenium-recaptcha-solver-1.8.0/LICENSE` & `selenium-recaptcha-solver-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.0/PKG-INFO` & `selenium-recaptcha-solver-1.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.0
+Version: 1.8.1
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
@@ -49,15 +49,15 @@
 from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
 options = Options()
 
-options.add_argument("--headless")
+options.add_argument("--headless")  # Remove this if you want to see the browser (Headless makes the chromedriver not have a GUI)
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
```

### Comparing `selenium-recaptcha-solver-1.8.0/README.md` & `selenium-recaptcha-solver-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
 options = Options()
 
-options.add_argument("--headless")
+options.add_argument("--headless")  # Remove this if you want to see the browser (Headless makes the chromedriver not have a GUI)
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
```

### Comparing `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/delay_config.py` & `selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/delay_config.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/services.py` & `selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/services.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver/solver.py` & `selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver/solver.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,20 +66,20 @@
             by='id',
             locator='recaptcha-anchor',
             timeout=150,
         )
 
         self._js_click(checkbox)
 
-        if self._delay_config:
-            self._delay_config.delay_after_click_checkbox()
-
         if checkbox.get_attribute('aria-checked') == 'true':
             return
 
+        if self._delay_config:
+            self._delay_config.delay_after_click_checkbox()
+
         self._driver.switch_to.parent_frame()
 
         captcha_challenge = self._wait_for_element(
             by=By.CSS_SELECTOR,
             locator='iframe[src*="www.google.com/recaptcha/api2/bframe"]',
             timeout=5,
         )
```

### Comparing `selenium-recaptcha-solver-1.8.0/selenium_recaptcha_solver.egg-info/PKG-INFO` & `selenium-recaptcha-solver-1.8.1/selenium_recaptcha_solver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.8.0
+Version: 1.8.1
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
@@ -49,15 +49,15 @@
 from selenium.webdriver.chrome.options import Options
 
 
 test_ua = 'Mozilla/5.0 (Windows NT 4.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/37.0.2049.0 Safari/537.36'
 
 options = Options()
 
-options.add_argument("--headless")
+options.add_argument("--headless")  # Remove this if you want to see the browser (Headless makes the chromedriver not have a GUI)
 options.add_argument("--window-size=1920,1080")
 
 options.add_argument(f'--user-agent={test_ua}')
 
 options.add_argument('--no-sandbox')
 options.add_argument("--disable-extensions")
```

### Comparing `selenium-recaptcha-solver-1.8.0/setup.py` & `selenium-recaptcha-solver-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='selenium-recaptcha-solver',
-    version='1.8.0',
+    version='1.8.1',
     license='MIT',
     author='Tomás Perestrelo',
     author_email='tomasperestrelo21@gmail.com',
     packages=find_packages(exclude=('tests*', 'testing*')),
     url='https://github.com/thicccat688/selenium-recaptcha-solver',
     download_url='https://pypi.org/project/selenium-recaptcha-solver',
     keywords='python, captcha, speech recognition, selenium, web automation',
```

