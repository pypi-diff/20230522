# Comparing `tmp/mlogevo-0.0.8-py3-none-any.whl.zip` & `tmp/mlogevo-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 34913 bytes, number of entries: 36
+Zip file size: 35687 bytes, number of entries: 36
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-18 01:52 mlogevo/__init__.py
 -rw-r--r--  2.0 unx     3596 b- defN 22-Nov-26 01:38 mlogevo/__main__.py
 -rw-r--r--  2.0 unx       73 b- defN 22-Nov-20 02:30 mlogevo/backend/__init__.py
 -rw-r--r--  2.0 unx      787 b- defN 22-Nov-23 11:42 mlogevo/backend/asm_template.py
--rw-r--r--  2.0 unx     5527 b- defN 22-Dec-27 07:45 mlogevo/backend/backend.py
+-rw-r--r--  2.0 unx     5138 b- defN 22-Dec-29 12:38 mlogevo/backend/backend.py
 -rw-r--r--  2.0 unx     2533 b- defN 22-Nov-23 08:47 mlogevo/backend/basic_block.py
--rw-r--r--  2.0 unx     2681 b- defN 22-Nov-20 10:53 mlogevo/backend/inline_utils.py
+-rw-r--r--  2.0 unx     4422 b- defN 22-Dec-27 13:11 mlogevo/backend/inline_utils.py
 -rw-r--r--  2.0 unx       79 b- defN 22-Nov-26 01:23 mlogevo/frontend/__init__.py
 -rw-r--r--  2.0 unx      184 b- defN 22-Nov-26 01:33 mlogevo/frontend/compilation_error.py
--rw-r--r--  2.0 unx    27743 b- defN 22-Dec-21 05:18 mlogevo/frontend/compiler.py
+-rw-r--r--  2.0 unx    29104 b- defN 23-Jan-15 02:40 mlogevo/frontend/compiler.py
 -rw-r--r--  2.0 unx      985 b- defN 22-Dec-19 06:11 mlogevo/frontend/mlog_object.py
--rw-r--r--  2.0 unx      960 b- defN 22-Oct-07 13:25 mlogevo/frontend/parent_node_visitor.py
--rw-r--r--  2.0 unx     3486 b- defN 22-Dec-21 06:55 mlogevo/frontend/type_util.py
+-rw-r--r--  2.0 unx     1031 b- defN 22-Dec-29 12:58 mlogevo/frontend/parent_node_visitor.py
+-rw-r--r--  2.0 unx     3541 b- defN 23-Jan-09 09:29 mlogevo/frontend/type_util.py
 -rw-r--r--  2.0 unx      214 b- defN 22-Sep-27 02:50 mlogevo/intermediate/__init__.py
 -rw-r--r--  2.0 unx      429 b- defN 22-Nov-16 03:55 mlogevo/intermediate/function.py
--rw-r--r--  2.0 unx     4255 b- defN 22-Dec-17 08:25 mlogevo/intermediate/ir_quadruple.py
+-rw-r--r--  2.0 unx     4358 b- defN 22-Dec-27 12:37 mlogevo/intermediate/ir_quadruple.py
 -rw-r--r--  2.0 unx     2845 b- defN 22-Nov-23 08:46 mlogevo/intermediate/quadruple_from_text.py
 -rw-r--r--  2.0 unx     2182 b- defN 22-Dec-27 08:01 mlogevo/optimizer/__init__.py
 -rw-r--r--  2.0 unx      741 b- defN 22-Nov-01 09:50 mlogevo/optimizer/mi_deduplicate_tail_return.py
--rw-r--r--  2.0 unx    18637 b- defN 22-Dec-27 09:04 mlogevo/optimizer/mi_lcse.py
+-rw-r--r--  2.0 unx    18637 b- defN 22-Dec-27 09:30 mlogevo/optimizer/mi_lcse.py
 -rw-r--r--  2.0 unx      928 b- defN 22-Dec-17 12:44 mlogevo/optimizer/mi_remove_unused_decls.py
 -rw-r--r--  2.0 unx      890 b- defN 22-Nov-01 09:50 mlogevo/optimizer/mi_remove_unused_labels.py
--rw-r--r--  2.0 unx     1667 b- defN 22-Dec-27 08:06 mlogevo/optimizer/mi_remove_unused_variables.py
+-rw-r--r--  2.0 unx     1815 b- defN 23-Jan-15 02:23 mlogevo/optimizer/mi_remove_unused_variables.py
 -rw-r--r--  2.0 unx      654 b- defN 22-Dec-06 15:43 mlogevo/optimizer/mi_reorder_decls.py
 -rw-r--r--  2.0 unx     1120 b- defN 22-Nov-30 02:16 mlogevo/optimizer/optimizer_registry.py
 -rw-r--r--  2.0 unx       55 b- defN 22-Nov-15 07:25 mlogevo/output/__init__.py
 -rw-r--r--  2.0 unx      172 b- defN 22-Nov-15 07:25 mlogevo/output/abstract_ir_converter.py
 -rw-r--r--  2.0 unx      338 b- defN 22-Nov-15 07:25 mlogevo/output/ir_output.py
 -rw-r--r--  2.0 unx     5718 b- defN 22-Dec-17 13:11 mlogevo/output/mlog_instructions.py
 -rw-r--r--  2.0 unx     2930 b- defN 22-Nov-23 09:01 mlogevo/output/mlog_output.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4626 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3159 b- defN 22-Dec-27 09:07 mlogevo-0.0.8.dist-info/RECORD
