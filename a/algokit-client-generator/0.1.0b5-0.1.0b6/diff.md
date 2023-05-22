# Comparing `tmp/algokit_client_generator-0.1.0b5-py3-none-any.whl.zip` & `tmp/algokit_client_generator-0.1.0b6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 15096 bytes, number of entries: 14
+Zip file size: 15669 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2132 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
--rw-r--r--  2.0 unx    22974 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx    23029 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
--rw-r--r--  2.0 unx     5549 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
--rw-r--r--  2.0 unx     3938 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
+-rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
+-rw-r--r--  2.0 unx     4303 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1299 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b5.dist-info/RECORD
-14 files, 46030 bytes uncompressed, 12880 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4585 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1299 b- defN 16-Jan-01 00:00 algokit_client_generator-0.1.0b6.dist-info/RECORD
+14 files, 48367 bytes uncompressed, 13453 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b5.dist-info/LICENSE
+Filename: algokit_client_generator-0.1.0b6.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b5.dist-info/METADATA
+Filename: algokit_client_generator-0.1.0b6.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b5.dist-info/WHEEL
+Filename: algokit_client_generator-0.1.0b6.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b5.dist-info/entry_points.txt
+Filename: algokit_client_generator-0.1.0b6.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-0.1.0b5.dist-info/RECORD
+Filename: algokit_client_generator-0.1.0b6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/generator.py

