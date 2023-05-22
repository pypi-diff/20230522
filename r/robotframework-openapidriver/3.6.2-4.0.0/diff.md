# Comparing `tmp/robotframework_openapidriver-3.6.2.tar.gz` & `tmp/robotframework_openapidriver-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapidriver-3.6.2.tar", max compression
+gzip compressed data, was "robotframework_openapidriver-4.0.0.tar", max compression
```

## Comparing `robotframework_openapidriver-3.6.2.tar` & `robotframework_openapidriver-4.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4747 2023-02-17 14:35:26.280382 robotframework_openapidriver-3.6.2/docs/README.md
--rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-3.6.2/LICENSE
--rw-r--r--   0        0        0     2302 2023-02-17 14:24:28.558817 robotframework_openapidriver-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     1103 2022-01-11 08:27:46.400406 robotframework_openapidriver-3.6.2/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32529 2023-02-17 14:31:44.730376 robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapi_executors.py
--rw-r--r--   0        0        0     3279 2023-02-17 14:31:44.528840 robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    22731 2023-02-17 14:35:26.201361 robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    13431 2023-02-17 14:35:16.085962 robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapidriver.py
--rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 robotframework_openapidriver-3.6.2/setup.py
--rw-r--r--   0        0        0     5778 1970-01-01 00:00:00.000000 robotframework_openapidriver-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4763 2023-05-22 14:37:21.907738 robotframework_openapidriver-4.0.0/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2966 2023-05-22 13:30:25.858447 robotframework_openapidriver-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1103 2022-01-11 08:27:46.400406 robotframework_openapidriver-4.0.0/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32663 2023-05-22 14:15:42.315705 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_executors.py
+-rw-r--r--   0        0        0     4573 2023-05-22 14:23:32.088745 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    23429 2023-05-22 14:37:21.799096 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    14035 2023-05-22 14:25:04.781026 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.py
+-rw-r--r--   0        0        0     5640 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.0.0/setup.py
+-rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.0.0/PKG-INFO
```

### Comparing `robotframework_openapidriver-3.6.2/docs/README.md` & `robotframework_openapidriver-4.0.0/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 ## OpenAPI (aka Swagger)
 
 The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
 to RESTful APIs, see https://swagger.io/specification/
 
 The OpenApiDriver module implements a reader class that generates a test case for
-each endpoint, method and response that is defined in an OpenAPI document, typically
-an openapi.json or openapi.yaml file.
+each path, method and response (i.e. every response for each endpoint) that is defined
+in an OpenAPI document, typically an openapi.json or openapi.yaml file.
 
 > Note: OpenApiDriver is designed for APIs based on the OAS v3
 The library has not been tested for APIs based on the OAS v2.
 
 ---
 
 ## Getting started
@@ -82,21 +82,21 @@
 *** Settings ***
 Library            OpenApiDriver
 ...                    source=http://localhost:8000/openapi.json
 ...                    origin=http://localhost:8000
 Test Template      Validate Using Test Endpoint Keyword
 
 *** Test Cases ***
-Test Endpoint for ${method} on ${endpoint} where ${status_code} is expected
+Test Endpoint for ${method} on ${path} where ${status_code} is expected
 
 *** Keywords ***
 Validate Using Test Endpoint Keyword
-    [Arguments]    ${endpoint}    ${method}    ${status_code}
+    [Arguments]    ${path}    ${method}    ${status_code}
     Test Endpoint
-    ...    endpoint=${endpoint}    method=${method}    status_code=${status_code}
+    ...    path=${path}    method=${method}    status_code=${status_code}
 
 ```
 
 Running the above suite for the first time is likely to result in some
 errors / failed tests.
 You should look at the Robot Framework `log.html` to determine the reasons
 for the failing tests.
@@ -116,9 +116,9 @@
 ---
 
 ## Limitations
 
 There are currently a number of limitations to supported API structures, supported
 data types and properties. The following list details the most important ones:
 - Only JSON request and response bodies are supported.
-- No support for per-endpoint authorization levels (only simple 401 / 403 validation).
+- No support for per-path authorization levels (only simple 401 / 403 validation).
```

### Comparing `robotframework_openapidriver-3.6.2/LICENSE` & `robotframework_openapidriver-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-3.6.2/pyproject.toml` & `robotframework_openapidriver-4.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapidriver"
-version = "3.6.2"
+version = "4.0.0"
 description = "A library for contract-testing OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapidriver"
 classifiers = [
@@ -20,29 +20,38 @@
     { include = "OpenApiDriver", from = "src" },
 ]
 include = ["*.libspec"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 robotframework-datadriver = ">=1.6.1"
-robotframework-openapi-libcore = "^1.8.2"
+robotframework-openapi-libcore = "^1.8.5"
 
 [tool.poetry.group.dev.dependencies]
-black = "*"
-isort = "*"
-pylint = "*"
-mypy = "*"
-types-requests = "^2.25.6"
-invoke = "*"
-robotframework-stacktrace = "*"
-robotframework-tidy = "^3.3.3"
-robotframework-robocop = "^2.7.0"
-uvicorn = "*"
-fastapi = ">=0.88"
-coverage = {version = "^5.5", extras = ["toml"]}
+fastapi = ">=0.95.0"
+uvicorn = ">=0.22.0"
+invoke = ">=2.0.0"
+coverage = {version=">=7.2.5", extras = ["toml"]}
+robotframework-stacktrace = ">=0.4.1"
+
+[tool.poetry.group.formatting.dependencies]
+black = ">=22.10.0"
+isort = ">=5.10.1"
+robotframework-tidy = ">=3.4.0"
+
+[tool.poetry.group.type-checking.dependencies]
+mypy = ">=1.2.0"
+pyright = ">=1.1.300"
+types-requests = ">=2.28.11"
+types-invoke = ">=2.0.0.6"
+
+[tool.poetry.group.linting.dependencies]
+pylint = ">=2.17.2"
+ruff = ">=0.0.267"
+robotframework-robocop = ">=2.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 branch = true
@@ -52,14 +61,21 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract"
 ]
 
 [tool.mypy]