-36 files, 101412 bytes uncompressed, 29781 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4626 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3160 b- defN 23-Jan-15 02:41 mlogevo-0.0.9.dist-info/RECORD
+36 files, 104503 bytes uncompressed, 30555 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -84,26 +84,26 @@
 
 Filename: mlogevo/output/mlog_instructions.py
 Comment: 
 
 Filename: mlogevo/output/mlog_output.py
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/LICENSE
+Filename: mlogevo-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/METADATA
+Filename: mlogevo-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/WHEEL
+Filename: mlogevo-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/entry_points.txt
+Filename: mlogevo-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/top_level.txt
+Filename: mlogevo-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mlogevo-0.0.8.dist-info/RECORD
+Filename: mlogevo-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlogevo/backend/backend.py

```diff
@@ -32,31 +32,18 @@
             continue
         if ir.instruction in COMPARISONS:
             result[ir.dest] = "i32"
         tokens = ir.instruction.split("_")
         result[ir.dest] = tokens[-1]
 
 
-def read_referred_temp_vars(ir_list: Iterable[Quadruple]) -> Set[str]:
-    def is_temp_variable(name: str):
-        return name.startswith("___vtmp_") or name.startswith("__vtmp_")
-
-    temp_variables = set()
-    for ir in ir_list:
-        if is_temp_variable(ir.src1):
-            temp_variables.add(ir.src1)
-        if is_temp_variable(ir.src2):
-            temp_variables.add(ir.src2)
-        for var in filter(is_temp_variable, ir.input_vars):
-            temp_variables.add(var)
-    return temp_variables
-
-
 class Backend:
-    def __init__(self):
+    def __init__(self, arch, target):
+        self.arch = arch
+        self.target = target
         # function_optimizers: work on the whole function
         self.mi_optimizers = []
         self.asm_template_handler = None
         self.output_component: AbstractIRConverter = None
 
     def compile(self, frontend_result, dump_blocks=False) -> str:
         variable_types: Dict[str, str] = {}
@@ -69,21 +56,22 @@
         for function in inline_functions.values():
             self.run_optimize_pass(function, all_functions, variable_types, dump_blocks)
         for function in common_functions.values():
             function.instructions = inline_calls(function.name, function.instructions, inline_functions)
             self.run_optimize_pass(function, all_functions, variable_types, dump_blocks)
 
         ir_list = inits[:]
+        # make main() the first function
         if "main" in common_functions.keys():
             ir_list += common_functions["main"].instructions
-        # make main() the first function
         for (name, body) in common_functions.items():
             if name == "main": continue
             ir_list.extend(body.instructions)
-        self.convert_asm(ir_list)
+        if self.target != "mlogev_ir":
+            self.convert_asm(ir_list)
         return self.output_component.convert(ir_list)
 
     def run_optimize_pass(self, function: Function, all_functions, variable_types: Dict[str, str], dump_blocks=False):
         for optimizer_triplet in self.mi_optimizers:
             optimizer, target, rank = optimizer_triplet
             if target == "function":
                 optimizer(function)
@@ -120,15 +108,15 @@
     """make_backend(arch='mlog', target='mlog', machine_independents={}, machine_dependents={})
     """
     if machine_independents is None:
         machine_independents = []
     if machine_dependents is None:
         machine_dependents = []
 
-    backend = Backend()
+    backend = Backend(arch, target)
     if arch == "mlog":
         backend.asm_template_handler = mlog_expand_asm_template
     if target == "mlog":
         backend.output_component = IRtoMlogConverter(
             strict_32bit="strict-32bit" in machine_dependents
         )
     elif target == "mlogev_ir":
```

## mlogevo/backend/inline_utils.py

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, Tuple, List, Dict
 from copy import copy
 
 from ..intermediate import Quadruple
+from ..intermediate.ir_quadruple import NO_INPUT_INSTRUCTIONS
 from ..intermediate.function import Function
 
 
 def should_inline(function: Function, arch="mlog") -> bool:
     if function.name == "main":
         return False
     if "inline" not in function.attributes:
@@ -44,33 +45,76 @@
         if should_inline(function, arch):
             inline_functions[function.name] = function
         else:
             common_functions[function.name] = function
     return inline_functions, common_functions
 
 