```diff
@@ -1,16 +1,16 @@
 import dataclasses
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable
 from typing import Literal
 
 from algokit_utils import ApplicationSpecification, OnCompleteActionName
 
 from algokit_client_generator import utils
 from algokit_client_generator.document import DocumentParts, Part
-from algokit_client_generator.spec import ABIContractMethod, ContractMethod, get_contract_methods
+from algokit_client_generator.spec import ABIContractMethod, ABIStruct, ContractMethod, get_contract_methods
 
 ESCAPED_QUOTE = r"\""
 
 
 @dataclasses.dataclass(kw_only=True)
 class GenerationSettings:
     indent: str = "    "
@@ -24,43 +24,45 @@
 class GenerateContext:
     def __init__(self, app_spec: ApplicationSpecification):
         self.app_spec = app_spec
         # TODO: track these as they are emitted?
         self.used_module_symbols = {
             "_APP_SPEC_JSON",
             "APP_SPEC",
-            "_T",
             "_TArgs",
+            "_TArgsHolder",
             "_TResult",
             "_ArgsBase",
-            "_TypedDeployCreateArgs",
-            "_TypedDeployArgs",
             "_as_dict",
+            "_filter_none",
             "_convert_on_complete",
             "_convert_deploy_args",
+            "DeployCreate",
+            "Deploy",
             "GlobalState",
             "LocalState",
         }
         self.used_client_symbols = {
             "__init__",
             "app_spec",
             "app_client",
+            "algod_client",
+            "app_id",
+            "app_address",
+            "sender",
+            "signer",
+            "suggested_params",
             "no_op",
-            "create",
-            "update",
-            "delete",
-            "opt_in",
-            "close_out",
             "clear_state",
             "deploy",
             "get_global_state",
             "get_local_state",
         }
         self.client_name = utils.get_unique_symbol_by_incrementing(
-            self.used_module_symbols, utils.get_class_name(f"{self.app_spec.contract.name}_client")
+            self.used_module_symbols, utils.get_class_name(self.app_spec.contract.name, "client")
         )
         self.methods = get_contract_methods(app_spec, self.used_module_symbols, self.used_client_symbols)
         self.disable_linting = True
         self.settings = GenerationSettings()
 
 
 def generated_comment(context: GenerateContext) -> DocumentParts:
@@ -74,14 +76,15 @@
     yield '# mypy: disable-error-code="no-any-return, no-untyped-call"'  # disable common type warnings
 
 
 def imports(context: GenerateContext) -> DocumentParts:
     yield utils.lines(
         """import base64
 import dataclasses
+import decimal
 import typing
 from abc import ABC, abstractmethod
 
 import algokit_utils
 import algosdk
 from algosdk.atomic_transaction_composer import TransactionSigner, TransactionWithSigner"""
     )
@@ -113,15 +116,14 @@
     yield utils.string_literal(abi.method.get_signature())
     yield Part.DecIndent
     yield Part.DecIndent
     yield Part.RestoreLineMode
 
 
 def helpers(context: GenerateContext) -> DocumentParts:
-    yield '_T = typing.TypeVar("_T")'
     has_abi_create = any(m.abi for m in context.methods.create)
     has_abi_update = any(m.abi for m in context.methods.update_application)
     has_abi_delete = any(m.abi for m in context.methods.delete_application)
     if context.methods.has_abi_methods:
         yield '_TReturn = typing.TypeVar("_TReturn")'
         yield Part.Gap2
         yield utils.indented(
@@ -129,110 +131,142 @@
 class _ArgsBase(ABC, typing.Generic[_TReturn]):
     @staticmethod
     @abstractmethod
     def method() -> str:
         ..."""
         )
     yield Part.Gap2
-    if has_abi_create or has_abi_update or has_abi_delete:
-        yield '_TArgs = typing.TypeVar("_TArgs", bound=_ArgsBase[typing.Any])'
-        yield Part.Gap2
-        yield utils.indented(
-            """
+    yield '_TArgs = typing.TypeVar("_TArgs", bound=_ArgsBase[typing.Any])'
+    yield Part.Gap2
+    yield utils.indented(
+        """
 @dataclasses.dataclass(kw_only=True)
 class _TArgsHolder(typing.Generic[_TArgs]):
     args: _TArgs
 """
-        )
-        yield Part.Gap2
+    )
+    yield Part.Gap2
 
     if has_abi_create:
         yield utils.indented(
             """
 @dataclasses.dataclass(kw_only=True)
-class _TypedDeployCreateArgs(algokit_utils.DeployCreateCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
+class DeployCreate(algokit_utils.DeployCreateCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
     pass
 """
         )
         yield Part.Gap2
     if has_abi_update or has_abi_delete:
         yield utils.indented(
             """
 @dataclasses.dataclass(kw_only=True)
-class _TypedDeployArgs(algokit_utils.DeployCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
+class Deploy(algokit_utils.DeployCallArgs, _TArgsHolder[_TArgs], typing.Generic[_TArgs]):
     pass"""
         )
         yield Part.Gap2
 
     yield Part.Gap2
     yield utils.indented(
         """
-def _as_dict(data: _T | None) -> dict[str, typing.Any]:
+def _filter_none(value: dict | typing.Any) -> dict | typing.Any:
+    if isinstance(value, dict):
+        return {k: _filter_none(v) for k, v in value.items() if v is not None}
+    return value"""
+    )
+    yield Part.Gap2
+    yield utils.indented(
+        """
+def _as_dict(data: typing.Any, *, convert_all: bool = True) -> dict[str, typing.Any]:
     if data is None:
         return {}
     if not dataclasses.is_dataclass(data):
         raise TypeError(f"{data} must be a dataclass")
-    return {f.name: getattr(data, f.name) for f in dataclasses.fields(data) if getattr(data, f.name) is not None}
-"""
+    if convert_all:
+        result = dataclasses.asdict(data)
+    else:
+        result = {f.name: getattr(data, f.name) for f in dataclasses.fields(data)}
+    return _filter_none(result)"""
+    )
+    yield Part.Gap2
+    yield utils.indented(
+        """
+def _convert_transaction_parameters(
+    transaction_parameters: algokit_utils.TransactionParameters | None,
+) -> algokit_utils.CommonCallParametersDict:
+    return typing.cast(algokit_utils.CommonCallParametersDict, _as_dict(transaction_parameters))"""
+    )
+    yield Part.Gap2
+    yield utils.indented(
+        """
+def _convert_call_transaction_parameters(
+    transaction_parameters: algokit_utils.TransactionParameters | None,
+) -> algokit_utils.OnCompleteCallParametersDict:
+    return typing.cast(algokit_utils.OnCompleteCallParametersDict, _as_dict(transaction_parameters))"""
     )
     yield Part.Gap2
     yield utils.indented(
         """
-def _convert_on_complete(on_complete: algokit_utils.OnCompleteActionName) -> algosdk.transaction.OnComplete:
+def _convert_create_transaction_parameters(
+    transaction_parameters: algokit_utils.TransactionParameters | None,
+    on_complete: algokit_utils.OnCompleteActionName,
+) -> algokit_utils.CreateCallParametersDict:
+    result = typing.cast(algokit_utils.CreateCallParametersDict, _as_dict(transaction_parameters))
     on_complete_enum = on_complete.replace("_", " ").title().replace(" ", "") + "OC"
-    return getattr(algosdk.transaction.OnComplete, on_complete_enum)"""
+    result["on_complete"] = getattr(algosdk.transaction.OnComplete, on_complete_enum)
+    return result
+    """
     )
     yield Part.Gap2
     yield utils.indented(
         """
 def _convert_deploy_args(
     deploy_args: algokit_utils.DeployCallArgs | None,
-) -> dict[str, typing.Any] | None:
+) -> algokit_utils.ABICreateCallArgsDict | None:
     if deploy_args is None:
         return None
 
-    deploy_args_dict = _as_dict(deploy_args)
-    if hasattr(deploy_args, "args") and hasattr(deploy_args.args, "method"):
+    deploy_args_dict = typing.cast(algokit_utils.ABICreateCallArgsDict, _as_dict(deploy_args))
+    if isinstance(deploy_args, _TArgsHolder):
         deploy_args_dict["args"] = _as_dict(deploy_args.args)
         deploy_args_dict["method"] = deploy_args.args.method()
 
     return deploy_args_dict"""
     )
     yield Part.Gap2
 
 
+def named_struct(context: GenerateContext, struct: ABIStruct) -> DocumentParts:
+    yield "@dataclasses.dataclass(kw_only=True)"
+    yield f"class {struct.struct_class_name}:"
+    yield Part.IncIndent
+    for field in struct.fields:
+        yield f"{field.name}: {field.python_type}"
+    yield Part.DecIndent
+
+
 def typed_arguments(context: GenerateContext) -> DocumentParts:
     # typed args classes
     processed_abi_signatures: set[str] = set()
+    processed_abi_structs: set[str] = set()
     for method in context.methods.all_abi_methods:
         abi = method.abi
         assert abi
         abi_signature = abi.method.get_signature()
         if abi_signature in processed_abi_signatures:
             continue
+        for struct in abi.structs:
+            if struct.struct_class_name not in processed_abi_structs:
+                yield named_struct(context, struct)
+                yield Part.Gap2
+                processed_abi_structs.add(struct.struct_class_name)
+
         processed_abi_signatures.add(abi_signature)
         yield typed_argument_class(abi)
         yield Part.Gap2
 
-    # typed deploy args
-    for method in context.methods.create:
-        if not method.abi:
-            continue
-        yield f"{method.abi.deploy_create_args_class_name} = _TypedDeployCreateArgs[{method.abi.args_class_name}]"
-
-    processed_abi_signatures.clear()
-    for method in (m for m in context.methods.update_application + context.methods.delete_application if m.abi):
-        abi = method.abi
-        assert abi
-        abi_signature = abi.method.get_signature()
-        if abi_signature in processed_abi_signatures:
-            continue
-        processed_abi_signatures.add(abi_signature)
-        yield f"{abi.deploy_args_class_name} = _TypedDeployArgs[{abi.args_class_name}]"
-
     yield Part.Gap2
 
 
 def state_type(context: GenerateContext, class_name: str, schema: dict[str, dict]) -> DocumentParts:
     if not schema:
         return
 
@@ -350,260 +384,220 @@
             suggested_params=suggested_params,
             template_values=template_values,
             app_name=app_name,
         )"""
     )
     yield Part.Gap1
     yield Part.IncIndent
+    yield forwarded_client_properties(context)
+    yield Part.Gap1
     yield get_global_state_method(context)
     yield Part.Gap1
     yield get_local_state_method(context)
     yield Part.Gap1
-    yield call_methods(context)
+    yield methods_by_side_effect(context, "none", context.methods.no_op)
     yield Part.Gap1
-    yield special_method(context, "create", context.methods.create)
+    yield methods_by_side_effect(context, "create", context.methods.create)
     yield Part.Gap1
-    yield special_method(context, "update", context.methods.update_application)
+    yield methods_by_side_effect(context, "update", context.methods.update_application)
     yield Part.Gap1
-    yield special_method(context, "delete", context.methods.delete_application)
+    yield methods_by_side_effect(context, "delete", context.methods.delete_application)
     yield Part.Gap1
-    yield special_method(context, "opt_in", context.methods.opt_in)
+    yield methods_by_side_effect(context, "opt_in", context.methods.opt_in)
     yield Part.Gap1
-    yield special_method(context, "close_out", context.methods.close_out)
+    yield methods_by_side_effect(context, "close_out", context.methods.close_out)
     yield Part.Gap1
     yield clear_method(context)
     yield Part.Gap1
     yield deploy_method(context)
 
 
+def forwarded_client_properties(context: GenerateContext) -> DocumentParts:
+    yield utils.indented(
+        """
+@property
+def algod_client(self) -> algosdk.v2client.algod.AlgodClient:
+    return self.app_client.algod_client
+
+@property
+def app_id(self) -> int:
+    return self.app_client.app_id
+
+@app_id.setter
+def app_id(self, value: int) -> None:
+    self.app_client.app_id = value
+
+@property
+def app_address(self) -> str:
+    return self.app_client.app_address
+
+@property
+def sender(self) -> str | None:
+    return self.app_client.sender
+
+@sender.setter
+def sender(self, value: str) -> None:
+    self.app_client.sender = value
+
+@property
+def signer(self) -> TransactionSigner | None:
+    return self.app_client.signer
+
+@signer.setter
+def signer(self, value: TransactionSigner) -> None:
+    self.app_client.signer = value
+
+@property
+def suggested_params(self) -> algosdk.transaction.SuggestedParams | None:
+    return self.app_client.suggested_params
+
+@suggested_params.setter
+def suggested_params(self, value: algosdk.transaction.SuggestedParams | None) -> None:
+    self.app_client.suggested_params = value"""
+    )
+
+
 def embed_app_spec(context: GenerateContext) -> DocumentParts:
     yield Part.InlineMode
     yield '_APP_SPEC_JSON = r"""'
     yield context.app_spec.to_json()
     yield '"""'
     yield Part.RestoreLineMode
     yield "APP_SPEC = algokit_utils.ApplicationSpecification.from_json(_APP_SPEC_JSON)"
 
 
-def call_method(context: GenerateContext, contract_method: ABIContractMethod) -> DocumentParts:
-    yield f"def {contract_method.client_method_name}("
+def signature(context: GenerateContext, name: str, method: ContractMethod) -> DocumentParts:
+    yield f"def {name}("
     yield Part.IncIndent
     yield "self,"
     yield "*,"
-    for arg in contract_method.args:
-        yield Part.InlineMode
-        yield f"{arg.name}: {arg.python_type}"
-        if arg.has_default:
-            yield " | None = None"
-        yield ","
-        yield Part.RestoreLineMode
-    yield "transaction_parameters: algokit_utils.TransactionParameters | None = None,"
+    abi = method.abi
+    if abi:
+        for arg in abi.args:
+            if arg.has_default:
+                yield f"{arg.name}: {arg.python_type} | None = None,"
+            else:
+                yield f"{arg.name}: {arg.python_type},"
+    if method.call_config == "create":
+        yield on_complete_literals(method.on_complete)
+        yield "transaction_parameters: algokit_utils.CreateTransactionParameters | None = None,"
+    else:
+        yield "transaction_parameters: algokit_utils.TransactionParameters | None = None,"
     yield Part.DecIndent
-    yield f") -> algokit_utils.ABITransactionResponse[{contract_method.python_type}]:"
-    yield Part.IncIndent
-    # TODO: yield doc
+    if abi:
+        yield f") -> algokit_utils.ABITransactionResponse[{abi.python_type}]:"
+    else:
+        yield ") -> algokit_utils.TransactionResponse:"
+    # TODO: docstring
+
 
-    if not contract_method.args:
+def instantiate_args(contract_method: ABIContractMethod | None) -> DocumentParts:
+    if contract_method and not contract_method.args:
         yield f"args = {contract_method.args_class_name}()"
-    else:
+    elif contract_method:
         yield f"args = {contract_method.args_class_name}(", Part.IncIndent
         for arg in contract_method.args:
             yield f"{arg.name}={arg.name},"
         yield Part.DecIndent, ")"
 
-    yield utils.indented(
-        """
-return self.app_client.call(
-    call_abi_method=args.method(),
-    transaction_parameters=_as_dict(transaction_parameters),
-    **_as_dict(args),
-)"""
-    )
-    yield Part.DecIndent
 
-
-def call_methods(context: GenerateContext) -> DocumentParts:
-    for method in context.methods.no_op:
-        if method.abi:
-            yield call_method(context, method.abi)
-        else:
-            yield utils.indented(
-                """
-def no_op(
-    self,
-    transaction_parameters: algokit_utils.TransactionParameters | None = None
-) -> algokit_utils.TransactionResponse:
-    return self.app_client.call(
-        call_abi_method=False,
-        transaction_parameters=_as_dict(transaction_parameters),
-    )"""
-            )
-        yield Part.Gap1
-
-
-def signature(
-    context: GenerateContext, name: str, args: "Sequence[str | DocumentParts]", return_types: list[str]
+def app_client_call(
+    app_client_method: Literal["call", "create", "update", "delete", "opt_in", "close_out"],
+    contract_method: ContractMethod,
 ) -> DocumentParts:
-    yield f"def {name}("
+    yield f"result = self.app_client.{app_client_method}("
     yield Part.IncIndent
-    for arg in args:
-        yield Part.InlineMode
-        if isinstance(arg, str):
-            yield arg
-        else:
-            yield arg
-        yield ","
-        yield Part.RestoreLineMode
-
-    return_signature = f") -> {' | '.join(return_types)}:"
-
-    if context.settings.indent_length + len(return_signature) < context.settings.max_line_length:
-        yield Part.DecIndent, return_signature
+    if contract_method.abi:
+        yield "call_abi_method=args.method(),"
     else:
-        yield Part.DecIndent, ") -> ("
-        yield Part.IncIndent
-        for idx, return_type in enumerate(return_types):
-            yield Part.InlineMode
-            if idx:
-                yield "| "
-            yield return_type
-            yield Part.RestoreLineMode
-        yield Part.DecIndent, "):"
+        yield "call_abi_method=False,"
+    if contract_method.call_config == "create":
+        yield "transaction_parameters=_convert_create_transaction_parameters(transaction_parameters, on_complete),"
+    elif "no_op" in contract_method.on_complete:
+        yield "transaction_parameters=_convert_call_transaction_parameters(transaction_parameters),"
+    else:
+        yield "transaction_parameters=_convert_transaction_parameters(transaction_parameters),"
+    if contract_method.abi:
+        yield "**_as_dict(args, convert_all=True),"
+    yield Part.DecIndent
+    yield ")"
+    if contract_method.abi and contract_method.abi.result_struct:
+        yield 'elements = self.app_spec.hints[args.method()].structs["output"]["elements"]'
+        yield "result_dict = {element[0]: value for element, value in zip(elements, result.return_value)}"
+        yield f"result.return_value = {contract_method.abi.python_type}(**result_dict)"
+    yield "return result"
 
 
 def on_complete_literals(on_completes: Iterable[OnCompleteActionName]) -> DocumentParts:
     yield Part.InlineMode
     yield 'on_complete: typing.Literal["'
     yield utils.join('", "', on_completes)
     yield '"]'
     if "no_op" in on_completes:
         yield ' = "no_op"'
+    yield ","
     yield Part.RestoreLineMode
 
 
-def multi_typed_arg(arg_name: str, arg_types: list[str], *, include_none_default: bool) -> DocumentParts:
-    yield Part.InlineMode
-    yield f"{arg_name}: "
-    yield utils.join(" | ", arg_types)
-    if include_none_default:
-        yield " = None"
-    yield Part.RestoreLineMode
-
-
-def special_typed_args(methods: list[ContractMethod]) -> DocumentParts:
-    has_bare = any(not m.abi for m in methods)
-    args = [m.abi.args_class_name for m in methods if m.abi]
-    if has_bare:
-        args.append("None")
-    yield multi_typed_arg("args", args, include_none_default=has_bare)
-
-
-def special_overload(
-    context: GenerateContext,
-    method_name: Literal["create", "update", "delete", "opt_in", "close_out"],
-    method: ContractMethod,
-) -> DocumentParts:
-    yield "@typing.overload"
-    args: list[str | DocumentParts] = ["self", "*"]
-
-    if method.abi:
-        args.append(f"args: {method.abi.args_class_name}")
-        return_type = f"algokit_utils.ABITransactionResponse[{method.abi.python_type}]"
-    else:
-        args.append("args: typing.Literal[None] = None")
-        return_type = "algokit_utils.TransactionResponse"
-    if method_name == "create":
-        args.append(on_complete_literals(method.on_complete))
-        args.append("transaction_parameters: algokit_utils.CreateTransactionParameters | None = None")
-    else:
-        args.append("transaction_parameters: algokit_utils.TransactionParameters | None = None")
-    yield signature(context, method_name, args, [return_type])
-    yield Part.IncIndent, "...", Part.DecIndent
-
-
-def special_method(
+def methods_by_side_effect(
     context: GenerateContext,
-    method_name: Literal["create", "update", "delete", "opt_in", "close_out"],
+    side_effect: Literal["none", "create", "update", "delete", "opt_in", "close_out"],
     methods: list[ContractMethod],
 ) -> DocumentParts:
     if not methods:
         return
-    is_create = method_name == "create"
-    has_bare = any(not m.abi for m in methods)
-    bare_only = all(not m.abi for m in methods)
-    # typed overloads
-    if len(methods) > 1:
-        for method in methods:
-            yield special_overload(context, method_name, method)
-            yield Part.Gap1
-
-    # signature
-    args: list[str | DocumentParts] = ["self", "*"]
-    if not bare_only:
-        args.append(special_typed_args(methods))
-    if is_create:
-        args.append(on_complete_literals(sorted({c for m in methods for c in m.on_complete})))
-        args.append("transaction_parameters: algokit_utils.CreateTransactionParameters | None = None")
-    else:
-        args.append("transaction_parameters: algokit_utils.TransactionParameters | None = None")
 
-    return_types = []
-    if has_bare:
-        return_types.append("algokit_utils.TransactionResponse")
-
-    return_types.extend(sorted(f"algokit_utils.ABITransactionResponse[{m.abi.python_type}]" for m in methods if m.abi))
-    yield signature(context, method_name, args, return_types)
-
-    # implementation
-    yield Part.IncIndent
+    for method in methods:
+        contract_method = method.abi
 
-    yield f"return self.app_client.{method_name}("
-    yield Part.IncIndent
-    if bare_only:
-        yield "call_abi_method=False,"
-    else:
-        yield "call_abi_method=args.method() if args else False,"
-    if is_create:
-        yield (
-            "transaction_parameters=_as_dict(transaction_parameters) | "
-            '{"on_complete": _convert_on_complete(on_complete)},'
-        )
-    else:
-        yield "transaction_parameters=_as_dict(transaction_parameters),"
-    if not bare_only:
-        yield "**_as_dict(args),"
-    yield Part.DecIndent
-    yield ")"
-    yield Part.DecIndent
+        if side_effect == "none":
+            if contract_method:  # an ABI method with no_op=CALL method
+                full_method_name = contract_method.client_method_name
+            else:
+                full_method_name = "no_op"
+        elif contract_method:  # an ABI method with a side effect
+            full_method_name = f"{side_effect}_{contract_method.client_method_name}"
+        else:  # a bare method
+            full_method_name = f"{side_effect}_bare"
+        yield signature(context, full_method_name, method)
+        yield Part.IncIndent
+        yield instantiate_args(contract_method)
+        yield app_client_call("call" if side_effect == "none" else side_effect, method)
+        yield Part.DecIndent
+        yield Part.Gap1
 
 
 def clear_method(context: GenerateContext) -> DocumentParts:
     yield utils.indented(
         """
 def clear_state(
     self,
     transaction_parameters: algokit_utils.TransactionParameters | None = None,
     app_args: list[bytes] | None = None,
 ) -> algokit_utils.TransactionResponse:
-    return self.app_client.clear_state(_as_dict(transaction_parameters), app_args)"""
+    return self.app_client.clear_state(_convert_transaction_parameters(transaction_parameters), app_args)"""
     )
 
 
 def deploy_method_args(context: GenerateContext, arg_name: str, methods: list[ContractMethod]) -> DocumentParts:
     yield Part.InlineMode
     has_bare = any(not m.abi for m in methods) or not methods
-    args = [
-        m.abi.deploy_create_args_class_name if m.call_config == "create" else m.abi.deploy_args_class_name
-        for m in methods
-        if m.abi
-    ]
+    typed_args = [m.abi.args_class_name for m in methods if m.abi]
+    args = []
+    if typed_args:
+        deploy_type = "DeployCreate" if arg_name == "create_args" else "Deploy"
+        args.append(f"{deploy_type}[{' | '.join(typed_args)}]")
     if has_bare:
         args.append("algokit_utils.DeployCallArgs")
         args.append("None")
-    yield multi_typed_arg(arg_name, args, include_none_default=has_bare)
+
+    yield f"{arg_name}: "
+    yield utils.join(" | ", args)
+    if has_bare:
+        yield " = None"
     yield ","
     yield Part.RestoreLineMode
 
 
 def deploy_method(context: GenerateContext) -> DocumentParts:
     yield utils.indented(
         """
@@ -644,27 +638,25 @@
 
 
 def get_global_state_method(context: GenerateContext) -> DocumentParts:
     if not context.app_spec.schema.get("global", {}).get("declared", {}):
         return
     yield "def get_global_state(self) -> GlobalState:"
     yield Part.IncIndent
-    # TODO: what if the key can't be decoded to utf8
-    yield "state = self.app_client.get_global_state(raw=True)"
+    yield "state = typing.cast(dict[bytes, bytes | int], self.app_client.get_global_state(raw=True))"
     yield "return GlobalState(state)"
     yield Part.DecIndent
 
 
 def get_local_state_method(context: GenerateContext) -> DocumentParts:
     if not context.app_spec.schema.get("local", {}).get("declared", {}):
         return
     yield "def get_local_state(self, account: str | None = None) -> LocalState:"
     yield Part.IncIndent
-    # TODO: what if the key can't be decoded to utf8
-    yield "state = self.app_client.get_local_state(account, raw=True)"
+    yield "state = typing.cast(dict[bytes, bytes | int], self.app_client.get_local_state(account, raw=True))"
     yield "return LocalState(state)"
     yield Part.DecIndent
 
 
 def generate(context: GenerateContext) -> DocumentParts:
     if context.disable_linting:
         yield disable_linting(context)
```