+plugins = ["pydantic.mypy"]
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+disallow_untyped_defs = true
+strict = true
 show_error_codes = true
 
 [[tool.mypy.overrides]]
 module = [
     "DataDriver.*",
     "prance.*",
     "robot.*",
@@ -71,26 +87,39 @@
 ignore_missing_imports = true
 
 [tool.black]
 line-length = 88
 target-version = ["py38"]
 
 [tool.isort]
-src_paths = [
-    "src"
-]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 88
+profile = "black"
+py_version=38
+
+[tool.ruff]
+line-length = 120
+select = ["E", "F", "PL"]
+src = ["src/OpenApiDriver"]
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = ["logging-fstring-interpolation", "missing-class-docstring"]
 
 [tool.pylint.'FORMAT CHECKER']
 max-line-length=120
 
 [tool.pylint.'SIMILARITIES CHECKER']
 ignore-imports="yes"
+
+[tool.robotidy]
+line_length = 120
+spacecount = 4
+
+[tool.robocop]
+filetypes = [".robot", ".resource"]
+configure = [
+    "line-too-long:line_length:120"
+]
+exclude = [
+    "missing-doc-suite",
+    "missing-doc-test-case",
+    "missing-doc-keyword",
+    "too-few-calls-in-test-case"
+]
```

### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/__init__.py` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_executors.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     STRICT = "STRICT"
 
 
 @library(scope="TEST SUITE", doc_format="ROBOT")
 class OpenApiExecutors(OpenApiLibCore):  # pylint: disable=too-many-instance-attributes
     """Main class providing the keywords and core logic to perform endpoint validations."""
 
-    def __init__(  # pylint: disable=too-many-arguments, dangerous-default-value
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         source: str,
         origin: str = "",
         base_path: str = "",
         mappings_path: Union[str, Path] = "",
         username: str = "",
         password: str = "",
@@ -79,94 +79,92 @@
         )
         self.response_validation = response_validation
         self.disable_server_validation = disable_server_validation
         self.require_body_for_invalid_url = require_body_for_invalid_url
         self.invalid_property_default_response = invalid_property_default_response
 
     @keyword
-    def test_unauthorized(self, endpoint: str, method: str) -> None:
+    def test_unauthorized(self, path: str, method: str) -> None:
         """
-        Perform a request for `method` on the `endpoint`, with no authorization.
+        Perform a request for `method` on the `path`, with no authorization.
 
         This keyword only passes if the response code is 401: Unauthorized.
 
         Any authorization parameters used to initialize the library are
         ignored for this request.
         > Note: No headers or (json) body are send with the request. For security
         reasons, the authorization validation should be checked first.
         """
-        url: str = run_keyword("get_valid_url", endpoint, method)
+        url: str = run_keyword("get_valid_url", path, method)
         response = self.session.request(
             method=method,
             url=url,
             verify=False,
         )
         assert response.status_code == 401
 
     @keyword
     def test_invalid_url(
-        self, endpoint: str, method: str, expected_status_code: int = 404
+        self, path: str, method: str, expected_status_code: int = 404
     ) -> None:
         """
-        Perform a request for the provided 'endpoint' and 'method' where the url for
-        the `endpoint` is invalidated.
+        Perform a request for the provided 'path' and 'method' where the url for
+        the `path` is invalidated.
 
-        This keyword will be `SKIPPED` if the endpoint contains no parts that
+        This keyword will be `SKIPPED` if the path contains no parts that
         can be invalidated.
 
         The optional `expected_status_code` parameter (default: 404) can be set to the
         expected status code for APIs that do not return a 404 on invalid urls.
 
         > Note: Depending on API design, the url may be validated before or after
         validation of headers, query parameters and / or (json) body. By default, no
         parameters are send with the request. The `require_body_for_invalid_url`
         parameter can be set to `True` if needed.
         """
-        valid_url: str = run_keyword("get_valid_url", endpoint, method)
+        valid_url: str = run_keyword("get_valid_url", path, method)
 
         if not (url := run_keyword("get_invalidated_url", valid_url)):
             raise SkipExecution(
-                f"Endpoint {endpoint} does not contain resource references that "
+                f"Path {path} does not contain resource references that "
                 f"can be invalidated."
             )
 
         params, headers, json_data = None, None, None
         if self.require_body_for_invalid_url:
-            request_data = self.get_request_data(method=method, endpoint=endpoint)
+            request_data = self.get_request_data(method=method, endpoint=path)
             params = request_data.params
             headers = request_data.headers
             dto = request_data.dto
             json_data = asdict(dto)
         response: Response = run_keyword(
             "authorized_request", url, method, params, headers, json_data
         )
         if response.status_code != expected_status_code:
             raise AssertionError(
                 f"Response {response.status_code} was not {expected_status_code}"
             )
 
     @keyword
-    def test_endpoint(self, endpoint: str, method: str, status_code: int) -> None:
+    def test_endpoint(self, path: str, method: str, status_code: int) -> None:
         """
-        Validate that performing the `method` operation on `endpoint` results in a
+        Validate that performing the `method` operation on `path` results in a
         `status_code` response.
 
         This is the main keyword to be used in the `Test Template` keyword when using
         the OpenApiDriver.
 
         The keyword calls other keywords to generate the neccesary data to perform
         the desired operation and validate the response against the openapi document.
         """
         json_data: Optional[Dict[str, Any]] = None
         original_data = None
 
-        url: str = run_keyword("get_valid_url", endpoint, method)
-        request_data: RequestData = self.get_request_data(
-            method=method, endpoint=endpoint
-        )
+        url: str = run_keyword("get_valid_url", path, method)
+        request_data: RequestData = self.get_request_data(method=method, endpoint=path)
         params = request_data.params
         headers = request_data.headers
         json_data = asdict(request_data.dto)
         # when patching, get the original data to check only patched data has changed
         if method == "PATCH":
             original_data = self.get_original_data(url=url)
         # in case of a status code indicating an error, ensure the error occurs
@@ -226,15 +224,15 @@
                     )
             else:
                 raise AssertionError(
                     f"No Dto mapping found to cause status_code {status_code}."
                 )
         run_keyword(
             "perform_validated_request",
-            endpoint,
+            path,
             status_code,
             RequestValues(
                 url=url,
                 method=method,
                 params=params,
                 headers=headers,
                 json_data=json_data,
@@ -243,25 +241,25 @@
         )
         if status_code < 300 and (
             request_data.has_optional_properties
             or request_data.has_optional_params
             or request_data.has_optional_headers
         ):
             logger.info("Performing request without optional properties and parameters")
-            url = run_keyword("get_valid_url", endpoint, method)
-            request_data = self.get_request_data(method=method, endpoint=endpoint)
+            url = run_keyword("get_valid_url", path, method)
+            request_data = self.get_request_data(method=method, endpoint=path)
             params = request_data.get_required_params()
             headers = request_data.get_required_headers()
             json_data = request_data.get_required_properties_dict()
             original_data = None
             if method == "PATCH":
                 original_data = self.get_original_data(url=url)
             run_keyword(
                 "perform_validated_request",
-                endpoint,
+                path,
                 status_code,
                 RequestValues(
                     url=url,
                     method=method,
                     params=params,
                     headers=headers,
                     json_data=json_data,
@@ -272,29 +270,29 @@
     def get_original_data(self, url: str) -> Optional[Dict[str, Any]]:
         """
         Attempt to GET the current data for the given url and return it.
 
         If the GET request fails, None is returned.
         """
         original_data = None
-        endpoint = self.get_parameterized_endpoint_from_url(url)
-        get_request_data = self.get_request_data(endpoint=endpoint, method="GET")
+        path = self.get_parameterized_endpoint_from_url(url)
+        get_request_data = self.get_request_data(endpoint=path, method="GET")
         get_params = get_request_data.params
         get_headers = get_request_data.headers
         response: Response = run_keyword(
             "authorized_request", url, "GET", get_params, get_headers
         )
         if response.ok:
             original_data = response.json()
         return original_data
 
     @keyword
     def perform_validated_request(
         self,
-        endpoint: str,
+        path: str,
         status_code: int,
         request_values: RequestValues,
         original_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         """
         This keyword first calls the Authorized Request keyword, then the Validate
         Response keyword and finally validates, for `DELETE` operations, whether
@@ -330,45 +328,44 @@
                 f"\nSend: {_json.dumps(request_values.json_data, indent=4, sort_keys=True)}"
                 f"\nGot: {_json.dumps(response_json, indent=4, sort_keys=True)}"
             )
             raise AssertionError(
                 f"Response status_code {response.status_code} was not {status_code}"
             )
 
-        run_keyword("validate_response", endpoint, response, original_data)
+        run_keyword("validate_response", path, response, original_data)
         if request_values.method == "DELETE":
-            get_request_data = self.get_request_data(endpoint=endpoint, method="GET")
+            get_request_data = self.get_request_data(endpoint=path, method="GET")
             get_params = get_request_data.params
             get_headers = get_request_data.headers
             get_response = run_keyword(
                 "authorized_request", request_values.url, "GET", get_params, get_headers
             )
             if response.ok:
                 if get_response.ok:
                     raise AssertionError(
                         f"Resource still exists after deletion. Url was {request_values.url}"
                     )
-                # if the endpoint supports GET, 404 is expected, if not 405 is expected
+                # if the path supports GET, 404 is expected, if not 405 is expected
                 if get_response.status_code not in [404, 405]:
                     logger.warning(
                         f"Unexpected response after deleting resource: Status_code "
                         f"{get_response.status_code} was received after trying to get {request_values.url} "
                         f"after sucessfully deleting it."
                     )
-            else:
-                if not get_response.ok:
-                    raise AssertionError(
-                        f"Resource could not be retrieved after failed deletion. "
-                        f"Url was {request_values.url}, status_code was {get_response.status_code}"
-                    )
+            elif not get_response.ok:
+                raise AssertionError(
+                    f"Resource could not be retrieved after failed deletion. "
+                    f"Url was {request_values.url}, status_code was {get_response.status_code}"
+                )
 
     @keyword
     def validate_response(
         self,
-        endpoint: str,
+        path: str,
         response: Response,
         original_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         """
         Validate the `response` by performing the following validations:
         - validate the `response` against the openapi schema for the `endpoint`
         - validate that the response does not contain extra properties
@@ -383,38 +380,51 @@
             return None
         # validate the response against the schema
         self._validate_response_against_spec(response)
 
         request_method = response.request.method
         if request_method is None:
             logger.warning(
-                f"Could not validate response for endpoint {endpoint}; no method found "
+                f"Could not validate response for path {path}; no method found "
                 f"on the request property of the provided response."
             )
             return None
 
         response_spec = self._get_response_spec(
-            endpoint=endpoint,
+            path=path,
             method=request_method,
             status_code=response.status_code,
         )
-        # "content" is optional in the OAS, if not provided, look at the response header
+
+        content_type_from_response = response.headers.get("Content-Type", "unknown")
+        mime_type_from_response, _, _ = content_type_from_response.partition(";")
+
         if not response_spec.get("content"):
-            content_type = response.headers.get("Content-Type", "unknown")
-        else:
-            # content should be a single key/value entry, so use tuple assignment
-            (content_type,) = response_spec["content"].keys()
-        if not content_type.endswith("json"):
-            # at present, only json reponses are supported
-            raise NotImplementedError(f"content_type '{content_type}' not supported")
-        if response.headers.get("Content-Type") != content_type:
+            logger.warning(
+                "The response cannot be validated: 'content' not specified in the OAS."
+            )
+            return None
+
+        # multiple content types can be specified in the OAS
+        content_types = list(response_spec["content"].keys())
+        supported_types = [
+            ct for ct in content_types if ct.partition(";")[0].endswith("json")
+        ]
+        if not supported_types:
+            raise NotImplementedError(
+                f"The content_types '{content_types}' are not supported. "
+                f"Only json types are currently supported."
+            )
+        content_type = supported_types[0]
+        mime_type = content_type.partition(";")[0]
+
+        if mime_type != mime_type_from_response:
             raise ValueError(
-                f"Content-Type '{response.headers.get('Content-Type')}' of the response "
-                f"is not '{content_type}' as specified in the OpenAPI document or the "
-                f"Content-Type was not specified."
+                f"Content-Type '{content_type_from_response}' of the response "
+                f"does not match '{mime_type}' as specified in the OpenAPI document."
             )
 
         json_response = response.json()
         response_schema = resolve_schema(
             response_spec["content"][content_type]["schema"]
         )
         if list_item_schema := response_schema.get("items"):
@@ -444,26 +454,26 @@
             self._assert_href_is_valid(href, json_response)
         # every property that was sucessfully send and that is in the response
         # schema must have the value that was send
         if response.ok and response.request.method in ["POST", "PUT", "PATCH"]:
             run_keyword("validate_send_response", response, original_data)
         return None
 
-    def _assert_href_is_valid(self, href: str, json_response: Dict[str, Any]):
+    def _assert_href_is_valid(self, href: str, json_response: Dict[str, Any]) -> None:
         url = f"{self.origin}{href}"
-        endpoint = url.replace(self.base_url, "")
-        request_data = self.get_request_data(endpoint=endpoint, method="GET")
+        path = url.replace(self.base_url, "")
+        request_data = self.get_request_data(endpoint=path, method="GET")
         params = request_data.params
         headers = request_data.headers
         get_response = run_keyword("authorized_request", url, "GET", params, headers)
         assert (
             get_response.json() == json_response
         ), f"{get_response.json()} not equal to original {json_response}"
 
-    def _validate_response_against_spec(self, response: Response):
+    def _validate_response_against_spec(self, response: Response) -> None:
         validation_result = self.validate_response_vs_spec(
             request=RequestsOpenAPIRequest(response.request),
             response=RequestsOpenAPIResponse(response),
         )
         if self.disable_server_validation:
             validation_result.errors = [
                 e for e in validation_result.errors if not isinstance(e, ServerNotFound)
@@ -714,13 +724,15 @@
                         f"match '{send_value}' in the pre-patch data"
                         f"\nPre-patch: {_json.dumps(original_data, indent=4, sort_keys=True)}"
                         f"\nGot: {_json.dumps(response_data, indent=4, sort_keys=True)}"
                     )
         return None
 
     def _get_response_spec(
-        self, endpoint: str, method: str, status_code: int
+        self, path: str, method: str, status_code: int
     ) -> Dict[str, Any]:
         method = method.lower()
         status = str(status_code)
-        spec = {**self.openapi_spec}["paths"][endpoint][method]["responses"][status]
+        spec: Dict[str, Any] = {**self.openapi_spec}["paths"][path][method][
+            "responses"
+        ][status]
         return spec
```

### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,114 @@
 """Module holding the OpenApiReader reader_class implementation."""
-from typing import Any, List, Union
+from typing import Any, Dict, List, Union
 
 from DataDriver.AbstractReaderClass import AbstractReaderClass
 from DataDriver.ReaderConfig import TestCaseData
 
 
 # pylint: disable=too-few-public-methods
 class Test:
-    """Helper class to support ignoring endpoints when generating the test cases."""
+    """
+    Helper class to support ignoring endpoint responses when generating the test cases.
+    """
 
-    def __init__(self, endpoint: str, method: str, response: Union[str, int]):
-        self.endpoint = endpoint
+    def __init__(self, path: str, method: str, response: Union[str, int]):
+        self.path = path
         self.method = method.lower()
         self.response = str(response)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, type(self)):
             return False
         return (
-            self.endpoint == other.endpoint
+            self.path == other.path
             and self.method == other.method
             and self.response == other.response
         )
 
 
 class OpenApiReader(AbstractReaderClass):
     """Implementation of the reader_class used by DataDriver."""
 
     def get_data_from_source(self) -> List[TestCaseData]:
         test_data: List[TestCaseData] = []
 
-        endpoints = getattr(self, "endpoints")
-        if ignored_endpoints := getattr(self, "ignored_endpoints", None):
-            for endpoint in ignored_endpoints:
-                endpoints.pop(endpoint)
-        if ignored_responses := getattr(self, "ignored_responses", None):
-            ignore_list: List[str] = [str(response) for response in ignored_responses]
-        else:
-            ignore_list = []
-        if ignored_testcases := getattr(self, "ignored_testcases", None):
-            ignored_tests = [Test(*test) for test in ignored_testcases]
-        else:
-            ignored_tests = []
-        for path, path_item in endpoints.items():
+        paths = getattr(self, "paths")
+        self._filter_paths(paths)
+
+        ignored_responses_ = [
+            str(response) for response in getattr(self, "ignored_responses", [])
+        ]
+
+        ignored_tests = [Test(*test) for test in getattr(self, "ignored_testcases", [])]
+
+        for path, path_item in paths.items():
+            # by reseversing the items, post/put operations come before get and delete
             for item_name, item_data in reversed(path_item.items()):
+                # this level of the OAS also contains data that's not related to a
+                # path operation
                 if item_name not in ["get", "put", "post", "delete", "patch"]:
                     continue
                 method, method_data = item_name, item_data
                 tags_from_spec = method_data.get("tags", [])
                 for response in method_data.get("responses"):
-                    # default applies to all status codes that are not specified, in
-                    # which case we don't know what to expect and thus can't verify
+                    # 'default' applies to all status codes that are not specified, in
+                    # which case we don't know what to expect and therefore can't verify
                     if (
                         response == "default"
-                        or response in ignore_list
+                        or response in ignored_responses_
                         or Test(path, method, response) in ignored_tests
                     ):
                         continue
+
                     tag_list = _get_tag_list(
                         tags=tags_from_spec, method=method, response=response
                     )
                     test_data.append(
                         TestCaseData(
                             arguments={
-                                "${endpoint}": path,
+                                "${path}": path,
                                 "${method}": method.upper(),
                                 "${status_code}": response,
                             },
                             tags=tag_list,
                         ),
                     )
         return test_data
 
+    def _filter_paths(self, paths: Dict[str, Any]) -> None:
+        def matches_include_pattern(path: str) -> bool:
+            for included_path in included_paths:
+                if path == included_path:
+                    return True
+                if included_path.endswith("*"):
+                    wildcard_include, _, _ = included_path.partition("*")
+                    if path.startswith(wildcard_include):
+                        return True
+            return False
+
+        def matches_ignore_pattern(path: str) -> bool:
+            for ignored_path in ignored_paths:
+                if path == ignored_path:
+                    return True
+
+                if ignored_path.endswith("*"):
+                    wildcard_ignore, _, _ = ignored_path.partition("*")
+                    if path.startswith(wildcard_ignore):
+                        return True
+            return False
+
+        if included_paths := getattr(self, "included_paths", ()):
+            path_list = list(paths.keys())
+            for path in path_list:
+                if not matches_include_pattern(path):
+                    paths.pop(path)
+
+        if ignored_paths := getattr(self, "ignored_paths", ()):
+            path_list = list(paths.keys())
+            for path in path_list:
+                if matches_ignore_pattern(path):
+                    paths.pop(path)
+
 
 def _get_tag_list(tags: List[str], method: str, response: str) -> List[str]:
     return [*tags, f"Method: {method.upper()}", f"Response: {response}"]
```

### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec`

 * *Files 3% similar despite different names*

#### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,34 +1,40 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-02-17T14:35:26+00:00" specversion="4" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="306">
-  <version>3.6.2</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-05-22T14:37:22+00:00" specversion="4" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="316">
+  <version>4.0.0</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="142">
-      <arguments repr="source: str, ignored_endpoints: List[str] | None = None, ignored_responses: List[int] | None = None, ignored_testcases: List[List[str]] | None = None, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, require_body_for_invalid_url: bool = False, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
+      <arguments repr="source: str, included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, require_body_for_invalid_url: bool = False, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type typedoc="string">str</type>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_endpoints: List[str] | None = None">
-          <name>ignored_endpoints</name>
-          <type typedoc="list">List[str]</type>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="included_paths: Iterable[str] | None = None">
+          <name>included_paths</name>
+          <type>Iterable[str]</type>
+          <type typedoc="None">None</type>
+          <default>None</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_paths: Iterable[str] | None = None">
+          <name>ignored_paths</name>
+          <type>Iterable[str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_responses: List[int] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_responses: Iterable[int] | None = None">
           <name>ignored_responses</name>
-          <type typedoc="list">List[int]</type>
+          <type>Iterable[int]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_testcases: List[List[str]] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_testcases: Iterable[Tuple[str, str, int]] | None = None">
           <name>ignored_testcases</name>
-          <type typedoc="list">List[List[str]]</type>
+          <type>Iterable[Tuple[str, str, int]]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
           <type typedoc="string">str</type>
           <default/>
@@ -119,24 +125,26 @@
           <name>default_id_property_name</name>
           <type typedoc="string">str</type>
           <default>id</default>
         </arg>
       </arguments>
       <doc>&lt;h4&gt;source&lt;/h4&gt;
 &lt;p&gt;An absolute path to an openapi.json or openapi.yaml file or an url to such a file.&lt;/p&gt;
-&lt;h4&gt;ignored_endpoints&lt;/h4&gt;
-&lt;p&gt;A list of endpoints that will be ignored when generating the test cases.&lt;/p&gt;
+&lt;h4&gt;included_paths&lt;/h4&gt;
+&lt;p&gt;A list of paths that will be included when generating the test cases. The &lt;code&gt;*&lt;/code&gt; character can be used at the end of a partial path to include all paths starting with the partial path (wildcard include).&lt;/p&gt;
+&lt;h4&gt;ignored_paths&lt;/h4&gt;
+&lt;p&gt;A list of paths that will be ignored when generating the test cases. The &lt;code&gt;*&lt;/code&gt; character can be used at the end of a partial path to ignore all paths starting with the partial path (wildcard ignore).&lt;/p&gt;
 &lt;h4&gt;ignored_responses&lt;/h4&gt;
 &lt;p&gt;A list of responses that will be ignored when generating the test cases.&lt;/p&gt;
 &lt;h4&gt;ignored_testcases&lt;/h4&gt;
-&lt;p&gt;A list of specific test cases that, if it would be generated, will be ignored. Specific test cases to ignore must be specified as a &lt;code&gt;List&lt;/code&gt; of &lt;code&gt;endpoint&lt;/code&gt;, &lt;code&gt;method&lt;/code&gt; and &lt;code&gt;response&lt;/code&gt;.&lt;/p&gt;
+&lt;p&gt;A list of specific test cases that, if it would be generated, will be ignored. Specific test cases to ignore must be specified as a &lt;code&gt;Tuple&lt;/code&gt; or &lt;code&gt;List&lt;/code&gt; of &lt;code&gt;path&lt;/code&gt;, &lt;code&gt;method&lt;/code&gt; and &lt;code&gt;response&lt;/code&gt;.&lt;/p&gt;
 &lt;h4&gt;origin&lt;/h4&gt;
 &lt;p&gt;The server (and port) of the target server. E.g. &lt;code&gt;https://localhost:8000&lt;/code&gt;&lt;/p&gt;
 &lt;h4&gt;base_path&lt;/h4&gt;
-&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the endpoints as found in the &lt;code&gt;paths&lt;/code&gt; in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
+&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the paths as found in the &lt;code&gt;paths&lt;/code&gt; in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
 &lt;h4&gt;mappings_path&lt;/h4&gt;
 &lt;p&gt;See &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;
 &lt;h4&gt;username&lt;/h4&gt;
 &lt;p&gt;The username to be used for Basic Authentication.&lt;/p&gt;
 &lt;h4&gt;password&lt;/h4&gt;
 &lt;p&gt;The password to be used for Basic Authentication.&lt;/p&gt;
 &lt;h4&gt;security_token&lt;/h4&gt;
@@ -171,70 +179,70 @@
 &lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entiry) within the API. The default value for this property name is &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
 &lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;span class=&quot;name&quot;&gt;ID_MAPPING&lt;/span&gt; can be implemented in the &lt;span class=&quot;name&quot;&gt;mappings_path&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>=== source === An absolute path to an openapi.json or openapi.yaml file or an url to such a file.</shortdoc>
     </init>
   </inits>
   <keywords>
     <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="148">
-      <arguments repr="endpoint: str, method: str, status_code: int">
-        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
-          <name>endpoint</name>
+      <arguments repr="path: str, method: str, status_code: int">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type typedoc="integer">int</type>
         </arg>
       </arguments>
-      <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
+      <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
-      <shortdoc>Validate that performing the `method` operation on `endpoint` results in a `status_code` response.</shortdoc>
+      <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
     <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="106">
-      <arguments repr="endpoint: str, method: str, expected_status_code: int = 404">
-        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
-          <name>endpoint</name>
+      <arguments repr="path: str, method: str, expected_status_code: int = 404">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="expected_status_code: int = 404">
           <name>expected_status_code</name>
           <type typedoc="integer">int</type>
           <default>404</default>
         </arg>
       </arguments>
-      <doc>&lt;p&gt;Perform a request for the provided 'endpoint' and 'method' where the url for the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; is invalidated.&lt;/p&gt;
-&lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the endpoint contains no parts that can be invalidated.&lt;/p&gt;
+      <doc>&lt;p&gt;Perform a request for the provided 'path' and 'method' where the url for the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; is invalidated.&lt;/p&gt;
+&lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the path contains no parts that can be invalidated.&lt;/p&gt;
 &lt;p&gt;The optional &lt;span class=&quot;name&quot;&gt;expected_status_code&lt;/span&gt; parameter (default: 404) can be set to the expected status code for APIs that do not return a 404 on invalid urls.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: Depending on API design, the url may be validated before or after validation of headers, query parameters and / or (json) body. By default, no parameters are send with the request. The &lt;span class=&quot;name&quot;&gt;require_body_for_invalid_url&lt;/span&gt; parameter can be set to &lt;span class=&quot;name&quot;&gt;True&lt;/span&gt; if needed.&lt;/p&gt;</doc>
-      <shortdoc>Perform a request for the provided 'endpoint' and 'method' where the url for the `endpoint` is invalidated.</shortdoc>
+      <shortdoc>Perform a request for the provided 'path' and 'method' where the url for the `path` is invalidated.</shortdoc>
     </kw>
     <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="86">
-      <arguments repr="endpoint: str, method: str">
-        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
-          <name>endpoint</name>
+      <arguments repr="path: str, method: str">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
-      <doc>&lt;p&gt;Perform a request for &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;, with no authorization.&lt;/p&gt;
+      <doc>&lt;p&gt;Perform a request for &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; on the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt;, with no authorization.&lt;/p&gt;
 &lt;p&gt;This keyword only passes if the response code is 401: Unauthorized.&lt;/p&gt;
 &lt;p&gt;Any authorization parameters used to initialize the library are ignored for this request. &amp;gt; Note: No headers or (json) body are send with the request. For security reasons, the authorization validation should be checked first.&lt;/p&gt;</doc>
-      <shortdoc>Perform a request for `method` on the `endpoint`, with no authorization.</shortdoc>
+      <shortdoc>Perform a request for `method` on the `path`, with no authorization.</shortdoc>
     </kw>
   </keywords>
   <datatypes>
     <enums>
       <enum name="ValidationLevel">
         <doc>&lt;p&gt;The available levels for the response_validation parameter.&lt;/p&gt;</doc>
         <members>
```

### Comparing `robotframework_openapidriver-3.6.2/src/OpenApiDriver/openapidriver.py` & `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 ## OpenAPI (aka Swagger)
 
 The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
 to RESTful APIs, see https://swagger.io/specification/
 
 The OpenApiDriver module implements a reader class that generates a test case for
-each endpoint, method and response that is defined in an OpenAPI document, typically
-an openapi.json or openapi.yaml file.
+each path, method and response (i.e. every response for each endpoint) that is defined
+in an OpenAPI document, typically an openapi.json or openapi.yaml file.
 
 > Note: OpenApiDriver is designed for APIs based on the OAS v3
 The library has not been tested for APIs based on the OAS v2.
 
 ---
 
 ## Getting started
@@ -80,21 +80,21 @@
 *** Settings ***
 Library            OpenApiDriver
 ...                    source=http://localhost:8000/openapi.json
 ...                    origin=http://localhost:8000
 Test Template      Validate Using Test Endpoint Keyword
 
 *** Test Cases ***
-Test Endpoint for ${method} on ${endpoint} where ${status_code} is expected
+Test Endpoint for ${method} on ${path} where ${status_code} is expected
 
 *** Keywords ***
 Validate Using Test Endpoint Keyword
-    [Arguments]    ${endpoint}    ${method}    ${status_code}
+    [Arguments]    ${path}    ${method}    ${status_code}
     Test Endpoint
-    ...    endpoint=${endpoint}    method=${method}    status_code=${status_code}
+    ...    path=${path}    method=${method}    status_code=${status_code}
 
 ```
 
 Running the above suite for the first time is likely to result in some
 errors / failed tests.
 You should look at the Robot Framework `log.html` to determine the reasons
 for the failing tests.
@@ -114,19 +114,19 @@
 ---
 
 ## Limitations
 
 There are currently a number of limitations to supported API structures, supported
 data types and properties. The following list details the most important ones:
 - Only JSON request and response bodies are supported.
-- No support for per-endpoint authorization levels (only simple 401 / 403 validation).
+- No support for per-path authorization levels (only simple 401 / 403 validation).
 
 """
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from DataDriver import DataDriver
 from requests.auth import AuthBase
 from robot.api.deco import library
 
 from OpenApiDriver.openapi_executors import OpenApiExecutors, ValidationLevel
 from OpenApiDriver.openapi_reader import OpenApiReader
@@ -138,17 +138,18 @@
     Visit the [https://github.com/MarketSquare/robotframework-openapidriver | library page]
     for an introduction and examples.
     """
 
     def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
         self,
         source: str,
-        ignored_endpoints: Optional[List[str]] = None,
-        ignored_responses: Optional[List[int]] = None,
-        ignored_testcases: Optional[List[List[str]]] = None,
+        included_paths: Optional[Iterable[str]] = None,
+        ignored_paths: Optional[Iterable[str]] = None,
+        ignored_responses: Optional[Iterable[int]] = None,
+        ignored_testcases: Optional[Iterable[Tuple[str, str, int]]] = None,
         origin: str = "",
         base_path: str = "",
         mappings_path: Union[str, Path] = "",
         username: str = "",
         password: str = "",
         security_token: str = "",
         auth: Optional[AuthBase] = None,
@@ -163,30 +164,37 @@
         faker_locale: Optional[Union[str, List[str]]] = None,
         default_id_property_name: str = "id",
     ):
         """
         === source ===
         An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
 
-        === ignored_endpoints ===
-        A list of endpoints that will be ignored when generating the test cases.
+        === included_paths ===
+        A list of paths that will be included when generating the test cases.
+        The ``*`` character can be used at the end of a partial path to include all paths
+        starting with the partial path (wildcard include).
+
+        === ignored_paths ===
+        A list of paths that will be ignored when generating the test cases.
+        The ``*`` character can be used at the end of a partial path to ignore all paths
+        starting with the partial path (wildcard ignore).
 
         === ignored_responses ===
         A list of responses that will be ignored when generating the test cases.
 
         === ignored_testcases ===
         A list of specific test cases that, if it would be generated, will be ignored.
-        Specific test cases to ignore must be specified as a ``List`` of ``endpoint``,
-        ``method`` and ``response``.
+        Specific test cases to ignore must be specified as a ``Tuple`` or ``List``
+        of ``path``, ``method`` and ``response``.
 
         === origin ===
         The server (and port) of the target server. E.g. ``https://localhost:8000``
 
         === base_path ===
-        The routing between ``origin`` and the endpoints as found in the ``paths`` in the
+        The routing between ``origin`` and the paths as found in the ``paths`` in the
         openapi document. E.g. ``/petshop/v2``.
 
         === mappings_path ===
         See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | here].
 
         === username ===
         The username to be used for Basic Authentication.
@@ -261,17 +269,18 @@
         The default value for this property name is `id`.
         If the target API uses a different name for all the resources within the API,
         you can configure it globally using this property.
 
         If different property names are used for the unique identifier for different
         types of resources, an `ID_MAPPING` can be implemented in the `mappings_path`.
         """
-        ignored_endpoints = ignored_endpoints if ignored_endpoints else []
-        ignored_responses = ignored_responses if ignored_responses else []
-        ignored_testcases = ignored_testcases if ignored_testcases else []
+        included_paths = included_paths if included_paths else ()
+        ignored_paths = ignored_paths if ignored_paths else ()
+        ignored_responses = ignored_responses if ignored_responses else ()
+        ignored_testcases = ignored_testcases if ignored_testcases else ()
 
         mappings_path = Path(mappings_path).as_posix()
         OpenApiExecutors.__init__(
             self,
             source=source,
             origin=origin,
             base_path=base_path,
@@ -288,29 +297,30 @@
             invalid_property_default_response=invalid_property_default_response,
             recursion_limit=recursion_limit,
             recursion_default=recursion_default,
             faker_locale=faker_locale,
             default_id_property_name=default_id_property_name,
         )
 
-        endpoints = self.openapi_spec["paths"]
+        paths = self.openapi_spec["paths"]
         DataDriver.__init__(
             self,
             reader_class=OpenApiReader,
-            endpoints=endpoints,
-            ignored_endpoints=ignored_endpoints,
+            paths=paths,
+            included_paths=included_paths,
+            ignored_paths=ignored_paths,
             ignored_responses=ignored_responses,
             ignored_testcases=ignored_testcases,
         )
 
 
 class DocumentationGenerator(OpenApiDriver):
     __doc__ = OpenApiDriver.__doc__
 
     @staticmethod
-    def get_keyword_names():
+    def get_keyword_names() -> List[str]:
         """Curated keywords for libdoc and libspec."""
         return [
             "test_unauthorized",
             "test_invalid_url",
             "test_endpoint",
         ]  # pragma: no cover
```

### Comparing `robotframework_openapidriver-3.6.2/setup.py` & `robotframework_openapidriver-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 ['OpenApiDriver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['robotframework-datadriver>=1.6.1',
- 'robotframework-openapi-libcore>=1.8.2,<2.0.0']
+ 'robotframework-openapi-libcore>=1.8.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'robotframework-openapidriver',
-    'version': '3.6.2',
+    'version': '4.0.0',
     'description': 'A library for contract-testing OpenAPI / Swagger APIs.',
-    'long_description': '---\n---\n\n# OpenApiDriver for Robot Framework®\n\nOpenApiDriver is an extension of the Robot Framework® DataDriver library that allows\nfor generation and execution of test cases based on the information in an OpenAPI\ndocument (also known as Swagger document).\nThis document explains how to use the OpenApiDriver library.\n\nFor more information about Robot Framework®, see http://robotframework.org.\n\nFor more information about the DataDriver library, see\nhttps://github.com/Snooz82/robotframework-datadriver.\n\n---\n\n> Note: OpenApiDriver is still under development so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapidriver`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiDriver module implements a reader class that generates a test case for\neach endpoint, method and response that is defined in an OpenAPI document, typically\nan openapi.json or openapi.yaml file.\n\n> Note: OpenApiDriver is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use OpenApiDriver to run automatic validations on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiDriver.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source` and `origin` altered to fit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiDriver\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\nTest Template      Validate Using Test Endpoint Keyword\n\n*** Test Cases ***\nTest Endpoint for ${method} on ${endpoint} where ${status_code} is expected\n\n*** Keywords ***\nValidate Using Test Endpoint Keyword\n    [Arguments]    ${endpoint}    ${method}    ${status_code}\n    Test Endpoint\n    ...    endpoint=${endpoint}    method=${method}    status_code=${status_code}\n\n```\n\nRunning the above suite for the first time is likely to result in some\nerrors / failed tests.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiDriver library parameters that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).\n\nThe OpenApiDriver also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels (only simple 401 / 403 validation).\n\n',
+    'long_description': '---\n---\n\n# OpenApiDriver for Robot Framework®\n\nOpenApiDriver is an extension of the Robot Framework® DataDriver library that allows\nfor generation and execution of test cases based on the information in an OpenAPI\ndocument (also known as Swagger document).\nThis document explains how to use the OpenApiDriver library.\n\nFor more information about Robot Framework®, see http://robotframework.org.\n\nFor more information about the DataDriver library, see\nhttps://github.com/Snooz82/robotframework-datadriver.\n\n---\n\n> Note: OpenApiDriver is still under development so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapidriver`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiDriver module implements a reader class that generates a test case for\neach path, method and response (i.e. every response for each endpoint) that is defined\nin an OpenAPI document, typically an openapi.json or openapi.yaml file.\n\n> Note: OpenApiDriver is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use OpenApiDriver to run automatic validations on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiDriver.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source` and `origin` altered to fit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiDriver\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\nTest Template      Validate Using Test Endpoint Keyword\n\n*** Test Cases ***\nTest Endpoint for ${method} on ${path} where ${status_code} is expected\n\n*** Keywords ***\nValidate Using Test Endpoint Keyword\n    [Arguments]    ${path}    ${method}    ${status_code}\n    Test Endpoint\n    ...    path=${path}    method=${method}    status_code=${status_code}\n\n```\n\nRunning the above suite for the first time is likely to result in some\nerrors / failed tests.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiDriver library parameters that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).\n\nThe OpenApiDriver also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-path authorization levels (only simple 401 / 403 validation).\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapidriver',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `robotframework_openapidriver-3.6.2/PKG-INFO` & `robotframework_openapidriver-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapidriver
-Version: 3.6.2
+Version: 4.0.0
 Summary: A library for contract-testing OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapidriver
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Dist: robotframework-datadriver (>=1.6.1)
-Requires-Dist: robotframework-openapi-libcore (>=1.8.2,<2.0.0)
+Requires-Dist: robotframework-openapi-libcore (>=1.8.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 ---
 ---
 
 # OpenApiDriver for Robot Framework®
 
@@ -58,16 +58,16 @@
 
 ## OpenAPI (aka Swagger)
 
 The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
 to RESTful APIs, see https://swagger.io/specification/
 
 The OpenApiDriver module implements a reader class that generates a test case for
-each endpoint, method and response that is defined in an OpenAPI document, typically
-an openapi.json or openapi.yaml file.
+each path, method and response (i.e. every response for each endpoint) that is defined
+in an OpenAPI document, typically an openapi.json or openapi.yaml file.
 
 > Note: OpenApiDriver is designed for APIs based on the OAS v3
 The library has not been tested for APIs based on the OAS v2.
 
 ---
 
 ## Getting started
@@ -109,21 +109,21 @@
 *** Settings ***
 Library            OpenApiDriver
 ...                    source=http://localhost:8000/openapi.json
 ...                    origin=http://localhost:8000
 Test Template      Validate Using Test Endpoint Keyword
 
 *** Test Cases ***
-Test Endpoint for ${method} on ${endpoint} where ${status_code} is expected
+Test Endpoint for ${method} on ${path} where ${status_code} is expected
 
 *** Keywords ***
 Validate Using Test Endpoint Keyword
-    [Arguments]    ${endpoint}    ${method}    ${status_code}
+    [Arguments]    ${path}    ${method}    ${status_code}
     Test Endpoint
-    ...    endpoint=${endpoint}    method=${method}    status_code=${status_code}
+    ...    path=${path}    method=${method}    status_code=${status_code}
 
 ```
 
 Running the above suite for the first time is likely to result in some
 errors / failed tests.
 You should look at the Robot Framework `log.html` to determine the reasons
 for the failing tests.
@@ -143,10 +143,10 @@
 ---
 
 ## Limitations
 
 There are currently a number of limitations to supported API structures, supported
 data types and properties. The following list details the most important ones:
 - Only JSON request and response bodies are supported.
-- No support for per-endpoint authorization levels (only simple 401 / 403 validation).
+- No support for per-path authorization levels (only simple 401 / 403 validation).
```