+def redirect_variable(ir: Quadruple, from_var: str, to_var: str) -> Quadruple:
+    if from_var == to_var:
+        return ir
+    if ir.instruction.startswith("decl_") or ir.instruction in NO_INPUT_INSTRUCTIONS:
+        return ir
+
+    if ir.src1 == from_var:
+        ir.src1 = to_var
+    if ir.src2 == from_var:
+        ir.src2 = to_var
+    if ir.dest == from_var:
+        ir.dest = to_var
+
+    # Avoid modifying original input_vars and output_vars
+    input_vars = []
+    output_vars = []
+    for v in ir.input_vars:
+        input_vars.append(v if v != from_var else to_var)
+    for v in ir.output_vars:
+        output_vars.append(v if v != from_var else to_var)
+    ir.input_vars = input_vars
+    ir.output_vars = output_vars
+    return ir
+
+
 def inline_calls(common_function_name: str,
                  common_function_body: List[Quadruple],
                  inline_functions: Dict[str, Function],) -> List[Quadruple]:
     result_irs: List[Quadruple] = []
     ctr = 0
-    for ir in common_function_body:
+    last_result_assignment: Dict[str, str] = {}
+    # A reference
+    last_assignment_ir: Dict[str, Quadruple] = {}
+    for ir in reversed(common_function_body):
+        if ir.instruction.startswith("set_") and ir.src1.startswith("result@"):
+            last_result_assignment[ir.src1] = ir.dest
+            last_assignment_ir[ir.src1] = ir
+            result_irs.append(ir)
+            continue
         if ir.instruction != "__call":
             result_irs.append(ir)
             continue
         if ir.src1 not in inline_functions.keys():
             result_irs.append(ir)
             continue
         ctr += 1
         inlined_target = inline_functions[ir.src1]
         inlined_body = inlined_target.instructions
-        assert len(inlined_body) >= 2
+        result_var = f"result@{inlined_target.name}"
+        assigned_to_var = last_result_assignment.get(result_var, result_var)
+        inlined_block = []
         return_jump = f"__MLOGEV_INLINE_CALL_{inlined_target.name}_{common_function_name}_{ctr}__"
         for inst in inlined_body:
             if inst.instruction in ("__funcbegin", "__funcend"):
                 continue
             if inst.instruction == "__return":
-                result_irs.append(Quadruple("goto", return_jump))
+                inlined_block.append(Quadruple("goto", return_jump))
                 continue
-            result_irs.append(copy(inst))
-        result_irs.append(Quadruple("label", return_jump))
-    return result_irs
+            inlined_block.append(redirect_variable(copy(inst), result_var, assigned_to_var))
+        inlined_block.append(Quadruple("label", return_jump))
+        #print("\n".join((v.dump() for v in inlined_block)))
+        inlined_block.reverse()
+        result_irs.extend(inlined_block)
+        if assigned_to_var != result_var:
+            last_assignment_ir[result_var].instruction = "ELIMINATED"
+            del last_result_assignment[result_var]
+            del last_assignment_ir[result_var]
+
+    return [i for i in reversed(result_irs) if i.instruction != "ELIMINATED"]
```

## mlogevo/frontend/compiler.py

```diff
@@ -4,15 +4,15 @@
 import os
 # for string constants
 from ast import literal_eval
 
 from pycparser.c_ast import \
     Compound, Constant, DeclList, Enum, FileAST, \
     FuncDecl, Struct, TypeDecl, Typename, PtrDecl, \
-    StructRef
+    Typedef, StructRef
 
 from pycparser.c_ast import NodeVisitor
 from pycparser import parse_file
 
 from pycparserext_gnuc.ext_c_parser import GnuCParser, \
     FuncDeclExt, Asm
 
@@ -23,31 +23,36 @@
 from .type_util import choose_binaryop_instruction, \
     choose_unaryop_instruction, \
     choose_set_instruction, choose_decl_instruction, \
     extract_attribute, \
     extract_typename, DUMMY_INT_TYPEDECL, \
     CORE_COMPARISONS
 from .mlog_object import MlogObjectDefinitionParser, convert_field_name
+from .parent_node_visitor import ParentNodeVisitor
 
 
 # Stateful compiler & ast node visitor
-class Compiler(NodeVisitor):
+# TODO: this stateful compiler is a mess, consider breaking it into several parts
+class Compiler(ParentNodeVisitor):
     def __init__(self):
         self.functions = None
         self.current_function = None
         self.globals: dict = {}
         self.loops: list = []
         self.loop_end: int = 0
         self.vtmp_count: int = 0
+        self.function_vtmp_count: int = 0
         self.instructions: list = []
         self.if_structure_count: int = 0
         self.loop_structure_count: int = 0
         self.loop_stack: list = []
         self.mlog_object_items: Dict[str, str] = {}
         self.mlog_builtins_items: Dict[str, str] = {}
+
+        self.typedefs = {}
         # Used in short-circuit evaluation
         self.short_circuit_count: int = 0
         self.short_circuit_triggered: bool = False
         self.inside_branch_condition: bool = False
         self.tag_if_true: str = ""
         self.tag_if_false: str = ""
         self.tag_if_end: str = ""
@@ -62,14 +67,16 @@
         self.if_structure_count = 0
         self.loop_structure_count = 0
         self.short_circuit_count = 0
         self.loop_stack = []
         self.instructions = []
         self.mlog_object_items = {}
         self.mlog_builtins_items: Dict[str, str] = {}
+
+        self.typedefs = {}
         # Used in short-circuit evaluation
         self.short_circuit_count = 0
         self.short_circuit_triggered = False
         self.inside_branch_condition = False
         self.tag_if_true = ""
         self.tag_if_false = ""
         self.tag_if_end = ""