## algokit_client_generator/spec.py

```diff
@@ -14,20 +14,36 @@
     abi_type: str
     python_type: str
     desc: str | None
     has_default: bool = False
 
 
 @dataclasses.dataclass(kw_only=True)
+class ABIStructField:
+    name: str
+    abi_type: str
+    python_type: str
+
+
+@dataclasses.dataclass(kw_only=True)
+class ABIStruct:
+    abi_name: str
+    struct_class_name: str
+    fields: list[ABIStructField]
+
+
+@dataclasses.dataclass(kw_only=True)
 class ABIContractMethod:
     method: Method
     hints: MethodHints
     abi_type: str
     python_type: str
+    result_struct: ABIStruct | None
     args: list[ContractArg]
+    structs: list[ABIStruct]
     args_class_name: str
     client_method_name: str
     deploy_args_class_name: str
     deploy_create_args_class_name: str
 
 
 @dataclasses.dataclass(kw_only=True)
@@ -109,47 +125,79 @@
 
 def get_contract_methods(
     app_spec: ApplicationSpecification, used_module_symbols: set[str], used_client_symbols: set[str]
 ) -> ContractMethods:
     result = ContractMethods()
     result.add_method(None, app_spec.bare_call_config)
 
+    structs: dict[str, ABIStruct] = {}
     for methods in group_by_overloads(app_spec.contract.methods):
         naming_strategy = find_naming_strategy(methods)
         for method in methods:
             method_name = naming_strategy(method)
             hints = app_spec.hints[method.get_signature()]
             args_class_name = utils.get_unique_symbol_by_incrementing(
                 used_module_symbols,
-                utils.get_class_name(f"{method_name}_args"),
+                utils.get_class_name(method_name, "args"),
             )
+
+            parameter_type_map: dict[str, str] = {}
+            method_structs: list[ABIStruct] = []
+            result_struct: ABIStruct | None = None
+            for parameter, struct in hints.structs.items():
+                abi_name = struct["name"]
+                abi_struct = structs.get(abi_name)
+                if not abi_struct:
+                    # TODO: check for collisions where the same name refers to different structures
+                    struct_class_name = utils.get_unique_symbol_by_incrementing(
+                        used_module_symbols, utils.get_class_name(abi_name)
+                    )
+                    abi_struct = ABIStruct(
+                        abi_name=abi_name,
+                        struct_class_name=struct_class_name,
+                        fields=[
+                            ABIStructField(
+                                name=name,
+                                abi_type=abi_type,
+                                python_type=utils.map_abi_type_to_python(abi_type),
+                            )
+                            # TODO: nested structs?!
+                            for name, abi_type in struct["elements"]
+                        ],
+                    )
+                structs[abi_name] = abi_struct
+                if parameter == "output":  # TODO: check return signature
+                    result_struct = abi_struct
+                parameter_type_map[parameter] = abi_struct.struct_class_name
+                method_structs.append(abi_struct)
+
             abi = ABIContractMethod(
                 method=method,
                 hints=hints,
                 abi_type=str(method.returns),
-                python_type=utils.map_abi_type_to_python(str(method.returns)),
+                python_type=result_struct.struct_class_name
+                if result_struct
+                else utils.map_abi_type_to_python(str(method.returns)),
+                result_struct=result_struct,
+                structs=method_structs,
                 args=[
                     ContractArg(
                         name=arg.name or f"arg{idx}",
                         abi_type=str(arg.type),
-                        python_type=utils.map_abi_type_to_python(str(arg.type)),
+                        python_type=parameter_type_map[arg.name]
+                        if arg.name in parameter_type_map
+                        else utils.map_abi_type_to_python(str(arg.type)),
                         desc=arg.desc,
                         has_default=arg.name in hints.default_arguments,
                     )
                     for idx, arg in enumerate(method.args)
                 ],
                 args_class_name=args_class_name,
-                deploy_args_class_name=utils.get_unique_symbol_by_incrementing(
-                    used_module_symbols,
-                    f"Deploy_{args_class_name}",
-                ),
-                deploy_create_args_class_name=utils.get_unique_symbol_by_incrementing(
-                    used_module_symbols,
-                    f"DeployCreate_{args_class_name}",
-                ),
+                deploy_args_class_name=f"Deploy[{args_class_name}]",
+                deploy_create_args_class_name=f"DeployCreate[{args_class_name}]",
                 client_method_name=utils.get_unique_symbol_by_incrementing(
                     used_client_symbols, utils.get_method_name(method_name)
                 ),
             )
             result.add_method(abi, hints.call_config)
 
     return result
```

