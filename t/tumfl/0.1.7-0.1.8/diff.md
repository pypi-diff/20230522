# Comparing `tmp/tumfl-0.1.7.tar.gz` & `tmp/tumfl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.7.tar", last modified: Tue May  9 19:07:22 2023, max compression
+gzip compressed data, was "tumfl-0.1.8.tar", last modified: Mon May 22 15:03:54 2023, max compression
```

## Comparing `tumfl-0.1.7.tar` & `tumfl-0.1.8.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 19:07:22.497871 tumfl-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 19:07:09.000000 tumfl-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-09 19:07:09.000000 tumfl-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 19:07:22.497871 tumfl-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.485871 tumfl-0.1.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37047 2023-05-09 19:07:09.000000 tumfl-0.1.7/test/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl/AST/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/ASTNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/BaseFunctionDefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/tumfl/AST/Expression/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/BinOp.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionCall.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Index.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/NamedIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Nil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Number.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/String.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/TableField.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/UnOp.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Vararg.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/Variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.493871 tumfl-0.1.7/tumfl/AST/Statement/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Assign.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Block.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Break.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/FunctionCall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/FunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Goto.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/If.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/IterativeFor.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/LocalAssign.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/MethodInvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/NumericFor.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Semicolon.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/Statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/While.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/Statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/AST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/basic_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32663 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-09 19:07:09.000000 tumfl-0.1.7/tumfl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:07:22.489871 tumfl-0.1.7/tumfl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:07:22.000000 tumfl-0.1.7/tumfl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.422342 tumfl-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 15:03:54.422342 tumfl-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 15:03:41.000000 tumfl-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 15:03:41.000000 tumfl-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 15:03:54.422342 tumfl-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37003 2023-05-22 15:03:41.000000 tumfl-0.1.8/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/tumfl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.418342 tumfl-0.1.8/tumfl/AST/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/ASTNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/BaseFunctionDefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.418342 tumfl-0.1.8/tumfl/AST/Expression/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/BinOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/NamedIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Nil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/String.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/TableField.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/UnOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Vararg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/Variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.422342 tumfl-0.1.8/tumfl/AST/Statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/FunctionCall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/FunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Goto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/IterativeFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/LocalAssign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/MethodInvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/NumericFor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Semicolon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/Statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/While.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/Statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/AST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/basic_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32804 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-22 15:03:41.000000 tumfl-0.1.8/tumfl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:03:54.414342 tumfl-0.1.8/tumfl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 15:03:54.000000 tumfl-0.1.8/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.7/PKG-INFO` & `tumfl-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.7/pyproject.toml` & `tumfl-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.7"
+version = "0.1.8"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `tumfl-0.1.7/test/test_lexer.py` & `tumfl-0.1.8/test/test_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,23 @@
     def test_multiple(self):
         lex = Lexer("[=[==[===[1245121[[\\\n]]]==]]=]a")
         self.assertEqual(lex.get_long_brackets(), "==[===[1245121[[\\\n]]]==]")
         self.assertEqual(lex.current_char, "a")
 
     def test_fails(self):
         lex = Lexer("[[dklaospkda\\")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_long_brackets()
         lex = Lexer("[==[[[]]]=]]===]")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_long_brackets()
 
     def test_no_long_bracket(self):
         lex = Lexer("[=======")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_long_brackets()
 
 
 class TestSkipComment(unittest.TestCase):
     def test_single_line_comment(self):
         lex = Lexer("--123456''\n1")
         lex.skip_comment()
@@ -188,51 +188,51 @@
         lex = Lexer("'\"'")
         self.assertEqual(lex.get_string(), '"')
         lex = Lexer('"\'"')
         self.assertEqual(lex.get_string(), "'")
 
     def test_fail_eof(self):
         lex = Lexer("'abc")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_string()
 
     def test_fail_line_end(self):
         lex = Lexer("'abc\n'")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_string()
 
     def test_simple_escape_codes(self):
         lex = Lexer(r"'\a\b\f\n\r\t\v\\\"\''")
         self.assertEqual(lex.get_string(), "\a\b\f\n\r\t\v\\\"'")
         lex = Lexer("'\\\n'")
         self.assertEqual(lex.get_string(), "\n")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex = Lexer("'\\A'")
             lex.get_string()
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex = Lexer("'\\e'")
             lex.get_string()
 
     def test_hexadecimal_escape(self):
         lex = Lexer("'\\x1'")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_string()
         lex = Lexer("'\\x'")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_string()
         lex = Lexer("'\\x0a'")
         self.assertEqual(lex.get_string(), "\n")
         lex = Lexer("'\\x61'")
         self.assertEqual(lex.get_string(), "a")
 
     def test_decimal_escape(self):
         lex = Lexer("'\\0'")
         self.assertEqual(lex.get_string(), "\0")
         lex = Lexer("'\\256'")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_string()
         lex = Lexer("'\\97\\0971'")
         self.assertEqual(lex.get_string(), "aa1")
         lex = Lexer("'\\97lo\\10\\04923\"'")
         self.assertEqual(lex.get_string(), 'alo\n123"')
 
 
@@ -268,15 +268,15 @@
         )
         self.assertEqual(lex.get_next_token(), Token(TokenType.STRING, "abab'", 2, 1))
         self.assertEqual(lex.get_next_token(), Token(TokenType.STRING, "abc", 5, 10))
         self.assertEqual(lex.get_next_token(), Token(TokenType.EOF, "eof", 5, 15))
 
     def test_tokenizer_error(self):
         lex = Lexer("!")
-        with self.assertRaises(LexerException):
+        with self.assertRaises(LexerError):
             lex.get_next_token()
 
 
 class TestNil(unittest.TestCase):
     def test_nil(self):
         lex = Lexer("nil")
         self.assertEqual(lex.get_next_token(), Token(TokenType.NIL, "nil", 1, 1))
```