@@ -124,16 +131,21 @@
         if self.current_function.local_vars.get(variable_name, None) is None:
             # Assume global
             return variable_name
         return F"_{variable_name}@{self.current_function.name}"
 
     # temp variable should be decorated
     def create_temp_variable(self, var_type, autodecorate=True) -> str:
-        self.vtmp_count += 1
-        temp_var_name = F"__vtmp_{self.vtmp_count}"
+        temp_var_name: str
+        if self.current_function is None:
+            self.vtmp_count += 1
+            temp_var_name = F"__vtmp_{self.vtmp_count}"
+        else:
+            self.function_vtmp_count += 1
+            temp_var_name = F"__vtmp_{self.function_vtmp_count}"
         self.declare_variable(temp_var_name, var_type)
         if autodecorate:
             temp_var_name = self.decorate_variable(temp_var_name)
         decl_inst = choose_decl_instruction(var_type)
         if len(decl_inst) > 0:
             self.push(Quadruple(decl_inst, dest=temp_var_name))
         return temp_var_name
@@ -165,23 +177,27 @@
     def declare_variable(self, var_name, var_type):
         if self.current_function is None:
             # is a global variable
             self.globals[var_name] = var_type
         else:
             self.current_function.local_vars[var_name] = var_type
 
+    def extract_actual_typename(self, target) -> str:
+        name = extract_typename(target)
+        return extract_typename(self.typedefs.get(name, target))
+
     # Return old or tmp variable name, or its literal
     # require decorated name
     # self.static_cast("3", [int], [int]) -> "3"
     def static_cast(self, src_var, src_typedecl, dst_typedecl) -> str:
         # TODO: PtrDecl
         # TODO: Struct?
         # Assume src_type and dst_type are TypeDecl
-        src_typename = extract_typename(src_typedecl)
-        dst_typename = extract_typename(dst_typedecl)
+        src_typename = self.extract_actual_typename(src_typedecl)
+        dst_typename = self.extract_actual_typename(dst_typedecl)
         if dst_typename == "int" and src_typename == "double":
             tmp_var = self.create_temp_variable(dst_typedecl, True)
             self.push(Quadruple("cvtf64_i32", src_var, "", tmp_var))
             return tmp_var
         return src_var
 
     def create_loop(self):
@@ -248,14 +264,15 @@
                 params = []
             else:
                 params = [(param_decl.name, param_decl.type)
                           for param_decl in func_decl.args.params]
             specs = [extract_attribute(attr) for attr in node.decl.funcspec] or ["default", ]
             self.current_function = Function(func_name, func_decl.type, params, dict(params), [], specs)
 
+        self.function_vtmp_count = 0
         # self.function_locals = self.current_function.local_vars
         self.functions[func_name] = self.current_function
 
         ir_attributes = ",".join(self.current_function.attributes)
         self.push(Quadruple("__funcbegin", func_name, "", ir_attributes))
         decl_inst = choose_decl_instruction(self.current_function.result_type)
         if len(decl_inst) > 0:
@@ -266,15 +283,17 @@
         self.current_function = None
         # self.function_locals = {}
 
     def visit_Decl(self, node):
         if isinstance(node.type, TypeDecl):
             var_name = node.name
             # Keep TypeDecl, for further Struct/Pointer support
-            var_type = node.type
+            # var_type = node.type
+            var_type = self.typedefs.get(extract_typename(node.type), node.type)
+            
             self.declare_variable(var_name, var_type)
             decorated_name = self.decorate_variable(var_name)
             decl_inst = choose_decl_instruction(var_type)
             if decl_inst:
                 self.push(Quadruple(decl_inst, dest=decorated_name))
             # print("Decl", var_name, var_type.type)
             if node.init is None:
@@ -300,15 +319,18 @@
                 self.mlog_object_items = struct_parser.items
                 return
             if node.type.name == "MLOG_BUILTINS":
                 struct_parser = MlogObjectDefinitionParser()
                 struct_parser.visit(node.type)
                 self.mlog_builtins_items = struct_parser.items
                 return
-            raise NotImplementedError(node)
+            raise CompilationError(
+                reason=f"struct support is not implemented yet",
+                coord=node.coord
+            )
         if isinstance(node.type, PtrDecl):
             # raise NotImplementedError("Pointers are NOT supported in mlog target", node)
             # node.show()
             return
         if isinstance(node.type, Enum):
             raise NotImplementedError(node)
         raise NotImplementedError(node)
@@ -323,27 +345,27 @@
             self.heuristic_assign(rvalue_after_cast, lvalue_decorated, lvalue_typedecl)
             return lvalue_typedecl, lvalue_decorated
 
         binary_op = node.op[:-1]
         result_typedecl, inst = choose_binaryop_instruction(
             binary_op, lvalue_typedecl, rvalue_typedecl
         )
