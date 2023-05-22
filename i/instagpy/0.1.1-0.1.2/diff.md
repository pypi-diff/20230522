# Comparing `tmp/instagpy-0.1.1.tar.gz` & `tmp/instagpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.1.tar", last modified: Sat May 20 10:01:41 2023, max compression
+gzip compressed data, was "instagpy-0.1.2.tar", last modified: Mon May 22 12:25:42 2023, max compression
```

## Comparing `instagpy-0.1.1.tar` & `instagpy-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 10:01:41.027227 instagpy-0.1.1/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3304 2023-05-20 10:01:41.027227 instagpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2242 2023-05-20 07:58:43.000000 instagpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 10:01:41.011564 instagpy-0.1.1/instagpy/
--rw-rw-rw-   0        0        0       32 2023-05-20 05:51:40.000000 instagpy-0.1.1/instagpy/__init__.py
--rw-rw-rw-   0        0        0    19438 2023-05-20 10:00:36.000000 instagpy-0.1.1/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     1821 2023-05-19 17:39:41.000000 instagpy-0.1.1/instagpy/path.py
--rw-rw-rw-   0        0        0     1014 2023-05-19 17:37:45.000000 instagpy-0.1.1/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2512 2023-05-20 05:51:32.000000 instagpy-0.1.1/instagpy/session_util.py
--rw-rw-rw-   0        0        0      723 2023-05-19 13:24:18.000000 instagpy-0.1.1/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 10:01:41.011564 instagpy-0.1.1/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3304 2023-05-20 10:01:40.000000 instagpy-0.1.1/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-20 10:01:40.000000 instagpy-0.1.1/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 10:01:40.000000 instagpy-0.1.1/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-20 10:01:40.000000 instagpy-0.1.1/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 10:01:40.000000 instagpy-0.1.1/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 10:01:41.027227 instagpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-20 09:54:21.000000 instagpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.034289 instagpy-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3318 2023-05-22 12:25:42.034289 instagpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.023415 instagpy-0.1.2/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-05-20 05:51:40.000000 instagpy-0.1.2/instagpy/__init__.py
+-rw-rw-rw-   0        0        0    20519 2023-05-22 12:17:53.000000 instagpy-0.1.2/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2019 2023-05-22 09:57:02.000000 instagpy-0.1.2/instagpy/path.py
+-rw-rw-rw-   0        0        0     1014 2023-05-19 17:37:45.000000 instagpy-0.1.2/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2512 2023-05-20 05:51:32.000000 instagpy-0.1.2/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 12:05:19.000000 instagpy-0.1.2/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.034289 instagpy-0.1.2/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 12:25:42.034289 instagpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-05-22 12:25:08.000000 instagpy-0.1.2/setup.py
```

### Comparing `instagpy-0.1.1/LICENSE` & `instagpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.1/PKG-INFO` & `instagpy-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
@@ -60,15 +60,15 @@
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
 insta = InstaGPy()
 
-print(insta.get_user_basic_details('champagnepapi'))
+insta.get_user_basic_details('champagnepapi',print_formatted=True)
 
 ```
 
 ## Documentation
 
 Check out step by step guide.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.1 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.2 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -25,16 +25,17 @@
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
     from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
         use_mutiple_account=False, session_ids=None, min_requests=None,
     max_requests=None) ``` > ### Example - Get Basic User Details of a User
-       ```python from instagpy import InstaGPy insta = InstaGPy() print
-(insta.get_user_basic_details('champagnepapi')) ``` ## Documentation Check out
-   step by step guide. [Documentation](instagpy/docs/docs.md) ## Features -
-   Extracts User's Followers - Extracts User's Followings - Extracts User's
-Profile Details along with Contact Details (Phone, WhatsApp, Email & Address) -
-   Extracts Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+          ```python from instagpy import InstaGPy insta = InstaGPy()
+   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
+  Documentation Check out step by step guide. [Documentation](instagpy/docs/
+docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
+ Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
+       Email & Address) - Extracts Instagram Profile Media ## Authors -
+ [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
+   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
+   contact me on Social Media @iSarabjitDhiman ## Support For support, email
+                           hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.1/README.md` & `instagpy-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
 insta = InstaGPy()
 
-print(insta.get_user_basic_details('champagnepapi'))
+insta.get_user_basic_details('champagnepapi',print_formatted=True)
 
 ```
 
 ## Documentation
 
 Check out step by step guide.
