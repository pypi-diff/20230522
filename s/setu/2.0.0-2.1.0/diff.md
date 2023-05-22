# Comparing `tmp/setu-2.0.0.tar.gz` & `tmp/setu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setu-2.0.0.tar", max compression
+gzip compressed data, was "setu-2.1.0.tar", max compression
```

## Comparing `setu-2.0.0.tar` & `setu-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1093 2022-07-19 05:18:27.096965 setu-2.0.0/LICENSE
--rw-r--r--   0        0        0     4471 2022-07-19 05:18:27.096965 setu-2.0.0/README.md
--rw-r--r--   0        0        0     2036 2022-07-19 05:18:27.100966 setu-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      197 2022-07-19 05:18:27.100966 setu-2.0.0/setu/__init__.py
--rw-r--r--   0        0        0     1347 2022-07-19 05:18:27.100966 setu-2.0.0/setu/auth.py
--rw-r--r--   0        0        0     4463 2022-07-19 05:18:27.100966 setu-2.0.0/setu/body.py
--rw-r--r--   0        0        0     4266 2022-07-19 05:18:27.100966 setu-2.0.0/setu/contract.py
--rw-r--r--   0        0        0     9317 2022-07-19 05:18:27.100966 setu-2.0.0/setu/deeplink.py
--rw-r--r--   0        0        0      797 2022-07-19 05:18:27.100966 setu-2.0.0/setu/endpoint.py
--rw-r--r--   0        0        0     6678 2022-07-19 05:18:27.100966 setu-2.0.0/setu/serial.py
--rw-r--r--   0        0        0       45 2022-07-19 05:18:27.100966 setu-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      576 2022-07-19 05:18:27.100966 setu-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      854 2022-07-19 05:18:27.100966 setu-2.0.0/tests/test_auth.py
--rw-r--r--   0        0        0     4421 2022-07-19 05:18:27.100966 setu-2.0.0/tests/test_deeplink.py
--rw-r--r--   0        0        0      558 2022-07-19 05:18:27.100966 setu-2.0.0/tests/test_endpoint.py
--rw-r--r--   0        0        0     5427 2022-07-19 05:19:31.579446 setu-2.0.0/setup.py
--rw-r--r--   0        0        0     5492 2022-07-19 05:19:31.579958 setu-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-22 06:27:32.760287 setu-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4613 2023-05-22 06:27:32.760287 setu-2.1.0/README.md
+-rw-r--r--   0        0        0     2088 2023-05-22 06:27:32.764287 setu-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      197 2023-05-22 06:27:32.764287 setu-2.1.0/setu/__init__.py
+-rw-r--r--   0        0        0     1347 2023-05-22 06:27:32.764287 setu-2.1.0/setu/auth.py
+-rw-r--r--   0        0        0     4463 2023-05-22 06:27:32.764287 setu-2.1.0/setu/body.py
+-rw-r--r--   0        0        0     4305 2023-05-22 06:27:32.764287 setu-2.1.0/setu/contract.py
+-rw-r--r--   0        0        0     9621 2023-05-22 06:27:32.764287 setu-2.1.0/setu/deeplink.py
+-rw-r--r--   0        0        0      797 2023-05-22 06:27:32.764287 setu-2.1.0/setu/endpoint.py
+-rw-r--r--   0        0        0     6757 2023-05-22 06:27:32.764287 setu-2.1.0/setu/serial.py
+-rw-r--r--   0        0        0       45 2023-05-22 06:27:32.764287 setu-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-22 06:27:32.764287 setu-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      854 2023-05-22 06:27:32.764287 setu-2.1.0/tests/test_auth.py
+-rw-r--r--   0        0        0     4405 2023-05-22 06:27:32.764287 setu-2.1.0/tests/test_deeplink.py
+-rw-r--r--   0        0        0     1381 2023-05-22 06:27:32.764287 setu-2.1.0/tests/test_deeplink_expire.py
+-rw-r--r--   0        0        0      558 2023-05-22 06:27:32.764287 setu-2.1.0/tests/test_endpoint.py
+-rw-r--r--   0        0        0     5685 1970-01-01 00:00:00.000000 setu-2.1.0/PKG-INFO
```

### Comparing `setu-2.0.0/LICENSE` & `setu-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/README.md` & `setu-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Downloads](https://img.shields.io/pypi/dw/setu?color=%23FEB452)](https://pypi.org/project/setu)
 [![License](https://img.shields.io/pypi/l/setu?color=%23FE90A0)](LICENSE.md)
 
 <img src="https://raw.githubusercontent.com/SetuHQ/setu-python-sdk/master/assets/deeplinks.png" alt="SDK in action" width="100%">
 
 ## Getting started
 
-[SDK documentation →](https://opensource.setu.co/setu-python-sdk)  
+[SDK documentation →](https://setuhq.github.io/upi-deeplinks-python-sdk/)  
 [Full documentation →](https://docs.setu.co/payments/upi-deeplinks)  
 [Product overview →](https://setu.co/payments/upi-deeplinks)
 
 ### Installation
 
 ```bash
 pip install setu
@@ -88,28 +88,37 @@
 ```python
 try:
     dl.trigger_mock_settlement([credit_response.utr])
 except SetuAPIException as e:
     assert False
 ```
 
+### Expire bill payment
+
+```python
+try:
+    dl.expire_payment_link(link.platform_bill_id)
+except SetuAPIException as e:
+    assert False
+```
+
 ### Initiate Refund
 
 ```python
 try:
     batch_initiate_refund_response = dl.initiate_batch_refund(
         refunds=[
             RefundRequestItem(
                 identifier=link.platform_bill_id,
                 identifierType="BILL_ID",
                 refundType="FULL",
             ),
         ],
     )
-    assert batch_initiate_refund_response.refunds[0].status == "MarkedForRefund"
+    assert batch_initiate_refund_response.refunds[0].status == "Pending"
 except SetuAPIException as e:
     assert False
 ```
 
 ### Get refund batch status
 
 ```python
```

### Comparing `setu-2.0.0/pyproject.toml` & `setu-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "setu"
-version = "2.0.0"
+version = "2.1.0"
 homepage = "https://github.com/SetuHQ/setu-python-sdk"
 description = "Python package to connect to Setu's UPI Deep Link APIs."
 authors = ["Naresh R <ghostwriternr@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
@@ -49,14 +49,16 @@
 mkdocstrings = "^0.17.0"
 mkdocs-material-extensions = "^1.0.1"
 twine = "^3.8.0"
 mkdocs-autorefs = "^0.3.1"
 pre-commit = "^2.17.0"
 toml = "^0.10.2"
 bump2version = "^1.0.1"
+types-requests = "^2.30.0.0"
+types-deprecated = "^1.2.9.2"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ['py36', 'py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
@@ -82,9 +84,9 @@
 ensure_newline_before_comments = true
 line_length = 120
 skip_gitignore = true
 # you can skip files as below
 #skip_glob = docs/conf.py
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `setu-2.0.0/setu/auth.py` & `setu-2.1.0/setu/auth.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/setu/body.py` & `setu-2.1.0/setu/body.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/setu/contract.py` & `setu-2.1.0/setu/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,17 @@
 class RefundResponseItem:
     """Refund response item."""
 
     id: str
     bill_id: str
     transaction_ref_id: str
     amount: Amount
+    type: str
     status: str
+    created_at: datetime
     deductions: Optional[List[Deduction]] = None
     initiated_at: Optional[datetime] = None
 
 
 @dataclass
 class InitiateBatchRefundResponse:
     """Initiate Batch Refund Response."""
```

### Comparing `setu-2.0.0/setu/deeplink.py` & `setu-2.1.0/setu/deeplink.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,23 @@
             json=payload,
             headers=self.headers,
         )
         mock_credit_response_data_schema = MockCreditResponseDataSchema()
         return mock_credit_response_data_schema.load(api_response.json()['data'])
 
     @Decorators.auth_handler
+    def expire_payment_link(self, platform_bill_id: str):
+        """Expire payment link."""
+        self.session.post(
+            get_url_path(API.EXPIRE_BILL, self.auth_type, self.mode).format(platform_bill_id),
+            headers=self.headers,
+        )
+        return
+
+    @Decorators.auth_handler
     def trigger_mock_settlement(self, utrs: List[str]):
         """Trigger mock settlement."""
         payload: Dict[str, Any] = get_mock_settlement_body(utrs=utrs)
 
         self.session.post(
             get_url_path(API.TRIGGER_MOCK_SETTLEMENT, self.auth_type, self.mode),
             json=payload,
```

### Comparing `setu-2.0.0/setu/endpoint.py` & `setu-2.1.0/setu/endpoint.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/setu/serial.py` & `setu-2.1.0/setu/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,17 @@
     """Refund Response Item Schema."""
 
     id = fields.Str()
     bill_id = fields.Str(data_key="billID")
     transaction_ref_id = fields.Str(data_key="transactionRefID")
     amount = fields.Nested(AmountSchema())
     status = fields.Str()
+    type = fields.Str()
     deductions = fields.List(fields.Nested(DeductionResponseSchema()), required=False)
+    created_at = fields.DateTime(data_key="createdAt")
     initiated_at = fields.DateTime(data_key="initiatedAt", required=False)
 
     @post_load
     def make_refund_response_item(self, data, **kwargs):
         """Deserialize to RefundResponseItem object."""
         return RefundResponseItem(**data)
```

### Comparing `setu-2.0.0/tests/conftest.py` & `setu-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/tests/test_auth.py` & `setu-2.1.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/tests/test_deeplink.py` & `setu-2.1.0/tests/test_deeplink.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,30 +88,30 @@
                     identifierType="BILL_ID",
                     refundType="FULL",
                     deductions=[split_account],
                 ),
             ],
         )
         LOGGER.info(batch_initiate_refund_response)
-        assert batch_initiate_refund_response.refunds[0].status == "MarkedForRefund"
+        assert batch_initiate_refund_response.refunds[0].status == "Pending"
 
         # Get refund batch status
         refund_batch_status_response = dl.get_batch_refund_status(batch_initiate_refund_response.batch_id)
         LOGGER.info(refund_batch_status_response)
         assert refund_batch_status_response.refunds[0].bill_id == link.platform_bill_id
 
         refund_batch_status_response = dl.get_refund_status_by_identifier(
             "batch", batch_initiate_refund_response.batch_id
         )
         LOGGER.info(refund_batch_status_response)
         assert refund_batch_status_response.refunds[0].bill_id == link.platform_bill_id
 
         refund_batch_status_response = dl.get_refund_status_by_identifier("bill", link.platform_bill_id)
         LOGGER.info(refund_batch_status_response)
-        assert refund_batch_status_response.refunds[0].status == "MarkedForRefund"
+        assert refund_batch_status_response.refunds[0].status == "Pending"
 
         # Get individual refund status
         refund_status_response = dl.get_refund_status(batch_initiate_refund_response.refunds[0].id)
         LOGGER.info(refund_status_response)
         assert refund_status_response.bill_id == link.platform_bill_id
     except SetuAPIException as e:
         LOGGER.error(e.error)
```

### Comparing `setu-2.0.0/tests/test_endpoint.py` & `setu-2.1.0/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `setu-2.0.0/setup.py` & `setu-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: setu
+Version: 2.1.0
+Summary: Python package to connect to Setu's UPI Deep Link APIs.
+Home-page: https://github.com/SetuHQ/setu-python-sdk
+License: MIT
+Author: Naresh R
+Author-email: ghostwriternr@gmail.com
+Requires-Python: >=3.6.2,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
+Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: marshmallow (>=3.14.1,<4.0.0)
+Requires-Dist: marshmallow-oneofschema (>=3.0.1,<4.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Description-Content-Type: text/markdown
+
+# Setu UPI DeepLinks: Python SDK
+
+`setu` is a Python SDK for accessing Setu’s [UPI Deeplinks](https://docs.setu.co/collect/biller/upi-deep-links) APIs. The SDK is designed with ease of access in mind, with native Python class objects for inputs & ouputs and custom exceptions.
+
+[![Version](https://img.shields.io/pypi/v/setu?color=%2320014B)](https://pypi.org/project/setu)
+[![Downloads](https://img.shields.io/pypi/dw/setu?color=%23FEB452)](https://pypi.org/project/setu)
+[![License](https://img.shields.io/pypi/l/setu?color=%23FE90A0)](LICENSE.md)
+
+<img src="https://raw.githubusercontent.com/SetuHQ/setu-python-sdk/master/assets/deeplinks.png" alt="SDK in action" width="100%">
+
+## Getting started
+
+[SDK documentation →](https://setuhq.github.io/upi-deeplinks-python-sdk/)  
+[Full documentation →](https://docs.setu.co/payments/upi-deeplinks)  
+[Product overview →](https://setu.co/payments/upi-deeplinks)
+
+### Installation
+
+```bash
+pip install setu
+```
+
+### Features
+
+-   Full support for latest UPI Deeplinks APIs
+-   Native Python class objects for all inputs & responses
+-   Allows both [JWT](https://docs.setu.co/payments/upi-deeplinks/resources/jwt) & [OAuth](https://docs.setu.co/payments/upi-deeplinks/resources/oauth) authentication mechanisms
+-   `SANDBOX` mode to test integration & `PRODUCTION` for live data
+-   Internal mechanism for OAuth authentication to automatically re-fetch token when current one expires, and retry all failed requests.
+
+## Examples
+
+### Setup
+
+```python
+from setu import Deeplink
+from setu.contract import RefundRequestItem, SetuAPIException
+
+dl = Deeplink(
+    scheme_id="c4f57443-dc1e-428f-8c4e-e5fd531057d2",
+    secret="5b288618-473f-4193-ae1b-8c42f223798e",
+    product_instance_id="861023031961584801",
+    auth_type="OAUTH",
+    mode="SANDBOX",
+)
+```
+
+### Generate UPI payment link
+
+```python
+bill_amount = 100
+try:
+    link = dl.create_payment_link(
+        amount_value=bill_amount,
+        biller_bill_id="test_transaction_1234",
+        amount_exactness="EXACT",
+        payee_name="Python SDK unittest",
+        transaction_note="unittest transaction",
+    )
+    assert link.payment_link.upi_id == "refundtest@kaypay"
+except SetuException as e:
+    assert False
+```
+
+### Get Payment Link Status
+
+```python
+try:
+    link_status = dl.check_payment_status(link.platform_bill_id)
+    assert link_status.status == "BILL_CREATED"
+except SetuAPIException as e:
+    assert False
+```
+
+### Trigger mock payment for UPI payment link (Sandbox only)
+
+```python
+try:
+    credit_response = dl.trigger_mock_payment(
+        float(bill_amount) / 100, link.payment_link.upi_id, link.platform_bill_id
+    )
+except SetuAPIException as e:
+    assert False
+```
+
+### Mock Settlement
+
+```python
+try:
+    dl.trigger_mock_settlement([credit_response.utr])
+except SetuAPIException as e:
+    assert False
+```
+
+### Expire bill payment
+
+```python
+try:
+    dl.expire_payment_link(link.platform_bill_id)
+except SetuAPIException as e:
+    assert False
+```
+
+### Initiate Refund
+
+```python
+try:
+    batch_initiate_refund_response = dl.initiate_batch_refund(
+        refunds=[
+            RefundRequestItem(
+                identifier=link.platform_bill_id,
+                identifierType="BILL_ID",
+                refundType="FULL",
+            ),
+        ],
+    )
+    assert batch_initiate_refund_response.refunds[0].status == "Pending"
+except SetuAPIException as e:
+    assert False
+```
+
+### Get refund batch status
+
+```python
+try:
+    refund_batch_status_response = dl.get_batch_refund_status(batch_initiate_refund_response.batch_id)
+    assert refund_batch_status_response.refunds[0].bill_id == link.platform_bill_id
+except SetuAPIException as e:
+    assert False
+```
+
+### Get individual refund status
+
+```python
+try:
+    refund_status_response = dl.get_refund_status(batch_initiate_refund_response.refunds[0].id)
+    assert refund_status_response.bill_id == link.platform_bill_id
+except SetuAPIException as e:
+    assert False
+```
+
+## Contributing
+
+Have a look through existing [Issues](https://github.com/SetuHQ/setu-python-sdk/issues) and [Pull Requests](https://github.com/SetuHQ/setu-python-sdk/pulls) that you could help with. If you'd like to request a feature or report a bug, please [create a GitHub Issue](https://github.com/SetuHQ/setu-python-sdk/issues) using the template provided.
+
+[See contribution guide →](CONTRIBUTING.md)
 
-packages = \
-['setu', 'tests']
+## Credits
 
-package_data = \
-{'': ['*']}
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
 
-install_requires = \
-['Deprecated>=1.2.13,<2.0.0',
- 'PyJWT>=2.4.0,<3.0.0',
- 'marshmallow-oneofschema>=3.0.1,<4.0.0',
- 'marshmallow>=3.14.1,<4.0.0',
- 'requests>=2.27.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'setu',
-    'version': '2.0.0',
-    'description': "Python package to connect to Setu's UPI Deep Link APIs.",
-    'long_description': '# Setu UPI DeepLinks: Python SDK\n\n`setu` is a Python SDK for accessing Setu’s [UPI Deeplinks](https://docs.setu.co/collect/biller/upi-deep-links) APIs. The SDK is designed with ease of access in mind, with native Python class objects for inputs & ouputs and custom exceptions.\n\n[![Version](https://img.shields.io/pypi/v/setu?color=%2320014B)](https://pypi.org/project/setu)\n[![Downloads](https://img.shields.io/pypi/dw/setu?color=%23FEB452)](https://pypi.org/project/setu)\n[![License](https://img.shields.io/pypi/l/setu?color=%23FE90A0)](LICENSE.md)\n\n<img src="https://raw.githubusercontent.com/SetuHQ/setu-python-sdk/master/assets/deeplinks.png" alt="SDK in action" width="100%">\n\n## Getting started\n\n[SDK documentation →](https://opensource.setu.co/setu-python-sdk)  \n[Full documentation →](https://docs.setu.co/payments/upi-deeplinks)  \n[Product overview →](https://setu.co/payments/upi-deeplinks)\n\n### Installation\n\n```bash\npip install setu\n```\n\n### Features\n\n-   Full support for latest UPI Deeplinks APIs\n-   Native Python class objects for all inputs & responses\n-   Allows both [JWT](https://docs.setu.co/payments/upi-deeplinks/resources/jwt) & [OAuth](https://docs.setu.co/payments/upi-deeplinks/resources/oauth) authentication mechanisms\n-   `SANDBOX` mode to test integration & `PRODUCTION` for live data\n-   Internal mechanism for OAuth authentication to automatically re-fetch token when current one expires, and retry all failed requests.\n\n## Examples\n\n### Setup\n\n```python\nfrom setu import Deeplink\nfrom setu.contract import RefundRequestItem, SetuAPIException\n\ndl = Deeplink(\n    scheme_id="c4f57443-dc1e-428f-8c4e-e5fd531057d2",\n    secret="5b288618-473f-4193-ae1b-8c42f223798e",\n    product_instance_id="861023031961584801",\n    auth_type="OAUTH",\n    mode="SANDBOX",\n)\n```\n\n### Generate UPI payment link\n\n```python\nbill_amount = 100\ntry:\n    link = dl.create_payment_link(\n        amount_value=bill_amount,\n        biller_bill_id="test_transaction_1234",\n        amount_exactness="EXACT",\n        payee_name="Python SDK unittest",\n        transaction_note="unittest transaction",\n    )\n    assert link.payment_link.upi_id == "refundtest@kaypay"\nexcept SetuException as e:\n    assert False\n```\n\n### Get Payment Link Status\n\n```python\ntry:\n    link_status = dl.check_payment_status(link.platform_bill_id)\n    assert link_status.status == "BILL_CREATED"\nexcept SetuAPIException as e:\n    assert False\n```\n\n### Trigger mock payment for UPI payment link (Sandbox only)\n\n```python\ntry:\n    credit_response = dl.trigger_mock_payment(\n        float(bill_amount) / 100, link.payment_link.upi_id, link.platform_bill_id\n    )\nexcept SetuAPIException as e:\n    assert False\n```\n\n### Mock Settlement\n\n```python\ntry:\n    dl.trigger_mock_settlement([credit_response.utr])\nexcept SetuAPIException as e:\n    assert False\n```\n\n### Initiate Refund\n\n```python\ntry:\n    batch_initiate_refund_response = dl.initiate_batch_refund(\n        refunds=[\n            RefundRequestItem(\n                identifier=link.platform_bill_id,\n                identifierType="BILL_ID",\n                refundType="FULL",\n            ),\n        ],\n    )\n    assert batch_initiate_refund_response.refunds[0].status == "MarkedForRefund"\nexcept SetuAPIException as e:\n    assert False\n```\n\n### Get refund batch status\n\n```python\ntry:\n    refund_batch_status_response = dl.get_batch_refund_status(batch_initiate_refund_response.batch_id)\n    assert refund_batch_status_response.refunds[0].bill_id == link.platform_bill_id\nexcept SetuAPIException as e:\n    assert False\n```\n\n### Get individual refund status\n\n```python\ntry:\n    refund_status_response = dl.get_refund_status(batch_initiate_refund_response.refunds[0].id)\n    assert refund_status_response.bill_id == link.platform_bill_id\nexcept SetuAPIException as e:\n    assert False\n```\n\n## Contributing\n\nHave a look through existing [Issues](https://github.com/SetuHQ/setu-python-sdk/issues) and [Pull Requests](https://github.com/SetuHQ/setu-python-sdk/pulls) that you could help with. If you\'d like to request a feature or report a bug, please [create a GitHub Issue](https://github.com/SetuHQ/setu-python-sdk/issues) using the template provided.\n\n[See contribution guide →](CONTRIBUTING.md)\n\n## Credits\n\nThis package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.\n\n## License\n\nMIT. Have at it.\n',
-    'author': 'Naresh R',
-    'author_email': 'ghostwriternr@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/SetuHQ/setu-python-sdk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0',
-}
+## License
 
+MIT. Have at it.
 
-setup(**setup_kwargs)
```