-        if extract_typename(result_typedecl) == extract_typename(lvalue_typedecl):
+        if self.extract_actual_typename(result_typedecl) == self.extract_actual_typename(lvalue_typedecl):
             self.push(Quadruple(inst, lvalue_decorated, rvalue, lvalue_decorated))
             return lvalue_typedecl, lvalue_decorated
 
         temp_var = self.create_temp_variable(result_typedecl, True)
         self.push(Quadruple(inst, lvalue_decorated, rvalue, temp_var))
         temp_after_cast = self.static_cast(temp_var, result_typedecl, lvalue_typedecl)
         self.heuristic_assign(temp_after_cast, lvalue_decorated, lvalue_typedecl)
         return lvalue_typedecl, lvalue_decorated
 
     # Return (type, value)
     def visit_Constant(self, node):
-        typename = extract_typename(node.type)
+        typename = self.extract_actual_typename(node.type)
         if typename in ("double", "float"):
             value = str(float(node.value))
             return node.type, value
         if typename == "string":
             # Treat string as a MlogObject
             return "struct MlogObject", node.value
             pass
@@ -356,23 +378,33 @@
             return self.current_function.result_type, f"result@{self.current_function.name}"
         # decorated_name = self.decorate_variable(node.name)
         var_typedecl, decorated_name = self.get_variable(node.name, node.coord)
         return var_typedecl, decorated_name
 
     def visit_Cast(self, node):
         src_typedecl, src_var = self.visit(node.expr)
-        src_typename = extract_typename(src_typedecl)
-        dst_typename = extract_typename(node.to_type.type)
+        src_typename = self.extract_actual_typename(src_typedecl)
+        dst_typename = self.extract_actual_typename(node.to_type.type)
         # Mlog Object can contain int or double
         if src_typename == dst_typename or dst_typename == "struct MlogObject":
             return src_typedecl, src_var
 
         result_var = self.static_cast(src_var, src_typedecl, node.to_type.type)
         return node.to_type.type, result_var
 
+    def visit_Typedef(self, node: Typedef):
+        typedecl = node.type
+        while extract_typename(typedecl) in self.typedefs.keys():
+            name = extract_typename(typedecl)
+            if name == self.typedefs[name]:
+                break
+            typedecl = self.typedefs[name]
+        self.typedefs[node.name] = typedecl
+        pass
+
     # May be generated by comma operators
     def visit_ExprList(self, node):
         var_typedecl = None
         name_or_value = None
         for child in node:
             var_typedecl, name_or_value = self.visit(child)
         return var_typedecl, name_or_value
@@ -542,16 +574,16 @@
 
     def visit_Return(self, node):
         function_name = self.current_function.name
         if node.expr is not None:
             r_typedecl, r_varname = self.visit(node.expr)
             result_typedecl = self.current_function.result_type
             result = r_varname
-            if extract_typename(r_typedecl) \
-                    != extract_typename(result_typedecl):
+            if self.extract_actual_typename(r_typedecl) \
+                    != self.extract_actual_typename(result_typedecl):
                 result = self.static_cast(r_varname, r_typedecl, result_typedecl)
 
             dest = f"result@{function_name}"
             self.heuristic_assign(result, dest, result_typedecl)
         self.push(Quadruple("__return", function_name))
 
     def visit_FuncCall(self, node):
@@ -578,16 +610,16 @@
             raise ValueError(f"{function_name} is not a function (or not declared)")
         # if len(func.params) != len(args):
         #    raise ValueError(f"{function_name} expect {len(func.params)} params, got {len(args)}")
         for param_decl, arg in zip(func.params, args):
             param_realname = f"_{param_decl[0]}@{function_name}"
             arg_typedecl, arg_varname = self.visit(arg)
             real_argument = arg_varname
-            param_type = extract_typename(param_decl[1])
-            if extract_typename(arg_typedecl) != param_type:
+            param_type = self.extract_actual_typename(param_decl[1])
+            if self.extract_actual_typename(arg_typedecl) != param_type:
                 real_argument = self.static_cast(arg_varname, arg_typedecl, param_decl[1])
             self.heuristic_assign(real_argument, param_realname, param_decl[1])
         self.push(Quadruple("__call", function_name))
         decl_inst = choose_decl_instruction(func.result_type)
         if decl_inst != "":
             self.push(Quadruple(decl_inst, dest=f"result@{function_name}"))
         # Assume a function returns something
@@ -616,39 +648,38 @@
             if constraints[0] == '+':
                 result_ir.input_vars.append(var_name)
         self.push(result_ir)
 
     def visit_StructRef(self, node: StructRef):
         # NOTE: this ignores node.type ( . or -> )
         base_typedecl, base_var = self.visit(node.name)
-        base_type = extract_typename(base_typedecl)
+        base_type = self.extract_actual_typename(base_typedecl)
         if not base_type.startswith("struct "):
             raise CompilationError(
                 reason=f"Attempted to use StructRef on non-struct item",
                 coord=node.coord
             )
         field_name = node.field.name
         result_type = None
         result_var = None
