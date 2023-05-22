# Comparing `tmp/certbot-dns-vultr-1.0.3.tar.gz` & `tmp/certbot-dns-vultr-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-vultr-1.0.3.tar", last modified: Wed Sep 30 10:18:07 2020, max compression
+gzip compressed data, was "certbot-dns-vultr-1.1.0rc1.tar", last modified: Mon May 22 13:25:55 2023, max compression
```

## Comparing `certbot-dns-vultr-1.0.3.tar` & `certbot-dns-vultr-1.1.0rc1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/
--rw-r--r--   0 matt      (1000) matt      (1000)     3545 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     2034 2020-09-30 10:10:11.000000 certbot-dns-vultr-1.0.3/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     3545 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      297 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       63 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       32 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       18 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)     5972 2020-09-30 10:10:11.000000 certbot-dns-vultr-1.0.3/certbot_dns_vultr.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1066 2020-09-30 10:18:07.000000 certbot-dns-vultr-1.0.3/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2020-09-30 10:10:11.000000 certbot-dns-vultr-1.0.3/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-22 13:25:55.985108 certbot-dns-vultr-1.1.0rc1/
+-rw-r--r--   0 matt       (501) staff       (20)      880 2023-05-22 13:22:18.000000 certbot-dns-vultr-1.1.0rc1/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     3003 2023-05-22 13:25:55.985190 certbot-dns-vultr-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     2034 2023-05-22 13:22:18.000000 certbot-dns-vultr-1.1.0rc1/README.md
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-22 13:25:55.984954 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     3003 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      305 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       62 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/entry_points.txt
+-rw-r--r--   0 matt       (501) staff       (20)       32 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)       18 2023-05-22 13:25:55.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)     5269 2023-05-22 13:22:18.000000 certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.py
+-rw-r--r--   0 matt       (501) staff       (20)     1069 2023-05-22 13:25:55.985720 certbot-dns-vultr-1.1.0rc1/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)       38 2023-05-22 13:22:18.000000 certbot-dns-vultr-1.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-vultr-1.0.3/README.md` & `certbot-dns-vultr-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-vultr-1.0.3/certbot_dns_vultr.py` & `certbot-dns-vultr-1.1.0rc1/certbot_dns_vultr.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,57 +52,55 @@
         return self.vultr
 
 
 class VultrClient:
     def __init__(self, key):
         self.api_key = key
         self.domains_cache = None
-        self.added_records = set()
+        self.added_records = dict()
 
     def add_txt_record(self, domain_name, record_name, record_data):
         try:
             base_domain_name = self.get_base_domain_name(domain_name)
             relative_record_name = self.get_relative_record_name(base_domain_name, record_name)
 
-            self.request("POST", "/dns/create_record", {
-                "domain": base_domain_name,
+            result = self.request("POST", f"/domains/{base_domain_name}/records", {
                 "type": "TXT",
                 "name": relative_record_name,
                 "data": quote(record_data),
             })
 
-            self.added_records.add((record_name, record_data))
+            self.added_records[(record_name, record_data)] = result["record"]["id"]
             logger.debug(f'Successfully added TXT record for "{domain_name}"')
         except (VultrPluginError, requests.HTTPError) as err:
-            error_message = err.message if isinstance(err, VultrPluginError) else response_error_message(err)
+            error_message = err.message if isinstance(err, VultrPluginError) else http_error_message(err)
             raise errors.PluginError(f'Failed to add TXT record for "{domain_name}": {error_message}')
 
     def del_txt_record(self, domain_name, record_name, record_data):
         if (record_name, record_data) not in self.added_records:
             logger.debug(f'Skipping deletion of TXT record for "{domain_name}" since it was not successfully added')
             return
 
         try:
             base_domain_name = self.get_base_domain_name(domain_name)
-            relative_record_name = self.get_relative_record_name(base_domain_name, record_name)
-            record_id = self.get_record_id(base_domain_name, relative_record_name, record_data)
+            record_id = self.added_records[(record_name, record_data)]
 
-            self.request("POST", "/dns/delete_record", {"domain": base_domain_name, "RECORDID": record_id})
+            self.request("DELETE", f"/domains/{base_domain_name}/records/{record_id}")
 
             logger.debug(f'Successfully deleted TXT record for "{domain_name}"')
         except (VultrPluginError, requests.HTTPError) as err:
             error_message = err.message if isinstance(err, VultrPluginError) else http_error_message(err)
             logger.warning(f'Failed to delete TXT record for "{domain_name}": {error_message}')
 
     def get_base_domain_name(self, full_domain_name):
         if self.domains_cache is not None:
             domains = self.domains_cache
         else:
             try:
-                domains = self.domains_cache = self.request("GET", "/dns/list")
+                domains = self.domains_cache = self.request("GET", "/domains")["domains"]
             except requests.HTTPError as err:
                 raise VultrPluginError("Error fetching DNS domains list: " + http_error_message(err))
 
         guess_list = dns_common.base_domain_name_guesses(full_domain_name)
         for guess in guess_list:
             for base_domain in domains:
                 if base_domain["domain"] == guess:
@@ -110,30 +108,18 @@
                     return guess
 
         raise VultrPluginError(f'Could not find the (base) domain for "{full_domain_name}" (Is the domain set in your DNS?)')
 
     def get_relative_record_name(self, base_domain_name, absolute_record_name):
         return absolute_record_name[:-len("." + base_domain_name)]
 
-    def get_record_id(self, base_domain_name, relative_record_name, record_data):
-        try:
-            dns_records = self.request("GET", "/dns/records?domain=" + base_domain_name)
-        except requests.HTTPError as err:
-            raise VultrPluginError(f'Error fetching DNS records for "{base_domain_name}": {http_error_message(err)}')
-
-        for r in dns_records:
-            if r.get("type") == "TXT" and r.get("name") == relative_record_name and r.get("data") == quote(record_data):
-                return r["RECORDID"]
-
-        raise VultrPluginError("TXT record not found")
-
     def request(self, method, path, data=None):
-        url = "https://api.vultr.com/v1" + path
+        url = "https://api.vultr.com/v2" + path
 
-        response = requests.request(method, url, data=data, headers={"API-Key": self.api_key})
+        response = requests.request(method, url, json=data, headers={"Authorization": f"Bearer {self.api_key}"})
         response.raise_for_status()
 
         if response.headers["Content-Type"] == "application/json":
             return response.json()
         else:
             return response.text
```

### Comparing `certbot-dns-vultr-1.0.3/setup.cfg` & `certbot-dns-vultr-1.1.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = certbot-dns-vultr
-version = 1.0.3
+version = 1.1.0rc1
 description = Vultr DNS authenticator plugin for Certbot
 url = https://github.com/lezgomatt/certbot-dns-vultr
 author = Matt
 author_email = lezgomatt@gmail.com
 license = Zlib
 long_description = file: README.md
 long_description_content_type = text/markdown
```