### Comparing `tumfl-0.1.7/test/test_parser.py` & `tumfl-0.1.8/test/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from tumfl.AST import *
 from tumfl.AST.BaseFunctionDefinition import BaseFunctionDefinition
 from tumfl.lexer import Lexer
-from tumfl.parser import Parser, ParserException
+from tumfl.parser import Parser, ParserError
 from tumfl.Token import Token, TokenType
 
 
 class TestParser(unittest.TestCase):
     @staticmethod
     def parse_number(to_parse: str) -> Number:
         lex = Lexer(to_parse)
@@ -127,15 +127,15 @@
         repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_error(self):
         parser = Parser("1+")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser._parse_exp()
 
     def test_unary_expr(self):
         parser = Parser("1- -2")
         expected_tree = BinOp.from_token(
             Token(TokenType.MINUS, "-", 0, 0),
             self.parse_number("1"),
@@ -159,18 +159,18 @@
         repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_wrong_token(self):
         parser = Parser("a,b+")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser.parse_chunk()
         parser = Parser("a=1\nb,c+")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser.parse_chunk()
 
     def test_parse_var(self):
         parser = Parser('a["b"].d')
         expected_tree = NamedIndex(
             Token(TokenType.NAME, "d", 0, 0),
             Index(
@@ -316,18 +316,18 @@
             self.parse_string("d"),
             self.parse_number("1"),
         ]
         self.assertEqual(parser._parse_args(), expected_args)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(a,b")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser._parse_args()
         parser = Parser("(a,b,)")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser._parse_args()
         parser = Parser('"abc"')
         self.assertEqual(parser._parse_args(), [self.parse_string("abc")])
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser('{a,"b"}')
         table_result = parser._parse_table_constructor()
@@ -354,18 +354,18 @@
         self.assertEqual(parser.current_token, Token(TokenType.NAME, "b", 0, 0))
         parser = Parser(",b")
         expected_names = [self.parse_name("a"), self.parse_name("b")]
         self.assertEqual(parser._parse_name_list(self.parse_name("a")), expected_names)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("a,")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser._parse_name_list()
         parser = Parser("a, 1")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser._parse_name_list()
 
     def test_parse_vararg(self):
         parser = Parser("...")
         expected_tree = Vararg(Token(TokenType.ELLIPSIS, "...", 0, 0))
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
@@ -593,15 +593,15 @@
         repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_unknown_local(self):
         parser = Parser("local and")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser.parse_chunk()
 
     def test_parse_function(self):
         parser = Parser("function a ()end")
         expected_tree = self.get_chunk(
             FunctionDefinition(
                 Token(TokenType.FUNCTION, "function", 0, 0),
@@ -688,15 +688,15 @@
         repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_unknown_for(self):
         parser = Parser("for name and")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser.parse_chunk()
 
     def test_parse_if(self):
         parser = Parser("if 1 then end")
         expected_tree = self.get_chunk(
             If(
                 Token(TokenType.IF, "if", 0, 0),
@@ -855,15 +855,15 @@
         repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_unexpected_statement(self):
         parser = Parser("+")
-        with self.assertRaises(ParserException):
+        with self.assertRaises(ParserError):
             parser.parse_chunk()
 
     def test_weird_stuff(self):
         parser = Parser("assert()()")
         expected_tree = self.get_chunk(
             FunctionCall(
                 Token(TokenType.NAME, "assert", 0, 0),
```

### Comparing `tumfl-0.1.7/tumfl/AST/ASTNode.py` & `tumfl-0.1.8/tumfl/AST/ASTNode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
 from abc import ABC
-from typing import Any, Generator, Optional
+from pathlib import Path
+from typing import Any, Generator, Generic, Optional, TypeVar
 
 from tumfl.Token import Token
 from tumfl.utils import generic_str
 
+T = TypeVar("T")
 
-class ASTNode(ABC):
+
+class ASTNode(ABC, Generic[T]):
     """Base class for all AST nodes"""
 
     def __init__(self, token: Token, name: str) -> None:
         self.name: str = name
         self.token: Token = token
         self.parent_class: Optional[ASTNode] = None
+        self.file_name: Optional[Path] = None
+        self.attributes: Optional[T] = None
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return all(
             callable(getattr(self, i)) or getattr(self, i) == getattr(other, i)
             for i in self.__dir()
@@ -28,23 +33,34 @@
 
     def __dir(self) -> Generator[str, None, None]:
         return (
             i
             for i in dir(self)
             if not i.startswith("__")
             # ignore "token" for comparison (and parent check)
-            and i not in ["replace", "parent", "parent_class", "var", "token"]
+            and i
+            not in ["replace", "parent", "parent_class", "var", "token", "comment"]
         )
 
-    def parent(self, parent: Optional[ASTNode]) -> None:
+    def parent(
+        self, parent: Optional[ASTNode], file_name: Optional[Path] = None
+    ) -> None:
         self.parent_class = parent
+        self.file_name = file_name
         for i in self.__dir():
             node: Any = getattr(self, i)
             if isinstance(node, ASTNode):
-                node.parent(self)
+                node.parent(self, file_name)
+            elif (
+                isinstance(node, list)
+                and len(node) > 0
+                and isinstance(node[0], ASTNode)
+            ):
+                for node in node:
+                    node.parent(self, file_name)
 
     def replace_child(self, to_replace: ASTNode, replacement: ASTNode) -> None:
         for i in self.__dir():
             node: Any = getattr(self, i)
             if node is to_replace:
                 setattr(self, i, replacement)
                 return
```

### Comparing `tumfl-0.1.7/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.8/tumfl/AST/BaseFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/BinOp.py` & `tumfl-0.1.8/tumfl/AST/Expression/BinOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.8/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.8/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/Name.py` & `tumfl-0.1.8/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/Number.py` & `tumfl-0.1.8/tumfl/AST/Expression/Number.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/String.py` & `tumfl-0.1.8/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.8/tumfl/AST/Expression/TableField.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.8/tumfl/AST/Expression/UnOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.8/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.8/tumfl/AST/Statement/Assign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.8/tumfl/AST/Statement/FunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.8/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/If.py` & `tumfl-0.1.8/tumfl/AST/Statement/If.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.8/tumfl/AST/Statement/IterativeFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.8/tumfl/AST/Statement/LocalAssign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.8/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/MethodInvocation.py` & `tumfl-0.1.8/tumfl/AST/Statement/MethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.8/tumfl/AST/Statement/NumericFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.8/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/Token.py` & `tumfl-0.1.8/tumfl/Token.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     OR = "or"
     REPEAT = "repeat"
     RETURN = "return"
     THEN = "then"
     TRUE = "true"
     UNTIL = "until"
     WHILE = "while"
+    AS = "as"
+    IS = "is"
     PLUS = "+"
     MINUS = "-"
     MULT = "*"
     DIVIDE = "/"
     MODULO = "%"
     EXPONENT = "^"
     HASH = "#"
```

### Comparing `tumfl-0.1.7/tumfl/basic_walker.py` & `tumfl-0.1.8/tumfl/basic_walker.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl/formatter.py` & `tumfl-0.1.8/tumfl/formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import string
 from enum import Enum
-from typing import Iterator, Optional, Sequence, Type
+from typing import Iterator, Literal, Optional, Sequence, Type
 
 from .AST import *
 from .basic_walker import BasicWalker
 
 
 class FormattingStyle:
     # pylint: disable=too-few-public-methods
@@ -61,30 +61,44 @@
         join_list: list[Retype] = list(to_join)
         for i in range(len(join_list) - 1, 0, -1):
             join_list[i:i] = [[self]]
         return [elem for part in join_list for elem in part]
 
 
 Retype = list[str | Separators]
+ESCAPE_CHARACTERS: dict[str, str] = {
+    "\a": "a",
+    "\b": "b",
+    "\f": "f",
+    "\n": "n",
+    "\r": "r",
+    "\t": "t",
+    "\v": "v",
+}
 
 
 class Formatter(BasicWalker[Retype]):
     # pylint: disable=too-many-public-methods
 
     def __init__(self, style: Type[FormattingStyle]):
         self.s: Type[FormattingStyle] = style
 
     def _format_args(self, arguments: Sequence[ASTNode]) -> Retype:
         return Separators.Argument.join(self.visit(arg) for arg in arguments)
 
     @staticmethod
     def _find_level(to_check: str) -> int:
         level: int = 0
+        if to_check.endswith("]"):
+            level = 1
         while True:
-            if f"[{'=' * level}[" not in to_check:
+            if (
+                f"[{'=' * level}[" not in to_check
+                and f"]{'=' * level}]" not in to_check
+            ):
                 break
             level += 1
         return level
 
     def _format_comment(self, comment: str, force_long: bool = False) -> Retype:
         comment = comment.strip()
         if force_long or "\n" in comment:
@@ -96,75 +110,83 @@
         if self.s.USE_CALL_SHORTHAND and len(args) == 1:
             if isinstance(args[0], String):
                 return self.visit(args[0])
             if isinstance(args[0], Table):
                 return self.visit(args[0])
         return ["(", *self._format_args(args), ")"]
 
+    def _format_var(self, var: Expression) -> Retype:
+        if isinstance(
+            var, (Name, Index, NamedIndex, ExpFunctionCall, ExpMethodInvocation)
+        ):
+            return self.visit(var)
+        return ["(", *self.visit(var), ")"]
+
     def visit_Assign(self, node: Assign) -> Retype:
+        targets: list[Retype] = [self._format_var(var) for var in node.targets]
         return [
-            *self._format_args(node.targets),
+            *Separators.Argument.join(iter(targets)),
             Separators.Space,
             "=",
             Separators.Space,
             *self._format_args(node.expressions),
         ]
 
     def visit_Block(self, node: Block) -> Retype:
-        result: Retype = [Separators.Indent]
+        result: Retype = ["do", Separators.Statement, Separators.Indent]
         for statement in node.statements:
             if self.s.INCLUDE_COMMENTS and statement.comment:
                 for comment in statement.comment:
                     result += self._format_comment(comment)
             result += self.visit(statement) + [Separators.Statement]
         if node.returns:
             returns: Retype = self._format_args(node.returns)
             result += ["return", Separators.Space, *returns, Separators.Statement]
-        result.append(Separators.DeIndent)
+        result += [Separators.DeIndent, "end"]
         return result
 
     def visit_Boolean(self, node: Boolean) -> Retype:
         return [str(node.value).lower()]
 
     def visit_Break(self, _node: Break) -> Retype:
         return ["break"]
 
     def visit_Chunk(self, node: Chunk) -> Retype:
         result: Retype = self.visit_Block(node)
-        return [Separators.DeIndent, *result[:-2]]
+        return result[3:-3]
 
     def visit_Goto(self, node: Goto) -> Retype:
         return ["goto", Separators.Space, *self.visit(node.label_name)]
 
     def visit_If(self, node: If) -> Retype:
         spaced_test: Retype = [
             Separators.Space,
             *self.visit(node.test),
             Separators.Space,
         ]
         result: Retype = ["if", *spaced_test, "then", Separators.Statement]
-        result += self.visit(node.true)
+        result += self.visit(node.true)[2:-1]
         current_if: If = node
         while isinstance(current_if.false, If):
             current_if = current_if.false
             spaced_test = [
                 Separators.Space,
                 *self.visit(current_if.test),
                 Separators.Space,
             ]
             result += ["elseif", *spaced_test, "then", Separators.Statement]
-            result += self.visit(current_if.true)
+            result += self.visit(current_if.true)[2:-1]
         if current_if.false:
             result += ["else", Separators.Statement]
-            result += self.visit(current_if.false)
+            result += self.visit(current_if.false)[2:-1]
         result += ["end"]
         return result
 
     def visit_Index(self, node: Index) -> Retype:
-        return [*self.visit(node.lhs), "[", *self.visit(node.variable_name), "]"]
+        return [*self._format_var(node.lhs), "[", *self.visit(node.variable_name), "]"]
 
     def visit_Label(self, node: Label) -> Retype:
         return ["::", *self.visit(node.label_name), "::"]
 
     def visit_Name(self, node: Name) -> Retype:
         return [node.variable_name]
 
@@ -174,47 +196,71 @@
     def visit_Number(self, node: Number) -> Retype:
         return [str(node)]
 
     def visit_Repeat(self, node: Repeat) -> Retype:
         return [
             "repeat",
             Separators.Statement,
-            *self.visit(node.body),
+            *self.visit(node.body)[2:-1],
             "until",
             Separators.Space,
             *self.visit(node.condition),
         ]
 
     def visit_Semicolon(self, _node: Semicolon) -> Retype:
         return [";"]
 
     def visit_String(self, node: String) -> Retype:
-        if "\n" in node.value:
+        escaped: str = ""
+        quote: str = '"'
+        contains_newline: bool = False
+        contains_unprintable: bool = False
+        single_quote_count: int = 0
+        double_quote_count: int = 0
+        for char in node.value:
+            if char == "\n":
+                contains_newline = True
+            elif char == "'":
+                single_quote_count += 1
+            elif char == '"':
+                double_quote_count += 1
+            elif not 32 <= ord(char) < 127:
+                contains_unprintable = True
+        if contains_newline and not contains_unprintable:
             level: int = self._find_level(node.value)
             return [f"[{'=' * level}[{node.value}]{'=' * level}]"]
-        if self.s.USE_SINGLE_QUOTE and node.value.count("'") < node.value.count('"'):
-            return ["'" + node.value.replace("'", "\\'") + "'"]
-        return ['"' + node.value.replace('"', '\\"') + '"']
+        if self.s.USE_SINGLE_QUOTE and single_quote_count < double_quote_count:
+            quote = "'"
+        for char in node.value:
+            if char in (quote, "\\"):
+                escaped += f"\\{char}"
+            elif 32 <= ord(char) < 127:
+                escaped += char
+            elif char in ESCAPE_CHARACTERS:
+                if quote == "" and char == "\n":
+                    escaped += "\n"
+                else:
+                    escaped += f"\\{ESCAPE_CHARACTERS[char]}"
+            else:
+                escaped += f"\\x{ord(char):02x}"
+        return [quote + escaped + quote]
 
     def visit_Table(self, node: Table) -> Retype:
         return ["{", *self._format_args(node.fields), "}"]
 
     def visit_Vararg(self, _node: Vararg) -> Retype:
         return ["..."]
 
     def visit_While(self, node: While) -> Retype:
         return [
             "while",
             Separators.Space,
             *self.visit(node.condition),
             Separators.Space,
-            "do",
-            Separators.Statement,
             *self.visit(node.body),
-            "end",
         ]
 
     def _need_brackets(
         self, own_node: BinOp, other_node: Expression, care_unop: bool
     ) -> bool:
         own_precedence: int = own_node.op.get_precedence()
         return (
@@ -242,79 +288,90 @@
         if self._need_brackets(node, node.right, False):
             result += ["(", *self.visit(node.right), ")"]
         else:
             result += self.visit(node.right)
         return result
 
     def visit_FunctionCall(self, node: FunctionCall) -> Retype:
-        return self.visit(node.function) + self._format_function_args(node.arguments)
+        return self._format_var(node.function) + self._format_function_args(
+            node.arguments
+        )
 
     def visit_FunctionDefinition(self, node: FunctionDefinition) -> Retype:
+        full_name: Retype = Separators.Dot.join(self.visit(name) for name in node.names)
+        if node.method_name:
+            full_name += [":", *self.visit(node.method_name)]
         return [
             "function",
             Separators.Space,
-            *Separators.Dot.join(self.visit(name) for name in node.names),
+            *full_name,
             "(",
             *self._format_args(node.parameters),
             ")",
-            Separators.Statement,
-            *self.visit(node.body),
-            "end",
+            *self.visit(node.body)[1:],
             Separators.Statement,
         ]
 
     def visit_IterativeFor(self, node: IterativeFor) -> Retype:
         return [
             "for",
             Separators.Space,
             *self._format_args(node.namelist),
             Separators.Space,
             "in",
             Separators.Space,
             *self._format_args(node.explist),
             Separators.Space,
-            "do",
-            Separators.Statement,
             *self.visit(node.body),
-            "end",
         ]
 
     def visit_LocalAssign(self, node: LocalAssign) -> Retype:
         result: Retype = ["local", Separators.Space]
-        result += Separators.Argument.join([str(arg)] for arg in node.variable_names)
+        names: list[Retype] = []
+        for name in node.variable_names:
+            if name.attribute:
+                names.append(
+                    [str(name.name), Separators.Space, "<", str(name.attribute), ">"]
+                )
+            else:
+                names.append([str(name.name)])
+        result += Separators.Argument.join(iter(names))
         if node.expressions:
             result += [Separators.Space, "=", Separators.Space]
             result += self._format_args(node.expressions)
         return result
 
     def visit_MethodInvocation(self, node: MethodInvocation) -> Retype:
         return [
-            *self.visit(node.function),
+            *self._format_var(node.function),
             ":",
             *self.visit(node.method),
             *self._format_function_args(node.arguments),
         ]
 
     def visit_NamedIndex(self, node: NamedIndex) -> Retype:
-        return [*self.visit(node.lhs), ".", *self.visit(node.variable_name)]
+        return [
+            *self._format_var(node.lhs),
+            Separators.Dot,
+            *self.visit(node.variable_name),
+        ]
 
     def visit_NumericFor(self, node: NumericFor) -> Retype:
         spaced_name: Retype = [
             Separators.Space,
-            self.visit(node.variable_name),
+            *self.visit(node.variable_name),
             Separators.Space,
         ]
         result: Retype = ["for", *spaced_name, "=", Separators.Space]
         result += self.visit(node.start)
-        result += [",", Separators.Space, *self.visit(node.stop)]
+        result += [Separators.Argument, *self.visit(node.stop)]
         if node.step:
-            result += [",", Separators.Space, *self.visit(node.step)]
-        result += [Separators.Space, "do", Separators.Statement]
+            result += [Separators.Argument, *self.visit(node.step)]
+        result.append(Separators.Space)
         result += self.visit(node.body)
-        result += ["end"]
         return result
 
     def visit_UnOp(self, node: UnOp) -> Retype:
         result: Retype = [node.op.value]
         if (
             self.s.ADD_ALL_BRACKETS
             or isinstance(node.right, BinOp)
@@ -324,48 +381,47 @@
         elif isinstance(node.right, UnOp) or node.op == UnaryOperand.NOT:
             result += [Separators.Space, *self.visit(node.right)]
         else:
             result += self.visit(node.right)
         return result
 
     def visit_ExpFunctionCall(self, node: ExpFunctionCall) -> Retype:
-        return self.visit(node.function) + self._format_function_args(node.arguments)
+        return self._format_var(node.function) + self._format_function_args(
+            node.arguments
+        )
 
     def visit_ExpFunctionDefinition(self, node: ExpFunctionDefinition) -> Retype:
         return [
             "function",
             Separators.Space,
             "(",
             *self._format_args(node.parameters),
             ")",
-            Separators.Statement,
-            *self.visit(node.body),
-            "end",
+            *self.visit(node.body)[1:],
         ]
 
     def visit_ExpMethodInvocation(self, node: ExpMethodInvocation) -> Retype:
         return [
-            *self.visit(node.function),
+            *self._format_var(node.function),
             ":",
             *self.visit(node.method),
             *self._format_function_args(node.arguments),
         ]
 
     def visit_LocalFunctionDefinition(self, node: LocalFunctionDefinition) -> Retype:
         return [
             "local",
+            Separators.Space,
             "function",
             Separators.Space,
             *self.visit(node.function_name),
             "(",
             *self._format_args(node.parameters),
             ")",
-            Separators.Statement,
-            *self.visit(node.body),
-            "end",
+            *self.visit(node.body)[1:],
             Separators.Statement,
         ]
 
     def visit_ExplicitTableField(self, node: ExplicitTableField) -> Retype:
         return [
             "[",
             *self.visit(node.at),
@@ -385,54 +441,82 @@
             *self.visit(node.value),
         ]
 
     def visit_NumberedTableField(self, node: NumberedTableField) -> Retype:
         return self.visit(node.value)
 
 
-def _sep_required(first: str, second: str) -> bool:
+def sep_required(first: str, second: str) -> bool:
+    """
+    Returns, whether a separator is strictly necessary between 2 tokens
+
+    :param first: last character of first token
+    :param second: first character of second token
+    :return: if the token is required
+    """
     return (
-        first in string.ascii_letters
-        and second in string.ascii_letters
-        or first in string.digits
-        and second in string.ascii_letters
-        or first in string.ascii_letters
-        and second in string.digits
+        first in string.ascii_letters + string.digits
+        and second in string.ascii_letters + string.digits
         or first == "-"
         and second == "-"
     )
 
 
-def _search_token(start_idx: int, direction: int, tokens: Retype) -> str | Separators:
+def search_token(
+    start_idx: int, direction: Literal[1, -1], tokens: Retype
+) -> str | Separators:
+    """
+    Search for a non indent/de-indent token.
+
+    :param start_idx: the first index to search
+    :param direction: in what direction to search, 1 for forwards and -1 for backwards
+    :param tokens: the token stream
+    :return: the closest non-indent token
+    """
     while isinstance(token := tokens[start_idx], Separators) and token in (
         Separators.Indent,
         Separators.DeIndent,
     ):
         start_idx += direction
     return token
 
 
-def _remove_separators(token_stream: Retype) -> None:
+def remove_separators(token_stream: Retype) -> None:
+    """
+    Remove all seperator tokens that are not strictly necessary.
+
+    :param token_stream: The token stream to filter. Removal happens in-place
+    :return: None
+    """
+    # Add a dummy token so that there is definitely a valid final token to look for
     token_stream.append("/")
     for i in range(len(token_stream) - 2, 0, -1):
         if isinstance(own_token := token_stream[i], Separators):
             if own_token not in (Separators.Space, Separators.Statement):
                 continue
-            previous_token = _search_token(i - 1, -1, token_stream)
-            next_token = _search_token(i + 1, 1, token_stream)
+            previous_token = search_token(i - 1, -1, token_stream)
+            next_token = search_token(i + 1, 1, token_stream)
             if (
                 isinstance(previous_token, Separators)
                 or isinstance(next_token, Separators)
-                or not _sep_required(previous_token[-1], next_token[0])
+                or not sep_required(previous_token[-1], next_token[0])
             ):
                 token_stream.pop(i)
+    # Remove the dummy token again
     token_stream.pop()
 
 
-def _resolve_tokens(token_stream: Retype, style: Type[FormattingStyle]) -> None:
+def resolve_tokens(token_stream: Retype, style: Type[FormattingStyle]) -> None:
+    """
+    Resolves all tokens except for Indent and DeIndent to strings.
+
+    :param token_stream: the token stream to resolve. Resolving happens in-place
+    :param style: The style object
+    :return: None
+    """
     newline: str = (
         style.STATEMENT_SEPARATOR if "\n" in style.STATEMENT_SEPARATOR else "\n"
     )
     for i, token in enumerate(token_stream):
         if isinstance(token, Separators):
             if token == Separators.Space:
                 token_stream[i] = " "
@@ -442,15 +526,22 @@
                 token_stream[i] = style.STATEMENT_SEPARATOR
             elif token == Separators.Argument:
                 token_stream[i] = style.ARGUMENT_SEPARATOR
             elif token == Separators.Newline:
                 token_stream[i] = newline
 
 
-def _indent(token_stream: Retype, indentation_str: str) -> None:
+def indent(token_stream: Retype, indentation_str: str) -> None:
+    """
+    Indent the token stream, adding indentation_str once per indentation level in front of existing tokens.
+
+    :param token_stream: the token stream to indent. Indentation happens in-place.
+    :param indentation_str: the string to use for indenting
+    :return: None
+    """
     indentation_level: int = 0
     indentation_dirty: bool = False
     for i, token in enumerate(token_stream):
         if isinstance(token, Separators):
             assert token in (Separators.Indent, Separators.DeIndent)
             if token == Separators.Indent:
                 indentation_level += 1
@@ -461,25 +552,38 @@
                 token_stream[i] = indentation_level * indentation_str + token
                 indentation_dirty = False
             if "\n" in token:
                 indentation_dirty = True
     assert indentation_level == 0
 
 
-def _join_tokens(token_stream: Retype) -> str:
+def join_tokens(token_stream: Retype) -> str:
+    """
+    Join all tokens into a string, ignoring all remaining Separators.
+
+    :param token_stream: The token stream to join
+    :return: The joined string
+    """
     result: str = ""
     for token in token_stream:
         if isinstance(token, str):
             result += token
     return result
 
 
 def format(ast: ASTNode, style: Optional[Type[FormattingStyle]] = None) -> str:
+    """
+    Format an ast tree according to the style class.
+
+    :param ast: The AST Node to format, usually a chunk
+    :param style: Optional style definition
+    :return: Formatted lua
+    """
     style = style or FormattingStyle
     formatter: Formatter = Formatter(style)
     token_stream: Retype = formatter.visit(ast)
     if style.REMOVE_UNNECESSARY_CHARS:
-        _remove_separators(token_stream)
-    token_stream[0:0] = ["--tumfl", Separators.Newline]
-    _resolve_tokens(token_stream, style)
-    _indent(token_stream, style.INDENTATION)
-    return _join_tokens(token_stream)
+        remove_separators(token_stream)
+    token_stream[0:0] = [f"--{style.COMMENT_SEP}tumfl", Separators.Newline]
+    resolve_tokens(token_stream, style)
+    indent(token_stream, style.INDENTATION)
+    return join_tokens(token_stream)
```

### Comparing `tumfl-0.1.7/tumfl/lexer.py` & `tumfl-0.1.8/tumfl/lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from typing import Dict, List, NoReturn, Optional, Tuple, TypedDict
 
-from .error import LexerException
+from .error import LexerError
 from .Token import Token, TokenType
 
 RESERVED_KEYWORDS: Dict[str, TokenType] = {
     t.value: t
     for t in list(TokenType)
     if t.value.isalpha() and t.value not in ["name", "number", "eof", "string"]
 }
@@ -44,37 +44,55 @@
 
 class TokenArgs(TypedDict):
     line: int
     column: int
     comment: list[str]
 
 
+def include_typing(do_include: bool) -> None:
+    """
+    Change the keywords to include typing
+
+    :param do_include: whether to include typing keywords
+    :return: None
+    """
+    if do_include and "as" not in RESERVED_KEYWORDS:
+        RESERVED_KEYWORDS["as"] = TokenType.AS
+        RESERVED_KEYWORDS["is"] = TokenType.IS
+    elif not do_include and "as" in RESERVED_KEYWORDS:
+        RESERVED_KEYWORDS.pop("as")
+        RESERVED_KEYWORDS.pop("is")
+
+
 class Lexer:
-    def __init__(self, text: str) -> None:
+    def __init__(
+        self, text: str, typed: bool = False, ignore_unicode_errors: bool = False
+    ) -> None:
         self.text: str = text
-        self.text_by_line: List[str] = text.split("\n")
         self.text_len: int = len(self.text)
         self.line: int = 0
         self.column: int = 0
         self.pos: int = 0
         self.newline_warn: int = 0
         self.current_char: Optional[str] = self.text[self.pos]
         self.last_hint: Optional[Tuple[str, int, int]] = None
         self.comments: list[str] = []
+        self.unicode_errors: str = "ignore" if ignore_unicode_errors else "strict"
+        include_typing(typed)
 
     def error(
         self, message: str, line: Optional[int] = None, column: Optional[int] = None
     ) -> NoReturn:
         current_line: int = line if line is not None else self.line
         current_column = column if column is not None else self.column
         print(f"Error on line {current_line + 1}:", file=sys.stderr)
-        print(self.text_by_line[current_line], file=sys.stderr)
+        print(self.text.split("\n")[current_line], file=sys.stderr)
         print(" " * current_column + "^", file=sys.stderr)
         print(message, file=sys.stderr)
-        raise LexerException(message, current_line, current_column)
+        raise LexerError(message, current_line, current_column)
 
     def get_token_args(self) -> TokenArgs:
         comment: list[str] = self.comments[:]
         self.comments.clear()
         return {"line": self.line + 1, "column": self.column + 1, "comment": comment}
 
     def advance(self) -> None:
@@ -236,14 +254,31 @@
         assert self.current_char in LETTER
         result: str = ""
         while self.current_char in ALPHANUMERIC:
             result += self.current_char
             self.advance()
         return result
 
+    def _safe_decode(self, base: int) -> str:
+        try:
+            return bytes((base,)).decode("utf-8", self.unicode_errors)
+        except UnicodeDecodeError:
+            self.error(
+                f"This library can't handle invalid unicode characters, got {base}"
+            )
+            assert False
+
+    def _safe_code_point(self, base: int) -> str:
+        try:
+            return chr(base)
+        except ValueError:
+            if self.unicode_errors == "strict":
+                self.error(f"Invalid unicode codepoint, got {base}")
+        return ""
+
     def get_string(self) -> str:
         assert self.current_char in ["'", '"']
         # character that is needed to close the string
         closing: str = self.current_char
         # whether the next character has been escaped
         escape: bool = False
         self.advance()
@@ -266,32 +301,50 @@
                     if self.current_char not in HEX_NUMBER:
                         self.error("Invalid hex digit", column=column)
                     self.advance()
                     digits += self.current_char
                     if self.current_char not in HEX_NUMBER:
                         self.error("Invalid hex digit", column=column)
                     self.advance()
-                    result += chr(int(digits, 16))
+                    result += self._safe_decode(int(digits, 16))
                 elif self.current_char == "u":
-                    print("Warning: ignoring unicode escape", file=sys.stderr)
+                    self.advance()
+                    if self.current_char != "{":
+                        self.error("Invalid character after \\u, expected {")
+                    self.advance()
+                    codepoint: str = ""
+                    for _ in range(8):
+                        codepoint += self.current_char
+                        if self.current_char not in HEX_NUMBER:
+                            self.error(
+                                "Invalid unicode codepoint, expected hexadecimal number"
+                            )
+                        self.advance()
+                        if self.current_char == "}":
+                            break
+                    else:
+                        self.error(
+                            "Unicode codepoints can be at most 2^31 - 1, did not close unicode escape"
+                        )
+                    result += self._safe_code_point(int(codepoint, 16))
                 # handle the decimal character specification case
                 elif self.current_char in NUMBER:
                     digits = self.current_char
                     self.advance()
                     # may have up to 3 digits
                     if self.current_char in NUMBER:
                         digits += self.current_char
                         self.advance()
                     if self.current_char in NUMBER:
                         digits += self.current_char
                         self.advance()
                     char: int = int(digits)
                     if char > 255:
                         self.error(f"Invalid char with number {char}", column=column)
-                    result += chr(char)
+                    result += self._safe_decode(char)
                 else:
                     # handle all simple escape sequences
                     if self.current_char not in ESCAPE_CODES:
                         self.error(
                             f"Invalid escape sequence: \\{self.current_char}",
                             column=column,
                         )
```

### Comparing `tumfl-0.1.7/tumfl/parser.py` & `tumfl-0.1.8/tumfl/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import sys
 from typing import Callable, NoReturn, Optional
 
 from .AST import *
 from .AST.BaseFunctionDefinition import BaseFunctionDefinition
-from .error import ParserException
+from .error import ParserError
 from .lexer import Lexer
 from .Token import Token, TokenType
 
 
 class Hint:
     def __init__(self, token: Token, where: str, what: str):
         self.token: Token = token
@@ -26,39 +26,43 @@
         TokenType.END,
         TokenType.RETURN,
         TokenType.UNTIL,
         TokenType.ELSEIF,
         TokenType.ELSE,
     )
 
-    def __init__(self, chunk: str):
+    def __init__(
+        self, chunk: str, typed: bool = False, ignore_unicode_errors: bool = False
+    ):
         self.chunk: str = chunk
-        self.lexer: Lexer = Lexer(self.chunk)
+        self.lexer: Lexer = Lexer(self.chunk, typed, ignore_unicode_errors)
         self.pos: int = 0
         self.current_token: Token = self.lexer.get_next_token()
         self.next_token: Token = self.lexer.get_next_token()
         self.context_hints: list[Hint] = []
+        self.typed: bool = typed
 
     def _error(self, message: str, token: Token) -> NoReturn:
         """Throw an error, prints out a description, and finally throws a value error"""
         current_line: int = token.line
         current_column = token.column
         print(f"Error on line {current_line}:", file=sys.stderr)
+        lines: list[str] = self.chunk.split("\n")
         if current_line > 1:
-            print(self.lexer.text_by_line[current_line - 2], file=sys.stderr)
-        print(self.lexer.text_by_line[current_line - 1], file=sys.stderr)
+            print(lines[current_line - 2], file=sys.stderr)
+        print(lines[current_line - 1], file=sys.stderr)
         print(" " * (current_column - 1) + "^", file=sys.stderr)
         print(message, file=sys.stderr)
         if self.context_hints:
             print(
                 "hints:",
                 " -> ".join(str(hint) for hint in self.context_hints),
                 file=sys.stderr,
             )
-        raise ParserException(message, self.context_hints, token)
+        raise ParserError(message, self.context_hints, token)
 
     def _assert(self, token_type: TokenType) -> None:
         """Assert that the current token is of a certain kind"""
         if self.current_token.type != token_type:
             self._error("Unexpected token", self.current_token)
 
     def _eat_token(self, token_type: Optional[TokenType] = None) -> None:
```

### Comparing `tumfl-0.1.7/tumfl/utils.py` & `tumfl-0.1.8/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.7/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.8/tumfl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumfl-0.1.7/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.8/tumfl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 README.md
 pyproject.toml
 setup.cfg
+test/test_dependency_resolver.py
 test/test_formatter.py
 test/test_lexer.py
 test/test_parser.py
 tumfl/Token.py
 tumfl/__init__.py
 tumfl/basic_walker.py
+tumfl/dependency_resolver.py
 tumfl/error.py
 tumfl/formatter.py
 tumfl/lexer.py
 tumfl/parser.py
 tumfl/utils.py
 tumfl.egg-info/PKG-INFO
 tumfl.egg-info/SOURCES.txt
```