-
-        if base_type == "struct MlogObject":
-            result_type = self.mlog_object_items.get(field_name)
-            result_var = self.create_temp_variable(result_type)
-            asm_ir = Quadruple("asm")
-            asm_ir.raw_instructions.append(f"sensor %0 %1 {convert_field_name(field_name)}")
-            asm_ir.input_vars.append(base_var)
-            asm_ir.output_vars.append(result_var)
-            self.push(asm_ir)
-        elif base_type == "struct MLOG_BUILTINS":
-            result_type = self.mlog_builtins_items.get(field_name)
-            result_var = convert_field_name(field_name)
-
-        if result_type is None or result_var is None:
+        try:
+            if base_type == "struct MlogObject":
+                result_type = self.mlog_object_items[field_name]
+                result_var = self.create_temp_variable(result_type)
+                asm_ir = Quadruple("asm")
+                asm_ir.raw_instructions.append(f"sensor %0 %1 {convert_field_name(field_name)}")
+                asm_ir.input_vars.append(base_var)
+                asm_ir.output_vars.append(result_var)
+                self.push(asm_ir)
+            elif base_type == "struct MLOG_BUILTINS":
+                result_type = self.mlog_builtins_items[field_name]
+                result_var = convert_field_name(field_name)
+        except KeyError as e:
             raise CompilationError(
-                reason=f"{base_type} does not have field `{field_name}`",
+                reason=f"`{base_type}` does not have field `{e.args[0]}`",
                 coord=node.coord
             )
         return result_type, result_var
 
 
 
 def extract_asm_operand(operand):
```

## mlogevo/frontend/parent_node_visitor.py

```diff
@@ -1,24 +1,27 @@
 from pycparser.c_ast import NodeVisitor
 
 class ParentNodeVisitor(NodeVisitor):
     def __init__(self):
         self._method_cache = {}
+        self.node_stack = []
         self.current_parent = None
 
     def visit(self, node):
         """ Visit a node, while keep a parent node reference in self.current_parent """
         # Almost copy-pasted part from pycparser.c_ast.NodeVisitor
         visitor = self._method_cache.get(node.__class__.__name__, None)
         if visitor is None:
             method = 'visit_' + node.__class__.__name__
             visitor = getattr(self, method, self.generic_visit)
             self._method_cache[node.__class__.__name__] = visitor
 
         # No, python does NOT have tail call optimization
         # https://stackoverflow.com/questions/13591970/does-python-optimize-tail-recursion
-        old_parent = self.current_parent
-        self.current_parent = node
+        if len(self.node_stack) > 0:
+            self.current_parent = self.node_stack[-1]
+
+        self.node_stack.append(node)
         result = visitor(node)
-        self.current_parent = old_parent
+        self.node_stack.pop()
 
         return result
```

## mlogevo/frontend/type_util.py

```diff
@@ -63,14 +63,16 @@
     rank_r = CONVERSION_RANK.get(extract_typename(type_r), None)
     if rank_l < rank_r:
         return type_r, rank_r
     return type_l, rank_l
 
 
 def decorate_instruction(core, result_rank):
+    if result_rank == -1:
+        return f"{core}_obj"
     return f"{core}_f64" if result_rank >= 7 else f"{core}_i32"
 
 
 def choose_binaryop_instruction(operator, type_l, type_r):
     "type_l, type_r can be string 'int' or TypeDecl. return (typedecl, inst)"
     result_type, result_rank = get_arithmetic_result_type(type_l, type_r)
     if operator in CORE_COMPARISONS.keys():
```

## mlogevo/intermediate/ir_quadruple.py

```diff
@@ -19,14 +19,18 @@
     "cvtf64_i32", "cvti32_f64",
     # __funcbegin function_name attribute
     "__funcbegin",
 }
 I2O1_INSTRUCTIONS = {"eq_obj", "ne_obj", }
 O1_INSTRUCTIONS = {"decl_obj", }
 COMPARISONS = {"eq_obj", "ne_obj", }
+NO_INPUT_INSTRUCTIONS = {
+    "goto", "label", "__funcbegin", "__funcend",
+    "__call", "__return",
+}
 
 CORE_I1O1_ITEMS = {
     "set", "minus",
 }
 CORE_I2O1_ITEMS = {
     "add", "sub", "mul", "div",
     "lt", "gt", "lteq", "gteq", "eq", "ne"
@@ -63,15 +67,15 @@
 
 for i in I32ONLY_I1O1_ITEMS:
     I1O1_INSTRUCTIONS.add(f"{i}_i32")
 
 for i in I32ONLY_I2O1_ITEMS:
     I2O1_INSTRUCTIONS.add(f"{i}_i32")
 
-variable_pattern = re.compile(r'^[A-Za-z_@][_@()\[\]\w]+')
+variable_pattern = re.compile(r'^[A-Za-z_@][_@()\[\]\w]*')
 
 
 def test_parameter_type(param: str) -> str:
     """Test a parameter if it's a "immediate_integer", "immediate_float", "variable" or "invalid" """
     if type(param) is not str or len(param) == 0:
         return "invalid"
     if variable_pattern.match(param):
```

## mlogevo/optimizer/mi_remove_unused_variables.py

```diff
@@ -10,41 +10,44 @@
     target="function",
     is_machine_dependent=False,
     rank=20,
     optimize_level=1
 )
 def remove_unused_variables(func: Function) -> Function:
     insts = func.instructions