## algokit_client_generator/utils.py

```diff
@@ -1,67 +1,73 @@
 import re
 from collections.abc import Iterable
 
+from algosdk import abi
+
 from algokit_client_generator.document import DocumentParts, Part
 
 
 def get_parts(value: str) -> list[str]:
     """Splits value into a list of words, with boundaries at _, and transitions between casing"""
     return re.findall("[A-Z][a-z]+|[0-9A-Z]+(?=[A-Z][a-z])|[0-9A-Z]{2,}|[a-z0-9]{2,}|[a-zA-Z0-9]", value)
 
 
 def get_class_name(name: str, string_suffix: str = "") -> str:
     parts = [p.title() for p in get_parts(name)]
     if string_suffix:
-        parts.append(string_suffix)
+        parts.append(string_suffix.title())
     return "".join(p for p in parts)
 
 
 def get_method_name(name: str, string_suffix: str = "") -> str:
     parts = [p.lower() for p in get_parts(name)]
     if string_suffix:
-        parts.append(string_suffix)
+        parts.append(string_suffix.lower())
     return "_".join(p for p in parts)
 
 
-def map_abi_type_to_python(abi_type: str) -> str:  # noqa: ignore[PLR0911]
-    match = re.match(r".*\[([0-9]*)]$", abi_type)
-    if match:
-        array_size = match.group(1)
-        if array_size:
-            abi_type = abi_type[: -2 - len(array_size)]
-            array_size = int(array_size)
-            inner_type = ", ".join([map_abi_type_to_python(abi_type)] * array_size)
-            tuple_type = f"tuple[{inner_type}]"
-            if abi_type == "byte":
-                return f"bytes | {tuple_type}"
-            return tuple_type
-        else:
-            abi_type = abi_type[:-2]
-            if abi_type == "byte":
-                return "bytes"
-            return f"list[{map_abi_type_to_python(abi_type)}]"
-    if abi_type.startswith("(") and abi_type.endswith(")"):
-        abi_type = abi_type[1:-1]
-        inner_types = [map_abi_type_to_python(t) for t in abi_type.split(",")]
-        return f"tuple[{', '.join(inner_types)}]"
-    # TODO validate or annotate ints
-    python_type = {
-        "string": "str",
-        "uint8": "int",  # < 256
-        "uint32": "int",  # < 2^32
-        "uint64": "int",  # < 2^64
-        "void": "None",
-        "byte[]": "bytes",
-        "byte": "int",  # length 1
-        "pay": "TransactionWithSigner",
-    }.get(abi_type)
-    if python_type:
-        return python_type
-    return abi_type
+def abi_type_to_python(abi_type: abi.ABIType) -> str:  # noqa: ignore[PLR0911]
+    match abi_type:
+        case abi.UintType():
+            return "int"
+        case abi.ArrayDynamicType() as array:
+            child = array.child_type
+            if isinstance(child, abi.ByteType):
+                return "bytes | bytearray"
+            return f"list[{abi_type_to_python(child)}]"
+        case abi.ArrayStaticType() as array:
+            child = array.child_type
+            if isinstance(child, abi.ByteType):
+                return f"bytes | bytearray | tuple[{', '.join('int' for _ in range(array.static_length))}]"
+            inner_type = abi_type_to_python(child)
+            return f"list[{inner_type}] | tuple[{', '.join(inner_type for _ in range(array.static_length))}]"
+        case abi.AddressType():
+            return "str"
+        case abi.BoolType():
+            return "bool"
+        case abi.UfixedType():
+            return "decimal.Decimal"
+        case abi.TupleType() as tuple_type:
+            return f"tuple[{', '.join(abi_type_to_python(t) for t in tuple_type.child_types)}]"
+        case abi.ByteType():
+            return "int"
+        case abi.StringType():
+            return "str"
+        case _:
+            return "typing.Any"
+
+
+def map_abi_type_to_python(abi_type_str: str) -> str:
+    if abi_type_str == "void":
+        return "None"
+    if abi.is_abi_transaction_type(abi_type_str):
+        # TODO: generic TransactionWithSigner and/or allow unsigned types signed with signer used in transaction
+        return "TransactionWithSigner"
+    abi_type = abi.ABIType.from_string(abi_type_str)
+    return abi_type_to_python(abi_type)
 
 
 def get_unique_symbol_by_incrementing(existing_symbols: set[str], base_name: str) -> str:
     suffix = 0
     while True:
         suffix_str = str(suffix) if suffix else ""
         symbol = base_name + suffix_str
```