```

#### html2text {}

```diff
@@ -10,16 +10,17 @@
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
     from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
         use_mutiple_account=False, session_ids=None, min_requests=None,
     max_requests=None) ``` > ### Example - Get Basic User Details of a User
-       ```python from instagpy import InstaGPy insta = InstaGPy() print
-(insta.get_user_basic_details('champagnepapi')) ``` ## Documentation Check out
-   step by step guide. [Documentation](instagpy/docs/docs.md) ## Features -
-   Extracts User's Followers - Extracts User's Followings - Extracts User's
-Profile Details along with Contact Details (Phone, WhatsApp, Email & Address) -
-   Extracts Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+          ```python from instagpy import InstaGPy insta = InstaGPy()
+   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
+  Documentation Check out step by step guide. [Documentation](instagpy/docs/
+docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
+ Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
+       Email & Address) - Extracts Instagram Profile Media ## Authors -
+ [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
+   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
+   contact me on Social Media @iSarabjitDhiman ## Support For support, email
+                           hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.1/instagpy/instagpy.py` & `instagpy-0.1.2/instagpy/instagpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -417,10 +417,31 @@
                 return response['data']['shortcode_media']['display_resources'][-1]['src']
             if media_type == "GraphVideo":
                 return response['data']['shortcode_media']['video_url']
             if media_type == "GraphSidecar":
                 return [each_carousel['node']['display_resources'][-1]['src'] for each_carousel in response['data']['shortcode_media']['edge_sidecar_to_children']["edges"]]
         return None
 
+    def get_about_user(self, username, print_formatted=True):
+        """Returns user about details like account location, if running any ads, verified, Joining Date, Verification Date.
+
+        Args:
+            username (str): Username of the person
+            print_formatted (bool, optional): Returns only necessary and structure data if set to True Else would return the whole dataset. Defaults to True.
+
+        Returns:
+            dict: User About Dataset.
+        """
+        if not self.logged_in():
+            self.login()
+        user_id = self.get_user_id(username)
+        data = {'referer_type': 'ProfileUsername', 'target_user_id': user_id, 'bk_client_context': {
+            'bloks_version': about_user_query, 'style_id': 'instagram'}, 'bloks_versioning_id': about_user_query}
+        response = make_request(about_user_url, method='POST', data=data,
+                                session=self.session, max_retries=self.max_retries)
+        if print_formatted:
+            return utils.format_about_data(response)
+        return response
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `instagpy-0.1.1/instagpy/path.py` & `instagpy-0.1.2/instagpy/path.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,10 +28,13 @@
 # return 50 at a time
 post_details_query = "9f8827793ef34641b2fb195d4d41151c"
 user_feed_query = "69cba40317214236af40e7efa697781d"
 # followers_list_query & following_list_query - both return max 50 results in a single request but work with blue tick verified accounts.
 followers_list_query = "7dd9a7e2160524fd85f50317462cff9f"
 following_list_query = "c56ee0ae1f89cdbd1c89e2bc6b8f3d18"
 
+about_user_url = "https://i.instagram.com/api/v1/bloks/apps/com.instagram.interactions.about_this_account/"
+about_user_query = "8ca96ca267e30c02cf90888d91eeff09627f0e3fd2bd9df472278c9a6c022cbb"
+
 
 if __name__ == '__main__':
     pass
```

### Comparing `instagpy-0.1.1/instagpy/request_util.py` & `instagpy-0.1.2/instagpy/request_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.1/instagpy/session_util.py` & `instagpy-0.1.2/instagpy/session_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.1/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.2/instagpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
@@ -60,15 +60,15 @@
 > ### Example - Get Basic User Details of a User
 
 ```python
 from instagpy import InstaGPy
 
 insta = InstaGPy()
 
-print(insta.get_user_basic_details('champagnepapi'))
+insta.get_user_basic_details('champagnepapi',print_formatted=True)
 
 ```
 
 ## Documentation
 
 Check out step by step guide.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.1 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.2 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
@@ -25,16 +25,17 @@
  extracting data at scale/in bulk. If possible, use multiple accounts to fetch
      data from Instagram.` **_DON'T USE YOUR PERSONAL ACCOUNT FOR SCRAPING
  PURPOSES._** ## Installation Install InstaGPy with pip ```python pip install
 instagpy ``` ## Usage/Examples ```python python quickstart.py ``` OR ```python
     from instagpy import InstaGPy InstaGPy(proxies=proxies, max_retries=3,
         use_mutiple_account=False, session_ids=None, min_requests=None,
     max_requests=None) ``` > ### Example - Get Basic User Details of a User
-       ```python from instagpy import InstaGPy insta = InstaGPy() print
-(insta.get_user_basic_details('champagnepapi')) ``` ## Documentation Check out
-   step by step guide. [Documentation](instagpy/docs/docs.md) ## Features -
-   Extracts User's Followers - Extracts User's Followings - Extracts User's
-Profile Details along with Contact Details (Phone, WhatsApp, Email & Address) -
-   Extracts Instagram Profile Media ## Authors - [@iSarabjitDhiman](https://
- www.github.com/iSarabjitDhiman) ## Feedback If you have any feedback, please
-   reach out to us at hello@sarabjitdhiman.com or contact me on Social Media
-   @iSarabjitDhiman ## Support For support, email hello@sarabjitdhiman.com
+          ```python from instagpy import InstaGPy insta = InstaGPy()
+   insta.get_user_basic_details('champagnepapi',print_formatted=True) ``` ##
+  Documentation Check out step by step guide. [Documentation](instagpy/docs/
+docs.md) ## Features - Extracts User's Followers - Extracts User's Followings -
+ Extracts User's Profile Details along with Contact Details (Phone, WhatsApp,
+       Email & Address) - Extracts Instagram Profile Media ## Authors -
+ [@iSarabjitDhiman](https://www.github.com/iSarabjitDhiman) ## Feedback If you
+   have any feedback, please reach out to us at hello@sarabjitdhiman.com or
+   contact me on Social Media @iSarabjitDhiman ## Support For support, email
+                           hello@sarabjitdhiman.com
```

### Comparing `instagpy-0.1.1/setup.py` & `instagpy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