-    referred_variables = set()
-    referred_variables.add("")
+    referred_variables = {"", }
+    involved_functions = {func.name, }
 
     for inst in insts:
         if inst in ("goto", "__funcbegin", "__funcend"):
             continue
         if inst.instruction.startswith("decl_"):
             continue
+        # TODO: call vs __call
+        if inst.instruction == "__call":
+            involved_functions.add(inst.src1)
+
         referred_variables.add(inst.src1)
         referred_variables.add(inst.src2)
         for var in inst.input_vars:
             referred_variables.add(var)
 
     result_insts = []
     for inst in insts:
-        if inst.instruction.startswith("decl_") and should_remove_decl(inst, func.name, referred_variables):
+        if inst.instruction.startswith("decl_") \
+                and should_remove_name(inst.src1, func.name, referred_variables, involved_functions):
             continue
-        if inst.dest.endswith(f"@{func.name}") and should_remove_normal(inst, func.name, referred_variables):
+        if inst.dest.endswith(f"@{func.name}") \
+                and should_remove_name(inst.dest, func.name, referred_variables, involved_functions):
             continue
         result_insts.append(inst)
     func.instructions = result_insts
     return func
 
 
-def should_remove_decl(inst: Quadruple, function_name: str, referred: Set):
-    return inst.src1.endswith(f"@{function_name}") \
-        and not inst.src1.startswith("result@") \
-        and inst.src1 not in referred
-
-
-def should_remove_normal(inst: Quadruple, function_name: str, referred: Set):
-    return inst.dest.endswith(f"@{function_name}") \
-        and not inst.dest.startswith("result@") \
-        and inst.dest not in referred
+def should_remove_name(name: str, function_name: str, referred: Set, involved_functions: Set):
+    if name in referred or "@" not in name or name.startswith("@"):
+        return False
+    function_scope = name.rsplit("@")[-1]
+    if function_scope not in involved_functions:
+        return True
+    return function_scope == function_name and not name.startswith("result@")
```

## Comparing `mlogevo-0.0.8.dist-info/LICENSE` & `mlogevo-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlogevo-0.0.8.dist-info/METADATA` & `mlogevo-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogevo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Compile C code to Mindustry logic
 Home-page: https://github.com/UMRnInside/MlogEvo
 Author: UMRnInside
 Author-email: 30196401+UMRnInside@users.noreply.github.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/UMRnInside/MlogEvo/issues
 Platform: UNKNOWN
```

## Comparing `mlogevo-0.0.8.dist-info/RECORD` & `mlogevo-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 mlogevo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlogevo/__main__.py,sha256=ilT_r1lEpQqqjp8a5xReLw4bqtGT7tHhQxsDuveKYEM,3596
 mlogevo/backend/__init__.py,sha256=vW-LOv-3RoI6h-sckYOrrIZd7NI419BwhHLchDOduEM,73
 mlogevo/backend/asm_template.py,sha256=nyMCWzqGfP9LX_WQm10UyBXvnszHgML37cxCrxSuTmA,787
-mlogevo/backend/backend.py,sha256=5td_5QiSFH4GcCwBIH-BUMmlKGFQI3yz_dYa4b3Li1A,5527
+mlogevo/backend/backend.py,sha256=arzGMfj_7nvPdRLowW1p8zGZ2msKwNOvPo0sd_877Rs,5138
 mlogevo/backend/basic_block.py,sha256=iyTmOVx3nS1X55NXGG3icFiyg1MTAwKmaG5GDF5RWCo,2533
-mlogevo/backend/inline_utils.py,sha256=D8Oz_BB2oAEY7-Cz9mH2ExgkrPzXboXujsXwCgKTFmg,2681
+mlogevo/backend/inline_utils.py,sha256=Xo0E-W12SXwE5yxZGvk5nVN5LsnRyz4S8zsuTC-1QQI,4422
 mlogevo/frontend/__init__.py,sha256=jAvw-O56g1uQDdEIMe9hLxJ99xNs1gJzP78RaxByX6I,79
 mlogevo/frontend/compilation_error.py,sha256=mfNM-x5FnMcuBxk4D1KyEtTxpm83re6GlavOMMqop1Y,184
-mlogevo/frontend/compiler.py,sha256=AVhA6qZjU7fbhqC8Cb4FaMIQ954-sMVTNOja4ScoIQU,27743
+mlogevo/frontend/compiler.py,sha256=8LlpqVEV5fJALWDbYoVwInWX6yjmiRqXYHDpywbUTaM,29104
 mlogevo/frontend/mlog_object.py,sha256=WynQmBe2pDqVA9clrWVqhVJociycVkj4yBKN4qHDH94,985