## Comparing `algokit_client_generator-0.1.0b5.dist-info/LICENSE` & `algokit_client_generator-0.1.0b6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-0.1.0b5.dist-info/METADATA` & `algokit_client_generator-0.1.0b6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_client_generator-0.1.0b5.dist-info/RECORD` & `algokit_client_generator-0.1.0b6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_client_generator/__init__.py,sha256=KHVr3rMTN2T146gjOpaF3fc5cqoLoVs01ueXn-p9QHI,179
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
 algokit_client_generator/cli.py,sha256=S9YxyLIpzDvSGLbxP7QJz8b-otpzX-lgHRJzvEzFC6Q,2132
 algokit_client_generator/document.py,sha256=X4xMvu_LfDcaosEy3AtjRoXpiLZoXRVCIoPNo8b-h08,3199
-algokit_client_generator/generator.py,sha256=PaNn4f0PfnWr0unmrU--I_OA-ERv9GY8xcQbejCno0Y,22974
+algokit_client_generator/generator.py,sha256=WlnxNObfumcp2R3cu0FqrBHQNfC1TiGwDLTBxNPfv7w,23029
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_client_generator/spec.py,sha256=wa4sHpbDRk7UQJsUDMdJ6NP8CCKiqBazbPrQg9khzjw,5549
-algokit_client_generator/utils.py,sha256=omhCEOXmxc523oiOcM6TL0IpbR6MqdM5Sy-o3o9VQTw,3938
+algokit_client_generator/spec.py,sha256=apgef1qcRbm2akT1ogF23d6HnSncPwnLdrqaVzJAKmo,7466
+algokit_client_generator/utils.py,sha256=LQ3wXw_1IlnkKKNzDetIbAIBqEgYrRRjI6Bu_42Yzpc,4303
 algokit_client_generator/writer.py,sha256=MF46CQ8q1nW-K66RcKcXYE1uArrNRKHWF-uKQT8eziU,890
-algokit_client_generator-0.1.0b5.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-0.1.0b5.dist-info/METADATA,sha256=lKUyLA1aAOkukiz0kpVPjvHA-86-6UMccWeWSUyp4AA,4585
-algokit_client_generator-0.1.0b5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_client_generator-0.1.0b5.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-0.1.0b5.dist-info/RECORD,,
+algokit_client_generator-0.1.0b6.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-0.1.0b6.dist-info/METADATA,sha256=DHw5TK0OeJjk4NTPcqNpsm9BPJD4vw_b1nY4LL0toWA,4585
+algokit_client_generator-0.1.0b6.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_client_generator-0.1.0b6.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-0.1.0b6.dist-info/RECORD,,
```

