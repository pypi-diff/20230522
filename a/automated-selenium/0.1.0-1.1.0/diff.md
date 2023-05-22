# Comparing `tmp/automated_selenium-0.1.0.tar.gz` & `tmp/automated_selenium-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automated_selenium-0.1.0.tar", max compression
+gzip compressed data, was "automated_selenium-1.1.0.tar", max compression
```

## Comparing `automated_selenium-0.1.0.tar` & `automated_selenium-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      105 2023-05-22 10:08:25.407552 automated_selenium-0.1.0/automated_selenium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-0.1.0/automated_selenium/drivers/__init__.py
--rw-r--r--   0        0        0     1004 2023-05-22 10:05:20.557927 automated_selenium-0.1.0/automated_selenium/drivers/undetected_driver.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-0.1.0/automated_selenium/pages/__init__.py
--rw-r--r--   0        0        0    15364 2023-05-22 10:39:50.355985 automated_selenium-0.1.0/automated_selenium/pages/base_page.py
--rw-r--r--   0        0        0     1175 2023-05-22 10:40:23.715165 automated_selenium-0.1.0/automated_selenium/resources/resources.py
--rw-r--r--   0        0        0     1121 2023-05-22 10:02:06.511333 automated_selenium-0.1.0/LICENSE
--rw-r--r--   0        0        0      644 2023-05-22 10:48:33.020147 automated_selenium-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3722 2023-05-22 10:00:47.380924 automated_selenium-0.1.0/README.md
--rw-r--r--   0        0        0     4511 1970-01-01 00:00:00.000000 automated_selenium-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-22 11:20:22.645610 automated_selenium-1.1.0/automated_selenium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.0/automated_selenium/drivers/__init__.py
+-rw-r--r--   0        0        0     1009 2023-05-22 11:20:41.941751 automated_selenium-1.1.0/automated_selenium/drivers/undetected_driver.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:02:49.528226 automated_selenium-1.1.0/automated_selenium/pages/__init__.py
+-rw-r--r--   0        0        0    15383 2023-05-22 11:21:18.542924 automated_selenium-1.1.0/automated_selenium/pages/base_page.py
+-rw-r--r--   0        0        0     1175 2023-05-22 10:40:23.715165 automated_selenium-1.1.0/automated_selenium/resources/resources.py
+-rw-r--r--   0        0        0     1121 2023-05-22 10:02:06.511333 automated_selenium-1.1.0/LICENSE
+-rw-r--r--   0        0        0      667 2023-05-22 12:08:15.790370 automated_selenium-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9041 2023-05-22 12:03:21.271803 automated_selenium-1.1.0/README.md
+-rw-r--r--   0        0        0     9766 1970-01-01 00:00:00.000000 automated_selenium-1.1.0/PKG-INFO
```

### Comparing `automated_selenium-0.1.0/automated_selenium/drivers/undetected_driver.py` & `automated_selenium-1.1.0/automated_selenium/drivers/undetected_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This file contains all the logic of how the driver or browser will react
 """
 import undetected_chromedriver as uc
 from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
 
 
-def get_undetected_chrome_browser(profile):
+def get_undetected_chrome_browser(profile=None):
     """Returns an instance of an undetected Chrome browser with added features to make it more undetectable and secure.
     The browser will save the profile and cookies to the specified folder so that you don't have to log in every time.
 
     Returns:
         uc.Chrome: An instance of the Chrome class from the undetected_chromedriver library.
     """
     if profile:
```

### Comparing `automated_selenium-0.1.0/automated_selenium/pages/base_page.py` & `automated_selenium-1.1.0/automated_selenium/pages/base_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from selenium.webdriver import Remote
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
-from resources.resources import CookieBotResources, Selector
+from automated_selenium.resources.resources import CookieBotResources, Selector
 
 
 class BasePage:
     """Base class for all the pages
     the subclasses will contain all the methods can be perform on a
     single page
```

### Comparing `automated_selenium-0.1.0/automated_selenium/resources/resources.py` & `automated_selenium-1.1.0/automated_selenium/resources/resources.py`

 * *Files identical despite different names*

### Comparing `automated_selenium-0.1.0/LICENSE` & `automated_selenium-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automated_selenium-0.1.0/pyproject.toml` & `automated_selenium-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "automated-selenium"
-version = "0.1.0"
+version = "1.1.0"
 description = "Automated-Selenium is a Python library that provides a base page class designed to facilitate the implementation of the Page Object Model (POM) structure in Selenium-based test automation projects."
 authors = ["Waqar Khan <waqarkhan1252617@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "automated_selenium"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 selenium = "^4.9.1"
 webdriver-manager = "^3.8.6"
 undetected-chromedriver = "^3.4.7"
+pyautogui = "^0.9.53"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