-mlogevo/frontend/parent_node_visitor.py,sha256=KBy5hkDnu_dqrzOt8Nzt2SN8tZwv-8EWLlQV-G4AUJY,960
-mlogevo/frontend/type_util.py,sha256=2Wbs6tmuY2nBn3qMrmhzUxCC6IASoqzLApI7pmLiJM8,3486
+mlogevo/frontend/parent_node_visitor.py,sha256=aTzPtVc14R-A4QdeN5tZga-zN8rxo9EqU910PKb48bg,1031
+mlogevo/frontend/type_util.py,sha256=vcQqp-A5iY0LrTx2K37s3rR0g5TQqwNBEWjoTzMmLUU,3541
 mlogevo/intermediate/__init__.py,sha256=wx8iGDqU9N5Mk0eqhIDLH7x8Sj1o-aVOUhHULk02Zn8,214
 mlogevo/intermediate/function.py,sha256=5QcINvQj2tPFLkxHuRXogfAI2FAs8LT4JEVa6jTETTc,429
-mlogevo/intermediate/ir_quadruple.py,sha256=K0xTC8H3CC_rd0WGIOUpTmbrQhP95wrn-vgG0az1ceE,4255
+mlogevo/intermediate/ir_quadruple.py,sha256=8DdkoEhTFYiYltJyDpU8de2LrLr-VucmsJvEGSb75ZU,4358
 mlogevo/intermediate/quadruple_from_text.py,sha256=TdNve815tiMZC86VWdoR3jMCNbSLxhx3kUovf2MNb3I,2845
 mlogevo/optimizer/__init__.py,sha256=chlC69NJDasvs7Y_A3giqrygD05lVhI0WY--MaHYv0s,2182
 mlogevo/optimizer/mi_deduplicate_tail_return.py,sha256=fWBGufyZ6dWxgFhXzQFg2f4YCq7zFS2ypp_KY_A_OsU,741
 mlogevo/optimizer/mi_lcse.py,sha256=jYRTkMQVwJDWUcUuoYzTF_yHLDbRrRbZNVt5ibYHtcE,18637
 mlogevo/optimizer/mi_remove_unused_decls.py,sha256=oYGFgqZJmdSQ-0CgOe_LYZ1iof4C5WB4O_B2MyPNM_g,928
 mlogevo/optimizer/mi_remove_unused_labels.py,sha256=FWCpZtKQ9csZSQdkUolA08DSkmn4CmaMCe-0bbwnT30,890
-mlogevo/optimizer/mi_remove_unused_variables.py,sha256=ucFdzEsPddKMKz3RGkJxXgBNLNJMcP-PQvyHTKtD4g8,1667
+mlogevo/optimizer/mi_remove_unused_variables.py,sha256=Kuz8IWTDjbstSm8npD67U5qHzuemNcFLEvR3XhP3ZW8,1815
 mlogevo/optimizer/mi_reorder_decls.py,sha256=60AXQgdZm2unRh3S19zA4idcYnICHScgERk_zCdKt_c,654
 mlogevo/optimizer/optimizer_registry.py,sha256=IsqvblTk3xp6nyNu4qCOyVBgAdeKYVCZvpZ_dOkHHJM,1120
 mlogevo/output/__init__.py,sha256=zqw5pjVHxTetm_lC_Grarx0xL-fLmiXJ5n7AtozvvV0,55
 mlogevo/output/abstract_ir_converter.py,sha256=8XFV9SEgsg2EmIHg7buPKamzAinT23SjJEG7AHTWkAo,172
 mlogevo/output/ir_output.py,sha256=rfdpu5suowJt4L0ER5_IpiLpNhU_AQ5xWntM3qbMFgU,338
 mlogevo/output/mlog_instructions.py,sha256=ju4Smbkr0MN1-9h64YiS8-kB-_i3HSuF9mB0kDzEjJc,5718
 mlogevo/output/mlog_output.py,sha256=vByZiXQjNAGSGLap_XywLbUZk7YYzjCMiXTwgTjmucY,2930
-mlogevo-0.0.8.dist-info/LICENSE,sha256=q0jTskpkyOwKFf24sfdxjz_n3a9bJyzzdo2vJhZmihE,1067
-mlogevo-0.0.8.dist-info/METADATA,sha256=h_QKS91no_u2xSEvCzX2UgjrBCQXyXtUuPUnCcgEA7g,4626
-mlogevo-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mlogevo-0.0.8.dist-info/entry_points.txt,sha256=mSTpt0NUa_VBKKorcIFLgmwwvUcoSE6-Hi6N5jsah-k,51
-mlogevo-0.0.8.dist-info/top_level.txt,sha256=6hW6bv3IqfUHLP8IGTPBar6JVL_UihhcASQAMpjO2JQ,8
-mlogevo-0.0.8.dist-info/RECORD,,
+mlogevo-0.0.9.dist-info/LICENSE,sha256=q0jTskpkyOwKFf24sfdxjz_n3a9bJyzzdo2vJhZmihE,1067
+mlogevo-0.0.9.dist-info/METADATA,sha256=yymg4GWZshvy3aoG8xnvs6xwGMPMilvu6-r6V7SmHUY,4626
+mlogevo-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mlogevo-0.0.9.dist-info/entry_points.txt,sha256=mSTpt0NUa_VBKKorcIFLgmwwvUcoSE6-Hi6N5jsah-k,51
+mlogevo-0.0.9.dist-info/top_level.txt,sha256=6hW6bv3IqfUHLP8IGTPBar6JVL_UihhcASQAMpjO2JQ,8
+mlogevo-0.0.9.dist-info/RECORD,,
```

