# Comparing `tmp/bytecodemanipulation-0.2.9.tar.gz` & `tmp/bytecodemanipulation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.2.9.tar", last modified: Thu May 11 11:41:26 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.3.1.tar", last modified: Sun Jun  4 20:18:54 2023, max compression
```

## Comparing `bytecodemanipulation-0.2.9.tar` & `bytecodemanipulation-0.3.1.tar`

### file list

```diff
@@ -1,153 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation/
--rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    56164 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunctionHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/Specialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/TypeEnforcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/annotated_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/AbstractBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/syntax_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.739894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/builtin_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.743894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.751894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    22643 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RawAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.751894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.755894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.755894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/specialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/mixin_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/optimise_self.py
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/optimiser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/bytecodemanipulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.735894 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 11:41:26.000000 bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-11 11:41:17.000000 bytecodemanipulation-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:41:26.763894 bytecodemanipulation-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    50753 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_InlineSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_Specializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_StandardLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 11:41:06.000000 bytecodemanipulation-0.2.9/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.018816 bytecodemanipulation-0.3.1/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/TypeEnforcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.026816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.034816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RawAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.034816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.038816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.038816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.042816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/specialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/mixin_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/CodeObjectBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/ExceptionTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24591 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-04 20:18:53.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-04 20:18:47.000000 bytecodemanipulation-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    52921 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_InlineSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Specializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.2.9/LICENSE` & `bytecodemanipulation-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/PKG-INFO` & `bytecodemanipulation-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.2.9
+Version: 0.3.1
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.2.9/README.md` & `bytecodemanipulation-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/Emulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import builtins
 import importlib
 import string
 import typing
 from inspect import CO_GENERATOR
 
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class UnknownOpcodeError(Exception):
     pass
 
 
 class FinalReturn(Exception):
@@ -90,23 +90,27 @@
         mutable = MutableFunction(mutable)
 
     mutable: MutableFunction
 
     if len(args) != mutable.argument_count:
         raise ValueError()
 
+    builder = mutable.create_filled_builder()
+
     stack = []
-    local_variables = [None] * len(mutable.shared_variable_names)
+    local_variables = [None] * len(builder.shared_variable_names)
     local_variables[: len(args)] = args
-    free_vars = [None] * len(mutable.free_variables)
+    free_vars = [None] * len(builder.free_variables)
     exception_handle_stack = []
 
-    instruction = mutable.instructions[0]
+    instruction = mutable.instruction_entry_point
     continue_stack = []
 
+    max_stack_size = mutable.calculate_max_stack_size()
+
     while True:
         print(instruction)
         print(stack)
         target = OPCODE_FUNCS[instruction.opcode]
 
         if target is None:
             raise UnknownOpcodeError(instruction)
@@ -125,16 +129,16 @@
             if len(e.args) > 1:
                 instruction, mutable = e.args[1:]
 
             return e.args[0]
         except YieldValue:
             raise RuntimeError("YIELD outside GENERATOR")
 
-        if len(stack) > mutable.stack_size:
-            raise StackSizeIssue(f"{len(stack)} > {mutable.stack_size}")
+        if len(stack) > max_stack_size:
+            raise StackSizeIssue(f"{len(stack)} > {max_stack_size}")
 
 
 OPCODE_FUNCS: typing.List[typing.Callable | None] = [None] * 256
 
 
 def execution(opcode: int):
     def target(
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/Mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from abc import ABC
 
 from bytecodemanipulation import Emulator
 
 from bytecodemanipulation.mixin_util import resolve_accesses
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.MutableFunctionHelpers import insert_method_into
-from bytecodemanipulation.MutableFunctionHelpers import MutableFunctionWithTree
 from bytecodemanipulation.Optimiser import _OptimisationContainer
 from bytecodemanipulation.util import AbstractInstructionWalker
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class MixinInjectionNotSupportedException(Exception):
     pass
 
 
 def _invoke_emulator(*args):
@@ -29,15 +28,14 @@
             self.target = target
             self.mixins: typing.List[Mixin._MixinHandle] = []
 
         def sort_and_apply(self):
             # todo: sort
 
             mutable = MutableFunction(self.target)
-            mutable.update_instruction_offsets(mutable.get_instructions())
 
             for mixin in self.mixins:
                 mixin.apply_on(mutable)
 
             try:
                 state = os.environ["DEBUG_MIXINS"]
             except KeyError:
@@ -476,32 +474,25 @@
         ):
             self.at = at
             self.inject = inject
 
         def apply_on(self, mutable: MutableFunction):
             protected_locals = resolve_accesses(mutable, self.inject)
 
-            if self.inject.shared_variable_names[0] in ("cls", "self"):
-                protected_locals.append(self.inject.shared_variable_names[0])
-
-            tree = MutableFunctionWithTree(mutable)
-
-            for position_instr in self.at.get_positions(mutable.instructions[0])[:]:
-                if position_instr not in mutable.instructions:
-                    continue
+            if self.inject.argument_names[0] in ("cls", "self"):
+                protected_locals.append(self.inject.argument_names[0])
 
+            for position_instr in self.at.get_positions(mutable.instruction_entry_point)[:]:
                 insert_method_into(
-                    tree,
+                    mutable,
                     position_instr.offset - 1,
                     self.inject,
                     protected_locals=protected_locals,
                 )
 
-                mutable.assemble_instructions_from_tree(tree.root)
-
     def __init__(
         self,
         target_class: str | typing.Type | typing.Callable[[], typing.Type],
         priority=0,
         optional=False,
         apply_on_others=True,
     ):
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
-from bytecodemanipulation.Opcodes import Opcodes, HAS_GLOBAL
-from bytecodemanipulation.Opcodes import UNCONDITIONAL_JUMPS
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes, HAS_GLOBAL
+from bytecodemanipulation.opcodes.Opcodes import UNCONDITIONAL_JUMPS
 
 
 class Guarantees:
     class AbstractGuarantee:
         pass
 
     RESULT_IS_CONSTANT = AbstractGuarantee()
@@ -65,180 +66,103 @@
                 or guarantee.arg_name == name_or_index
             ):
                 return False
 
         return True
 
 
-class MutableFunctionWithTree:
-    def __init__(self, mutable: MutableFunction, root: Instruction = None):
-        self.mutable = mutable
-        self.root = root or mutable.instructions[0]
-
-    def visitor(
-        self, visitor: typing.Callable[[Instruction, typing.List[Instruction]], None]
-    ):
-        def visit(
-            instruction: Instruction,
-            visited: typing.Set[Instruction],
-            path: typing.List[Instruction],
-        ):
-            visitor(instruction, path)
-
-            if instruction in visited:
-                return
-
-            visited.add(instruction)
-
-            if not instruction.has_stop_flow():
-                visit(instruction.next_instruction, visited, path + [instruction])
-
-            if instruction.has_jump():
-                # visit the jump target, but reset the instruction path, as we cannot make sure that
-                # it is the only path leading there
-                # TODO: is there a better way? (first visit the main tree, and than branch?)
-                visit(instruction.arg_value, visited, [instruction])
-
-        visit(self.root, set(), [])
-
-    def print_recursive(self, root: Instruction = None, visited: set = None, level=0):
-        if root is None:
-            print("Starting Dump...")
-            root = self.root
-
-        if visited is None:
-            visited = set()
-        elif root in visited:
-            return
-
-        print(
-            " " * level + repr(root),
-            "-> -1"
-            if root.next_instruction is None
-            else "-> " + str(root.next_instruction.offset),
-        )
-        visited.add(root)
-
-        if root.has_stop_flow():
-            return
-
-        if root.next_instruction is None:
-            print("-" * level, "END OF CONTROL FLOW")
-            return
-
-        self.print_recursive(root.next_instruction, visited, level)
-
-        if root.has_jump():
-            self.print_recursive(root.arg_value, visited, level + 1)
-
-
 def prefix_all_locals_with_all(
-    mutable: MutableFunction | MutableFunctionWithTree,
+    mutable: MutableFunction,
     prefix: str,
 ):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    mutable.shared_variable_names = [prefix + e for e in mutable.shared_variable_names]
-
-    for instruction in mutable.instructions:
-        if instruction.has_local():
-            instruction.change_arg(instruction.arg)
+    def add_prefix(instr: Instruction):
+        if instr.has_local():
+            instr.arg_value = prefix + instr.arg_value
+
+    mutable.walk_instructions(add_prefix)
 
 
 def prefix_all_locals_with_specified(
-    mutable: MutableFunction | MutableFunctionWithTree,
+    mutable: MutableFunction,
     prefix: str,
     protected_locals: typing.List[str] = tuple(),
 ):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    mutable.shared_variable_names = [
-        prefix + e if e not in protected_locals else e
-        for e in mutable.shared_variable_names
-    ]
-
-    for instruction in mutable.instructions:
-        if instruction.has_local():
-            instruction.update_owner(mutable, instruction.offset)
+    def add_prefix(instr: Instruction):
+        if instr.has_local() and instr.arg_value not in protected_locals:
+            instr.arg_value = prefix + instr.arg_value
+
+    mutable.walk_instructions(add_prefix)
 
 
 def replace_opcode_with_other(
-    mutable: MutableFunction | MutableFunctionWithTree,
+    mutable: MutableFunction,
     old_opcode: int,
     new_opcode: int,
     handle_new: typing.Callable[[Instruction], None] = lambda _: None,
 ):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
-    for instruction in mutable.instructions:
+    def replace(instruction: Instruction):
         if instruction.opcode == old_opcode:
             instruction.change_opcode(new_opcode)
 
             handle_new(instruction)
 
+    mutable.walk_instructions(replace)
+
 
 def inline_access_to_global(
-    mutable: MutableFunction | MutableFunctionWithTree, global_name: str, value=...
+    mutable: MutableFunction, global_name: str, value=...
 ):
-    if isinstance(mutable, MutableFunctionWithTree):
-        mutable.mutable.assemble_instructions_from_tree(mutable.root)
-        mutable = mutable.mutable
-
     if value == ...:
         value = mutable.target.__globals__[global_name]
 
-    for i, instruction in enumerate(mutable.instructions):
+    def replace(instruction: Instruction):
         if instruction.opcode == Opcodes.LOAD_GLOBAL:
             if instruction.arg_value == global_name:
                 instruction.change_opcode(Opcodes.LOAD_CONST)
                 instruction.change_arg_value(value)
 
+    mutable.walk_instructions(replace)
+
 
 def replace_const_func_call_with_opcode(
-    mutable: MutableFunctionWithTree,
+    mutable: MutableFunction,
     func: typing.Callable,
     opcode: int,
     handle_args: typing.Callable[
-        [MutableFunctionWithTree, Instruction, typing.List[Instruction]], bool
+        [MutableFunction, Instruction, typing.List[Instruction]], bool
     ],
 ):
-    def visitor(instruction: Instruction, path: typing.List[Instruction]):
+    def visitor(instruction: Instruction):
         if instruction.opcode == Opcodes.CALL_FUNCTION:
             counter = instruction.arg
-            args = path[-counter:]
-            load_method = path[-counter - 1]
+            args = [next(instruction.trace_stack_position(i)) for i in range(instruction.arg)]
+            load_method = next(instruction.trace_stack_position(instruction.arg))
 
             if (
                 load_method.opcode == Opcodes.LOAD_CONST
                 and load_method.arg_value == func
                 and all(instr.opcode == Opcodes.LOAD_CONST for instr in args)
             ):
                 instruction.change_opcode(opcode)
                 if not handle_args(mutable, instruction, args):
                     instruction.change_opcode(Opcodes.CALL_FUNCTION)
 
-    mutable.visitor(visitor)
+    mutable.walk_instructions(visitor)
 
 
 def capture_local(name: str):
     pass
 
 
 def outer_return(value=None):
     pass
 
 
 def _inline_capture_local(
-    tree: MutableFunctionWithTree,
+    mutable: MutableFunction,
     instruction: Instruction,
     args: typing.List[Instruction],
 ) -> bool:
     if len(args) != 1:
         return False
     if args[0].opcode != Opcodes.LOAD_CONST:
         return False
@@ -249,68 +173,76 @@
     args[0].arg = 0
     args[0].arg_value = None
 
     return True
 
 
 def _inline_outer_return(
-    tree: MutableFunctionWithTree,
+    mutable: MutableFunction,
     instruction: Instruction,
     args: typing.List[Instruction],
 ) -> bool:
     if len(args) > 1:
         return False
     if len(args) > 0 and args[0].opcode != Opcodes.LOAD_CONST:
         return False
 
     # In case we have no args, we need to add a LOAD_CONST(None)
     if len(args) == 0:
         instruction.change_opcode(Opcodes.LOAD_CONST)
         instruction.change_arg_value(None)
         return_instr = Instruction.create(Opcodes.RETURN_VALUE)
-        return_instr.update_owner(tree.mutable, -1)
+        return_instr.update_owner(mutable, -1)
         return_instr.next_instruction = instruction.next_instruction
         instruction.next_instruction = return_instr
 
     return True
 
 
 def insert_method_into(
-    body: MutableFunction | MutableFunctionWithTree,
-    offset: typing.Union[Instruction, int],
-    to_insert: MutableFunction | MutableFunctionWithTree,
+    body: MutableFunction,
+    entry_point: typing.Union[Instruction, int],
+    to_insert: MutableFunction,
     protected_locals: typing.List[str] = tuple(),
     drop_return_result=True,
 ):
     """
     Inserts the function AFTER the given offset / Instruction.
     If wanted at HEAD, set offset to -1
     """
 
-    if isinstance(to_insert, MutableFunctionWithTree):
-        to_insert.mutable.assemble_instructions_from_tree(to_insert.root)
-        to_insert = to_insert.mutable
+    if entry_point == -1:
+        HEAD_INSTRUCTION = Instruction.create("NOP")
+        HEAD_INSTRUCTION.function = body
+        HEAD_INSTRUCTION.next_instruction = body.instruction_entry_point
+        body.instruction_entry_point = HEAD_INSTRUCTION
+
+    elif isinstance(entry_point, int):
+        head = body.instruction_entry_point
+
+        for _ in range(entry_point):
+            if not head.has_unconditional_jump():
+                head = head.next_instruction
+            else:
+                head = head.arg_value
 
-    if not isinstance(body, MutableFunctionWithTree):
-        body = MutableFunctionWithTree(body)
+        HEAD_INSTRUCTION = head
+        del head
+
+    elif isinstance(entry_point, Instruction):
+        HEAD_INSTRUCTION = entry_point
 
-    if offset == -1:
-        HEAD_INSTRUCTION = Instruction.create("NOP")
-        HEAD_INSTRUCTION.function = body.mutable
-        HEAD_INSTRUCTION.next_instruction = body.root
-        body.root = HEAD_INSTRUCTION
-    elif isinstance(offset, int):
-        body.mutable.assemble_instructions_from_tree(body.root)
-        HEAD_INSTRUCTION = body.mutable.instructions[offset]
     else:
-        HEAD_INSTRUCTION = offset
+        raise ValueError(entry_point)
 
-    for instr in to_insert.instructions:
+    def set_offset(instr):
         instr.offset = -1
 
+    to_insert.walk_instructions(set_offset)
+
     if protected_locals is not None:
         prefix_all_locals_with_specified(
             to_insert, to_insert.function_name + ":", protected_locals
         )
     else:
         prefix_all_locals_with_all(to_insert, to_insert.function_name + ":")
 
@@ -318,112 +250,83 @@
         to_insert, Opcodes.RETURN_VALUE, Opcodes.INTERMEDIATE_INNER_RETURN
     )
     inline_access_to_global(to_insert, "capture_local", capture_local)
     inline_access_to_global(to_insert, "outer_return", outer_return)
 
     # MutableFunctionWithTree(to_insert).print_recursive()
 
-    instr = None
-    previous = None
-    for instr in to_insert.instructions:
+    instr: Instruction = None
+    previous: Instruction = None
+
+    def visit(instr):
+        nonlocal previous
+
         if previous is not None:
             previous.next_instruction = instr
 
         if instr.opcode == Opcodes.INTERMEDIATE_INNER_RETURN:
             if drop_return_result:
                 previous.insert_after(Instruction(to_insert, -1, Opcodes.POP_TOP))
 
             instr.change_opcode(
                 Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
             )
 
         previous = instr
 
+    to_insert.walk_instructions(visit)
+
     if instr is not None and instr.next_instruction is None:
         instr.next_instruction = HEAD_INSTRUCTION.next_instruction
 
-    to_insert.assemble_instructions_from_tree(
-        to_insert.instructions[0],
-        breaks_flow=(
-            Instruction.create(
-                Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
-            ),
-        ),
-    )
-    # MutableFunctionWithTree(to_insert).print_recursive()
-    # to_insert.decode_instructions()
+    def visit(instr):
+        instr.update_owner(body, -1, False)
 
-    for instr in to_insert.instructions:
-        instr.update_owner(body.mutable, -1, False)
+    to_insert.walk_instructions(visit)
 
-    to_insert_tree = MutableFunctionWithTree(to_insert)
-    # to_insert_tree.print_recursive()
     replace_const_func_call_with_opcode(
-        to_insert_tree,
+        to_insert,
         capture_local,
         Opcodes.LOAD_FAST,
         _inline_capture_local,
     )
-    # to_insert_tree.print_recursive()
     replace_const_func_call_with_opcode(
-        to_insert_tree,
+        to_insert,
         outer_return,
         Opcodes.RETURN_VALUE,
         _inline_outer_return,
     )
-    # to_insert_tree.print_recursive()
-
-    def visit(instruction: Instruction, path):
-        if instruction is None:
-            print(path)
-            raise
-
-        instruction.function = body.mutable
-
-        if instruction.has_constant():
-            instruction.arg = body.mutable.allocate_shared_constant(
-                instruction.arg_value
-            )
 
-        elif instruction.has_name():
-            instruction.arg = body.mutable.allocate_shared_name(instruction.arg_value)
+    HEAD_INSTRUCTION.next_instruction = to_insert.instruction_entry_point
 
-        elif instruction.has_local():
-            instruction.arg = body.mutable.allocate_shared_variable_name(
-                instruction.arg_value
-            )
-
-    HEAD_INSTRUCTION.next_instruction = to_insert_tree.root
-    body.visitor(visit)
-
-    # body.print_recursive()
-
-    body.mutable.assemble_instructions_from_tree(body.root)
-
-    # body.print_recursive()
 
-
-def inline_calls_to_const_functions(mutable: MutableFunction):
+def inline_calls_to_const_functions(mutable: MutableFunction, builder):
     from bytecodemanipulation.Optimiser import _OptimisationContainer
 
-    for instr in mutable.instructions[:]:
+    dirty = False
+
+    def visit(instr: Instruction):
         if instr.opcode == Opcodes.CALL_FUNCTION:
             source = next(instr.trace_stack_position(instr.arg))
 
             if source.opcode != Opcodes.LOAD_CONST:
-                continue
+                return
 
             target = source.arg_value
 
             container = _OptimisationContainer.get_for_target(target)
             if not container.try_inline_calls:
-                continue
+                return
 
             instr.change_opcode(Opcodes.NOP)
             insert_method_into(
                 mutable,
                 instr.offset,
                 MutableFunction(target),
                 drop_return_result=False,
-                protected_locals=None,
             )
             source.change_opcode(Opcodes.NOP)
+            nonlocal dirty
+            dirty = True
+
+    mutable.walk_instructions(visit)
+    return dirty
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/Opcodes.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Opcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,35 +179,36 @@
         CALL = 189
         KW_NAMES = 190
         POP_JUMP_BACKWARD_IF_NOT_NONE = 191
         POP_JUMP_BACKWARD_IF_NONE = 192
         POP_JUMP_BACKWARD_IF_FALSE = 193
         POP_JUMP_BACKWARD_IF_TRUE = 194
 
-    INTERMEDIATE_INNER_RETURN = 256
-    INTERMEDIATE_OUTER_RETURN = 257
-    INTERMEDIATE_LOAD_FAST = 258
-    BYTECODE_LABEL = 259
-    MACRO_PARAMETER_EXPANSION = 260
-    STATIC_ATTRIBUTE_ACCESS = 261
-    MACRO_RETURN_VALUE = 262
-    MACRO_LOAD_PARAMETER = 263
-    MACRO_STORE_PARAMETER = 264
+    INTERMEDIATE_INNER_RETURN = -1
+    INTERMEDIATE_OUTER_RETURN = -1
+    INTERMEDIATE_LOAD_FAST = -1
+    BYTECODE_LABEL = -1
+    MACRO_PARAMETER_EXPANSION = -1
+    STATIC_ATTRIBUTE_ACCESS = -1
+    MACRO_RETURN_VALUE = -1
+    MACRO_LOAD_PARAMETER = -1
+    MACRO_STORE_PARAMETER = -1
 
 
 OPCODE2NAME = {}
 OPNAME2CODE = {}
 
 
 def init_maps():
     OPNAME2CODE.clear()
     OPCODE2NAME.clear()
 
     for key, value in Opcodes.__dict__.items():
         key: str
+
         if key.isupper() and isinstance(value, int):
             OPNAME2CODE[key] = value
             OPCODE2NAME[value] = key
 
 
 END_CONTROL_FLOW: typing.List[int] = []
 HAS_NAME: typing.List[int] = []
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/Optimiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import types
 import typing
 import builtins
 import random
 
 from bytecodemanipulation.MutableFunctionHelpers import Guarantees
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.optimiser_util import inline_const_value_pop_pairs
 from bytecodemanipulation.optimiser_util import inline_constant_binary_ops
 from bytecodemanipulation.optimiser_util import inline_constant_method_invokes
 from bytecodemanipulation.optimiser_util import inline_static_attribute_access
 from bytecodemanipulation.optimiser_util import remove_branch_on_constant
 from bytecodemanipulation.optimiser_util import remove_local_var_assign_without_use
 from bytecodemanipulation.optimiser_util import remove_nops
@@ -256,68 +257,64 @@
         mutable.prepare_previous_instructions()
 
         # Walk over the code and resolve cached globals
         self._inline_load_globals(mutable)
 
         # Walk over the entries as long as the optimisers are doing their stuff
         while True:
-            mutable.assemble_instructions_from_tree(
-                mutable.instructions[0].optimise_tree()
-            )
-            mutable.prepare_previous_instructions()
+            builder = mutable.create_filled_builder()
+            # mutable.prepare_previous_instructions()
 
             dirty = False
             for optimiser in self.optimisations:
-                dirty = optimiser.apply(self, mutable) or dirty
+                dirty = optimiser.apply(self, mutable, builder) or dirty
 
             if dirty:
                 continue
 
-            if inline_const_value_pop_pairs(mutable):
+            if inline_const_value_pop_pairs(mutable, builder):
                 continue
 
-            if remove_local_var_assign_without_use(mutable):
+            if remove_local_var_assign_without_use(mutable, builder):
                 continue
 
             # Inlines access to static items
-            if inline_static_attribute_access(mutable):
+            if inline_static_attribute_access(mutable, builder):
                 continue
 
             # Inline invokes to builtins and other known is_constant_op-s with static args
-            if inline_constant_method_invokes(mutable):
+            if inline_constant_method_invokes(mutable, builder):
                 continue
 
             # Resolve known constant types
-            if self._resolve_constant_local_types(mutable):
+            if self._resolve_constant_local_types(mutable, builder):
                 continue
             # self._resolve_constant_local_attr_types(mutable)
             # todo: use return type of known functions
 
-            if inline_constant_binary_ops(mutable):
+            if inline_constant_binary_ops(mutable, builder):
                 continue
 
             # apply optimisation specialisations
-            if apply_specializations(mutable):
+            if apply_specializations(mutable, builder):
                 continue
 
             # Inline invokes to builtins and other known is_constant_op-s with static args
-            if inline_constant_method_invokes(mutable):
+            if inline_constant_method_invokes(mutable, builder):
                 continue
 
             # Remove conditional jumps no longer required
-            if remove_branch_on_constant(mutable):
+            if remove_branch_on_constant(mutable, builder):
                 continue
 
-            if inline_calls_to_const_functions(mutable):
+            if inline_calls_to_const_functions(mutable, builder):
                 continue
 
             break
 
-        mutable.assemble_instructions_from_tree(mutable.instructions[0].optimise_tree())
-
         mutable.reassign_to_function()
 
         # print(mutable)
 
     def _resolve_lazy_references(self):
         try:
             for key, lazy in self.lazy_global_name_cache.items():
@@ -348,63 +345,70 @@
         except:
             print(self.target)
             raise
 
     def _inline_load_globals(self, mutable: MutableFunction) -> bool:
         dirty = False
 
-        for instruction in mutable.instructions:
+        def inline(instruction: Instruction):
             if instruction.opcode == Opcodes.LOAD_GLOBAL:
                 if instruction.arg_value in self.dereference_global_name_cache:
                     name = instruction.arg_value
                     instruction.change_opcode(Opcodes.LOAD_CONST)
                     instruction.change_arg_value(
                         self.dereference_global_name_cache[name]
                     )
+                    nonlocal dirty
                     dirty = True
 
             elif instruction.opcode in (Opcodes.STORE_GLOBAL, Opcodes.DELETE_GLOBAL):
                 if (
                     instruction.arg_value in self.dereference_global_name_cache
                     and instruction.arg_value not in self.unsafe_global_writes_allowed
                 ):
                     raise BreaksOwnGuaranteesException(
                         f"Global {instruction.arg_value} is cached but written to!"
                     )
 
+        mutable.walk_instructions(inline)
+
         return dirty
 
-    def _resolve_constant_local_types(self, mutable: MutableFunction) -> bool:
+    def _resolve_constant_local_types(self, mutable: MutableFunction, builder) -> bool:
         dirty = False
 
-        for instruction in mutable.instructions:
+        def visit(instruction: Instruction):
             if instruction.opcode == Opcodes.LOAD_ATTR:
                 try:
                     source = next(instruction.trace_stack_position(0))
                 except StopIteration:
-                    continue
+                    return
 
                 if source.opcode in (Opcodes.LOAD_FAST, Opcodes.LOAD_METHOD):
                     if source.arg_value not in self.dereference_local_var_type:
-                        continue
+                        return
 
                     data_type = self.dereference_local_var_type[source.arg_value]
 
                     if not hasattr(data_type, instruction.arg_value):
-                        continue
+                        return
 
                     # todo: check for dynamic class variables!
 
                     attr = getattr(data_type, instruction.arg_value)
 
                     instruction.change_opcode(Opcodes.LOAD_CONST)
                     instruction.change_arg_value(attr)
                     source.change_opcode(Opcodes.NOP)
+
+                    nonlocal dirty
                     dirty = True
 
+        mutable.walk_instructions(visit)
+
         return dirty
 
 
 _OptimisationContainer.get_for_target(typing).is_static = True
 _OptimisationContainer.get_for_target(random).is_static = True
 _OptimisationContainer.get_for_target(string).is_static = True
 _OptimisationContainer.get_for_target(re).is_static = True
@@ -414,19 +418,19 @@
 
 
 class AbstractOptimisationWalker:
     """
     Optimisation walker for classes and functions, constructed by the optimiser annotations
     """
 
-    def apply(
-        self, container: "_OptimisationContainer", mutable: MutableFunction
-    ) -> bool:
+    def apply(self, container: "_OptimisationContainer", mutable: MutableFunction, builder) -> bool:
         """
         Applies this optimisation on the given container with the MutableFunction as target
+        :param builder:
+        :type builder:
         """
         raise NotImplementedError
 
 
 def cache_global_name(
     name: str,
     accessor: typing.Callable[[], object] = None,
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/Specialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 import warnings
 
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class TypeAnnotation:
     pass
 
 
 class MethodCallDescriptor:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/AbstractBase.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/AbstractBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import types
 import typing
 from abc import ABC
 
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class ParsingScope:
     @classmethod
     def create_for_module(cls, module: types.ModuleType):
         scope = cls()
@@ -189,14 +189,20 @@
         return visitor(self, tuple(), parents)
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         pass
 
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        raise NotImplementedError
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return tuple()
+
 
 class AbstractAccessExpression(AbstractSourceExpression, ABC):
     PREFIX: str | None = None
     IS_STATIC = False
 
     def __init__(
         self,
@@ -232,24 +238,30 @@
         return f"-> Label('{self.name}')"
 
 
 class IIdentifierAccessor:
     def __call__(self, scope: ParsingScope):
         raise NotImplementedError
 
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return tuple()
+
 
 class MacroExpandedIdentifier(IIdentifierAccessor):
     def __init__(
         self,
         macro_name: typing.Union[str, "IIdentifierAccessor"],
         token: typing.List[AbstractToken] = None,
     ):
         self.macro_name = macro_name
         self.token = token
 
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return self.token
+
     def __hash__(self):
         return hash(self.macro_name)
 
     def __eq__(self, other):
         if isinstance(other, MacroExpandedIdentifier):
             return self.macro_name == other.macro_name
         return False
@@ -310,15 +322,15 @@
             scope,
             self.token,
             f"Expected <static evaluated expression> for getting the name for storing, got {value}",
         )
 
 
 class StaticIdentifier(IIdentifierAccessor):
-    def __init__(self, name: str):
+    def __init__(self, name: str, token: AbstractToken = None):
         self.name = name
 
     def __eq__(self, other):
         return (
             isinstance(other, StaticIdentifier) and self.name == other.name
         ) or self.name == other
 
@@ -326,7 +338,10 @@
         return hash(self.name)
 
     def __repr__(self):
         return repr(self.name)
 
     def __call__(self, scope: ParsingScope):
         return self.name
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Emitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import dis
 import string
 import types
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import Lexer
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.CodeObjectBuilder import CodeObjectBuilder
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.assembler.Parser import (
     Parser as AssemblyParser,
 )
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler import target as assembly_targets
 from bytecodemanipulation.util import LambdaInstructionWalker
@@ -44,29 +46,30 @@
     return eff, max_size
 
 
 GLOBAL_SCOPE_CACHE: typing.Dict[str, dict] = {}
 
 
 def apply_inline_assemblies(
-    target: MutableFunction | typing.Callable, store_at_target: bool = None
+    target: MutableFunction | typing.Callable, builder: CodeObjectBuilder = None, store_at_target: bool = None
 ):
     """
     Processes all assembly() calls and label() calls in 'target'
     """
-
     if not isinstance(target, MutableFunction):
         target = MutableFunction(target)
         if store_at_target is None:
             store_at_target = True
 
+    builder = builder or target.create_filled_builder()
+
     labels = set()
     insertion_points: typing.List[typing.Tuple[str, Instruction]] = []
 
-    for instr in target.instructions[:]:
+    for instr in builder.temporary_instructions[:]:
         if instr.opcode == Opcodes.LOAD_GLOBAL:
             try:
                 value = target.target.__globals__.get(instr.arg_value)
             except KeyError:
                 continue
 
             if value == assembly_targets.assembly:
@@ -221,19 +224,19 @@
                     print("error: ", ins)
 
                 ins.change_opcode(Opcodes.NOP)
                 ins.next_instruction = (
                     bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
                 )
 
-    for i, ins in enumerate(target.instructions):
+    for i, ins in enumerate(builder.temporary_instructions):
         if ins.opcode == Opcodes.BYTECODE_LABEL:
             label_targets[ins.arg_value] = ins.next_instruction
             ins.change_opcode(Opcodes.NOP)
-            ins.next_instruction = target.instructions[i + 1]
+            ins.next_instruction = builder.temporary_instructions[i + 1]
 
     pending: typing.List[Instruction] = []
 
     def resolve_special_code(ins: Instruction, *_):
         # print(ins)
         if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
             ins.change_arg_value(label_targets[ins.arg_value.name])
@@ -247,24 +250,22 @@
 
             obj = source.arg_value
             source.change_opcode(Opcodes.NOP, update_next=False)
             ins.change_opcode(
                 Opcodes.LOAD_CONST, getattr(obj, ins.arg_value), update_next=False
             )
 
-    target.instructions[0].apply_value_visitor(resolve_special_code)
+    target.walk_instructions(resolve_special_code)
 
     while pending:
         pending.pop().apply_value_visitor(resolve_special_code)
 
-    target.stack_size += max(max_stack_effects)
-
     # target.instructions[0].apply_value_visitor(lambda instr, *_: print(instr))
 
-    target.assemble_instructions_from_tree(target.instructions[0])
+    # target.assemble_instructions_from_tree(target.instructions[0])
 
     if store_at_target:
         target.reassign_to_function()
 
     return target
 
 
@@ -285,15 +286,16 @@
 
     asm = AssemblyParser(asm_code, scope).parse()
     scope.labels = asm.get_labels(scope)
     # asm.fill_scope_complete(scope)
     scope.scope_path.clear()
     create_function = lambda m: None
     target = MutableFunction(create_function)
-    target.shared_variable_names[0] = "$module$"
+    target.argument_names[0] = "$module$"
+
     bytecode = asm.create_bytecode(target, scope)
 
     if bytecode is None:
         return
 
     label_targets = {}
     for ins in bytecode:
@@ -312,23 +314,19 @@
         instr.update_owner(
             target, -1, force_change_arg_index=True, update_following=False
         )
 
     if not bytecode:
         bytecode.append(Instruction(target, -1, "NOP"))
 
-    bytecode[-1].next_instruction = target.instructions[0]
-    target.assemble_instructions_from_tree(bytecode[0])
+    bytecode[-1].next_instruction = target.instruction_entry_point
 
-    target.instructions[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
-    target.stack_size = bytecode[0].apply_value_visitor(_visit_for_stack_effect)[1]
+    target.walk_instructions(resolve_jump_to_label)
 
-    target.assemble_instructions_from_tree(target.instructions[0])
-
-    for instr in target.instructions:
+    for instr in bytecode:
         if instr.opcode == Opcodes.STORE_FAST:
             load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
             store = Instruction(target, -1, Opcodes.STORE_ATTR, instr.arg_value)
 
             instr.change_opcode(Opcodes.NOP)
             instr.insert_after([load_module, store])
 
@@ -342,15 +340,17 @@
         elif instr.opcode == Opcodes.DELETE_FAST:
             load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
             delete = Instruction(target, -1, Opcodes.DELETE_ATTR, instr.arg_value)
 
             instr.change_opcode(Opcodes.NOP)
             instr.insert_after([load_module, delete])
 
-    target.assemble_instructions_from_tree(target.instructions[0])
     target.function_name = module.__name__
 
+    target.instruction_entry_point = bytecode[0]
+    target.prepare_previous_instructions()
+
     target.reassign_to_function()
 
     # dis.dis(target)
 
     create_function(module)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Lexer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/Parser.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     SubscriptionAccessExpression,
 )
 from bytecodemanipulation.data.shared.expressions.TopOfStackAccessExpression import (
     TopOfStackAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
 
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 
 from bytecodemanipulation.assembler.Lexer import (
     Lexer,
     SpecialToken,
     StringLiteralToken,
 )
 
@@ -543,15 +543,15 @@
         self.rollback()
 
     def try_parse_identifier_like(self) -> IIdentifierAccessor | None:
         if expr := self.try_consume_multi([SpecialToken("&"), IdentifierToken]):
             return MacroExpandedIdentifier(expr[1].text, expr)
 
         if expr := self.try_consume(IdentifierToken):
-            return StaticIdentifier(expr.text)
+            return StaticIdentifier(expr.text, expr)
 
     def parse_identifier_like(self, scope: ParsingScope) -> IIdentifierAccessor:
         identifier = self.try_parse_identifier_like()
 
         if identifier is None:
             raise throw_positioned_syntax_error(
                 scope,
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/hook.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/hook.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/syntax_errors.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/syntax_errors.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,19 +66,19 @@
         mutable = bytecodemanipulation.MutableFunction.MutableFunction(function)
 
         macro_asm = MacroAssembly(
             [IdentifierToken(macro_name[-1])],
             [
                 # todo: add data type here!
                 MacroAssembly.MacroArg(IdentifierToken(name))
-                for name in mutable.shared_variable_names[: mutable.argument_count]
+                for name in mutable.argument_names
             ],
             MacroAssembly.Function2CompoundMapper(
                 function,
-                scoped_names=mutable.shared_variable_names[: mutable.argument_count],
+                scoped_names=mutable.argument_names,
             ),
         )
 
         namespace = macro_name.split(":")[:-1]
 
         scope = bytecodemanipulation.assembler.AbstractBase.ParsingScope.create_for_function(
             function
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/parser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 import random
 
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.Specialization import SpecializationContainer, register
-from bytecodemanipulation.MutableFunction import Instruction
-
+from bytecodemanipulation.opcodes.Instruction import Instruction
 
 ASSERT_TYPE_CASTS = False
 DISCARD_ALL_ANY_WITHOUT_SIDE_EFFECT_CHECK = True
 
 
 @register(typing.cast)
 def specialize_typing_cast(container: SpecializationContainer):
@@ -429,26 +428,47 @@
     elif arg_count != create_primitive_arg.arg:
         create_primitive_arg.change_arg(arg_count)
 
         container.no_special = False
 
 
 @register(sum)
-def specialize_any(container: SpecializationContainer):
+def specialize_sum(container: SpecializationContainer):
     args = container.get_arg_specifications()
 
     if len(args) == 1:
         if args[0].get_normalized_data_instr().opcode == Opcodes.LOAD_CONST:
-            container.replace_with_constant_value(
-                sum(args[0].get_normalized_data_instr().arg_value)
-            )
+            obj = args[0].get_normalized_data_instr().arg_value
+
+            if None in obj:
+                container.replace_with_raise_exception(
+                    TypeError(
+                        "TypeError: unsupported operand type(s) for +: 'int' and 'NoneType'"
+                    )
+                )
+                return
+
+            container.replace_with_constant_value(sum(obj))
+
         elif args[0].get_normalized_data_instr().opcode in (
             Opcodes.BUILD_LIST,
             Opcodes.BUILD_TUPLE,
             Opcodes.BUILD_SET,
         ):
+            for source in [
+                next(args[0].get_normalized_data_instr().trace_stack_position(i))
+                for i in range(args[0].get_normalized_data_instr().arg)
+            ]:
+                if source.opcode == Opcodes.LOAD_CONST and source.arg_value is None:
+                    container.replace_with_raise_exception(
+                        TypeError(
+                            "TypeError: unsupported operand type(s) for +: 'int' and 'NoneType'"
+                        )
+                    )
+                    return
+
             count = args[0].get_normalized_data_instr().arg
             args[0].get_normalized_data_instr().change_opcode(Opcodes.NOP)
             container.replace_call_with_opcodes(
                 [Instruction(None, -1, Opcodes.BINARY_ADD) for _ in range(count - 1)],
                 leave_args_on_stack=True,
             )
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
+from bytecodemanipulation.assembler.AbstractBase import (
+    IIdentifierAccessor,
+    StaticIdentifier,
+)
 
 
 class AttributeAccessExpression(AbstractAccessExpression):
-    def __init__(
-        self, root: AbstractAccessExpression, name: IIdentifierAccessor | str
-    ):
+    def __init__(self, root: AbstractAccessExpression, name: IIdentifierAccessor | str):
         self.root = root
-        self.name = (
-            name
-            if not isinstance(name, str)
-            else StaticIdentifier(name)
-        )
+        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
             and self.name == other.name
         )
@@ -34,32 +32,42 @@
     def copy(self) -> "AttributeAccessExpression":
         return AttributeAccessExpression(self.root.copy(), self.name)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
-            Instruction(
-                function, -1, "LOAD_ATTR", self.name(scope)
-            )
+            Instruction(function, -1, "LOAD_ATTR", self.name(scope))
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
-            Instruction(
-                function, -1, "STORE_ATTR", self.name(scope)
-            )
+            Instruction(function, -1, "STORE_ATTR", self.name(scope))
         ]
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
             self, (self.root.visit_parts(visitor, parents + [self]),), parents
         )
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (
+            list(self.root.get_tokens()) + list(self.name.get_tokens()) + [self.token]
+        )
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        base = self.root.evaluate_static_value(scope)
+        name = self.name(scope)
+
+        if not hasattr(base, name):
+            raise NotImplementedError
+
+        return getattr(base, name)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/CompoundExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/CompoundExpression.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class CompoundExpression(AbstractExpression, IAssemblyStructureVisitable):
     def __init__(self, children: typing.List[AbstractExpression] = None):
         self.children = children or []
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class ConstantAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
 
     def __init__(self, value, token: AbstractToken = None):
@@ -32,7 +32,13 @@
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise throw_positioned_syntax_error(
             scope, self.token, f"Cannot assign to a constant: {self}"
         )
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        return self.value
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.data.shared.instructions.YieldAssembly import (
+    AbstractYieldAssembly,
+)
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class DerefAccessExpression(AbstractAccessExpression):
-    PREFIX = "§"
-
+@Parser.register
+class YieldAssembly(AbstractYieldAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
+        bytecode = []
 
-        if value.isdigit():
-            value = int(value)
+        if self.expr:
+            bytecode += self.expr.emit_bytecodes(function, scope)
 
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, "LOAD_DEREF", value, _decode_next=False
-            )
-        ]
+        if self.is_star:
+            bytecode += [
+                Instruction(function, -1, Opcodes.GET_YIELD_FROM_ITER),
+                Instruction(function, -1, Opcodes.LOAD_CONST, None),
+                Instruction(function, -1, Opcodes.YIELD_FROM),
+            ]
 
-    def emit_store_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
+        else:
+            bytecode += [
+                Instruction(function, -1, Opcodes.YIELD_VALUE),
+            ]
+
+        if self.target:
+            bytecode += self.target.emit_store_bytecodes(function, scope)
+
+        else:
+            bytecode += [Instruction(function, -1, Opcodes.POP_TOP)]
 
-        if value.isdigit():
-            value = int(value)
+        # print(bytecode)
 
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, "STORE_DEREF", value
-            )
-        ]
+        return bytecode
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class DiscardValueExpression(AbstractAccessExpression):
     def __init__(self, token=None):
         self.token = token
 
     def emit_bytecodes(
@@ -16,7 +17,10 @@
     ) -> typing.List[Instruction]:
         raise RuntimeError
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return [Instruction(function, -1, Opcodes.POP_TOP)]
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class DynamicAttributeAccessExpression(AbstractAccessExpression):
     def __init__(
         self, root: AbstractAccessExpression, name_expr: AbstractSourceExpression
     ):
         self.root = root
@@ -60,7 +61,19 @@
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
             self, (self.root.visit_parts(visitor, parents + [self]),), parents
         )
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        base = self.root.evaluate_static_value(scope)
+        name = self.name_expr.evaluate_static_value(scope)
+
+        if not hasattr(base, name):
+            raise NotImplementedError
+
+        return getattr(base, name)
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return list(self.root.get_tokens()) + list(self.name_expr.get_tokens())
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+import builtins
+import types
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class GlobalAccessExpression(AbstractAccessExpression):
-    PREFIX = "@"
+class ModuleAccessExpression(AbstractAccessExpression):
+    IS_STATIC = True
+    PREFIX = "~"
+    _CACHE = builtins.__dict__.copy()
+
+    @classmethod
+    def _cached_lookup(cls, module_name: str) -> types.ModuleType:
+        if module_name not in cls._CACHE:
+            module = cls._CACHE[module_name] = __import__(module_name)
+            return module
+
+        return cls._CACHE[module_name]
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value.isdigit():
-            value = int(value)
-
+        value = self._cached_lookup(self.get_name(scope))
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "LOAD_GLOBAL", value
+                self.token, function, -1, Opcodes.LOAD_CONST, value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value.isdigit():
-            value = int(value)
+        raise RuntimeError
 
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, "STORE_GLOBAL", value
-            )
-        ]
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        return self._cached_lookup(self.get_name(scope))
 
-    def get_static_value(self, scope: ParsingScope) -> typing.Any:
-        raise ValueError("not implemented")
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import builtins
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class GlobalStaticAccessExpression(AbstractAccessExpression):
     PREFIX = "@!"
     IS_STATIC = True
 
@@ -27,17 +28,20 @@
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise RuntimeError("Cannot assign to a constant global")
 
-    def get_static_value(self, scope: ParsingScope) -> typing.Any:
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         if self.get_name(scope) in scope.globals_dict:
             return scope.globals_dict[self.get_name(scope)]
 
         raise throw_positioned_syntax_error(
             scope,
             self.token,
             f"Name {self.get_name(scope)} not found!",
             NameError,
         )
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
-class LocalAccessExpression(AbstractAccessExpression):
-    PREFIX = "$"
+class GlobalAccessExpression(AbstractAccessExpression):
+    PREFIX = "@"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "LOAD_FAST", value, _decode_next=False
+                self.token, function, -1, "LOAD_GLOBAL", value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
-            Instruction.create_with_token(self.token, function, -1, "STORE_FAST", value)
+            Instruction.create_with_token(
+                self.token, function, -1, "STORE_GLOBAL", value
+            )
         ]
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        raise NotImplementedError  # todo: implement in some cases
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class MacroAccessExpression(AbstractAccessExpression):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
@@ -25,7 +26,13 @@
         return type(self) is type(other) and self.name == other.name
 
     def __repr__(self):
         return f"MACRO-LINK({':'.join(map(lambda e: e.text, self.name))})"
 
     def copy(self) -> "MacroAccessExpression":
         return type(self)(self.name.copy())
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        raise NotImplementedError  # todo: implement in some cases
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return self.name
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class MacroParameterAccessExpression(AbstractAccessExpression):
     PREFIX = "&"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
@@ -52,7 +53,18 @@
             )
 
         return [
             Instruction.create_with_token(
                 self.token, function, -1, Opcodes.MACRO_STORE_PARAMETER, value
             )
         ]
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        name = self.name(scope)
+
+        if name not in scope.macro_parameter_namespace:
+            raise NotImplementedError
+
+        return scope.macro_parameter_namespace[name].evaluate_static_value(scope)
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-import builtins
-import types
 import typing
 
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
+
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
 
 
-class ModuleAccessExpression(AbstractAccessExpression):
-    IS_STATIC = True
-    PREFIX = "~"
-    _CACHE = builtins.__dict__.copy()
+class TopOfStackAccessExpression(AbstractAccessExpression):
+    PREFIX = "%"
+
+    def __init__(self, token=None, offset=0):
+        self.token = token
+        self.offset = offset
+
+    def __eq__(self, other):
+        return type(self) == type(other)
 
-    @classmethod
-    def _cached_lookup(cls, module_name: str) -> types.ModuleType:
-        if module_name not in cls._CACHE:
-            module = cls._CACHE[module_name] = __import__(module_name)
-            return module
+    def __repr__(self):
+        return f"%"
 
-        return cls._CACHE[module_name]
+    def copy(self) -> "AbstractAccessExpression":
+        return type(self)(self.token)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self._cached_lookup(self.get_name(scope))
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, Opcodes.LOAD_CONST, value
-            )
-        ]
+        if self.offset != 0:
+            return [
+                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset)
+                for _ in range(self.offset - 1)
+            ] + [
+                Instruction(function, -1, Opcodes.DUP_TOP),
+                Instruction(function, -1, Opcodes.ROT_TWO),
+                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset),
+            ]
+
+        return []
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise RuntimeError
+        if self.offset != 0:
+            raise NotImplementedError("%<n> as store target")
+
+        return []
 
-    def get_static_value(self, scope: ParsingScope) -> typing.Any:
-        return self._cached_lookup(self.get_name(scope))
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
+from bytecodemanipulation.assembler.AbstractBase import (
+    IIdentifierAccessor,
+    StaticIdentifier,
+)
 
 
 class StaticAttributeAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
 
     def __init__(
-        self, root: AbstractAccessExpression, name: typing.Union["IIdentifierAccessor", str],
+        self,
+        root: AbstractAccessExpression,
+        name: typing.Union["IIdentifierAccessor", str],
     ):
         self.root = root
-        self.name = (
-            name
-            if not isinstance(name, str)
-            else StaticIdentifier(name)
-        )
+        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.root == other.root
             and self.name == other.name
         )
@@ -61,7 +63,18 @@
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
             self, (self.root.visit_parts(visitor, parents + [self]),), parents
         )
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        base = self.root.evaluate_static_value(scope)
+
+        if not hasattr(base, self.name(scope)):
+            raise NotImplementedError
+
+        return getattr(base, self.name(scope))
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return list(self.root.get_tokens()) + [self.token]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class SubscriptionAccessExpression(AbstractAccessExpression):
     def __init__(
         self,
         base_expr: "AbstractAccessExpression",
         index_expr: AbstractAccessExpression | IntegerToken,
@@ -71,24 +72,44 @@
                         "LOAD_CONST",
                         int(self.index_expr.text),
                     )
                 ]
             )
             + [
                 Instruction.create_with_token(
-                    self.name_token, function, -1, Opcodes.STORE_SUBSCR
+                    self.name(scope), function, -1, Opcodes.STORE_SUBSCR
                 )
             ]
         )
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
             self,
-            (self.base_expr.visit_parts(visitor), self.index_expr.visit_parts(visitor)),
+            (
+                self.base_expr.visit_parts(visitor, parents + [self]),
+                self.index_expr.visit_parts(visitor, parents + [self]),
+            ),
+            parents,
+        )
+
+    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
+        base = self.base_expr.evaluate_static_value(scope)
+        index = self.index_expr.evaluate_static_value(scope)
+
+        try:
+            return base[index]
+        except (IndexError, KeyError):
+            raise NotImplementedError from None
+
+    def get_tokens(self) -> typing.Iterable[AbstractToken]:
+        return (
+            list(self.base_expr.get_tokens())
+            + list(self.index_expr.get_tokens())
+            + [self.token]
         )
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 import typing
 
-from bytecodemanipulation.Opcodes import Opcodes
-
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.data.shared.instructions.YieldAssembly import (
+    AbstractYieldAssembly,
+)
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class TopOfStackAccessExpression(AbstractAccessExpression):
-    PREFIX = "%"
-
-    def __init__(self, token=None, offset=0):
-        self.token = token
-        self.offset = offset
-
-    def __eq__(self, other):
-        return type(self) == type(other)
-
-    def __repr__(self):
-        return f"%"
-
-    def copy(self) -> "AbstractAccessExpression":
-        return type(self)(self.token)
-
+@Parser.register
+class YieldAssembly(AbstractYieldAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        if self.offset != 0:
-            return [
-                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset)
-                for _ in range(self.offset - 1)
-            ] + [
-                Instruction(function, -1, Opcodes.DUP_TOP),
-                Instruction(function, -1, Opcodes.ROT_TWO),
-                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset),
+        bytecode = []
+
+        if self.expr:
+            bytecode += self.expr.emit_bytecodes(function, scope)
+
+        if self.is_star:
+            bytecode += [
+                Instruction(function, -1, Opcodes.GET_YIELD_FROM_ITER),
+                Instruction(function, -1, Opcodes.LOAD_CONST, None),
+                Instruction(function, -1, Opcodes.YIELD_FROM),
             ]
 
-        return []
+        else:
+            bytecode += [
+                Instruction(function, -1, Opcodes.YIELD_VALUE),
+            ]
 
-    def emit_store_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        if self.offset != 0:
-            raise NotImplementedError("%<n> as store target")
+        if self.target:
+            bytecode += self.target.emit_store_bytecodes(function, scope)
+
+        else:
+            bytecode += [Instruction(function, -1, Opcodes.POP_TOP)]
+
+        # print(bytecode)
 
-        return []
+        return bytecode
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 from abc import ABC
 
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/CallAssembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 
 
 class AbstractForEachAssembly(AbstractAssemblyInstruction, abc.ABC):
     # FOREACH <variable> {',' <variable>} IN <iterable> {(',' | '*') <iterable>} '{' <block> '}'
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/IfAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LabelAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LabelAssembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class LabelAssembly(AbstractAssemblyInstruction):
     # LABEL <name>
     NAME = "LABEL"
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadAssembly(AbstractAssemblyInstruction):
     # LOAD <access> [-> <target>]
     NAME = "LOAD"
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 )
 from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
     GlobalAccessExpression,
 )
 from bytecodemanipulation.data.shared.expressions.LocalAccessExpression import (
     LocalAccessExpression,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
 
 
 LOCAL_TO_DEREF_OPCODES = {
@@ -594,14 +594,17 @@
             self.function = MutableFunction(function)
             self.scoped_names = scoped_names or []
 
         def emit_bytecodes(
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             macro_exit_label = scope.scope_name_generator("macro_exit")
+
+            builder = self.function.create_filled_builder()
+
             return [
                 (
                     instr.copy(owner=function)
                     if instr.opcode != Opcodes.RETURN_VALUE
                     else instr.copy(owner=function)
                     .change_opcode(Opcodes.POP_TOP)
                     .insert_after(
@@ -613,9 +616,9 @@
                         )
                     )
                 )
                 if not instr.has_local() or instr.arg_value not in self.scoped_names
                 else instr.copy(owner=function).change_opcode(
                     LOCAL_TO_DEREF_OPCODES[instr.opcode]
                 )
-                for instr in self.function.instructions
+                for instr in builder.temporary_instructions
             ] + [Instruction(function, -1, Opcodes.BYTECODE_LABEL, macro_exit_label)]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class MacroImportAssembly(AbstractAssemblyInstruction):
     # MACRO_IMPORT <module name with '.'> ['->' ['.'] <namespace with '.'>]
     NAME = "MACRO_IMPORT"
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class MacroPasteAssembly(AbstractAssemblyInstruction):
     # MACRO_PASTE <macro param name> ['->' <target>]
     NAME = "MACRO_PASTE"
 
     @classmethod
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class MacroReturnAssembly(AbstractAssemblyInstruction):
     NAME = "MACRO_RETURN"
 
     @classmethod
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/OpAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import PythonCodeToken
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class PythonCodeAssembly(AbstractAssemblyInstruction):
     # PYTHON '{' <code> '}'
     NAME = "PYTHON"
@@ -34,20 +34,12 @@
         inner_code = "\n    ".join(self.code.text.split("\n"))
         code = f"def target():\n    {inner_code}"
 
         ctx = {}
         exec(code, ctx)
 
         mutable = MutableFunction(ctx["target"])
-
-        instructions = []
-
-        for instr in mutable.instructions:
-            instr.update_owner(
-                function, offset=-1, update_following=False, force_change_arg_index=True
-            )
-            instructions.append(instr)
-
-        return instructions
+        builder = mutable.create_filled_builder()
+        return builder.temporary_instructions
 
     def copy(self) -> "PythonCodeAssembly":
         return type(self)(self.code)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/RawAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RawAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken, IntegerToken
-from bytecodemanipulation.MutableFunction import MutableFunction, Instruction
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 
 
 @Parser.register
 class RawAssembly(AbstractAssemblyInstruction):
     # RAW <opcode_or_name> [<arg>]
     NAME = "RAW"
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class StoreAssembly(AbstractAssemblyInstruction):
     # STORE <access> [(expression)]
     NAME = "STORE"
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/WhileAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/shared/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/YieldAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/assembly_instructions.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/assembly_instructions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     NamespaceAssembly,
     MacroImportAssembly,
     LoadAssembly,
     StoreAssembly,
     MacroReturnAssembly,
     RawAssembly,
 )
-from bytecodemanipulation.data.v3_10.instructions import (
+from bytecodemanipulation.data.v3_11.instructions import (
     CallAssembly,
     ClassDefinitionAssembly,
     ForEachAssembly,
     FunctionDefinitionAssembly,
     IfAssembly,
     JumpAssembly,
     LoadConstAssembly,
@@ -22,15 +22,14 @@
     PopElementAssembly,
     RaiseAssembly,
     ReturnAssembly,
     StoreFastAssembly,
     StoreGlobalAssembly,
     WhileAssembly,
     YieldAssembly,
-    AssertAssembly,
 )
 
 
 MacroAssembly.MacroAssembly.register()
 MacroPasteAssembly.MacroPasteAssembly.register()
 NamespaceAssembly.NamespaceAssembly.register()
 MacroImportAssembly.MacroImportAssembly.register()
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.AssertAssembly import (
     AbstractAssertAssembly,
 )
 
 
 @Parser.register
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class CallAssembly(AbstractCallAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ClassDefinitionAssembly import (
     AbstractClassDefinitionAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ForEachAssembly import (
     AbstractForEachAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class ForEachAssembly(AbstractForEachAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing
 
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
 )
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.util import LambdaInstructionWalker
 
 
 @Parser.register
 class FunctionDefinitionAssembly(AbstractFunctionDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
@@ -42,15 +42,15 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                # print(name, name(scope), is_static)
+                print(name, name(scope), is_static)
                 inner_bytecode += [
                     Instruction(target, -1, Opcodes.LOAD_DEREF, name(scope) + "%inner"),
                     Instruction(target, -1, Opcodes.STORE_DEREF, name(scope)),
                 ]
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
         inner_bytecode[-1].next_instruction = target.instructions[0]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class IFAssembly(AbstractIFAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
 
         if self.label_name is None:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.JumpAssembly import (
     AbstractJumpAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class JumpAssembly(AbstractJumpAssembly):
     # JUMP <label name> [(IF <condition access>) | ('(' <expression> | <op expression> ')')]
 
     def emit_bytecodes(
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import typing
 
-from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
-    ConstantAccessExpression,
-)
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.LoadConstAssembly import (
-    AbstractLoadConstAssembly,
+from bytecodemanipulation.data.shared.instructions.LoadFastAssembly import (
+    AbstractLoadFastAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class LoadConstAssembly(AbstractLoadConstAssembly):
+class LoadFastAssembly(AbstractLoadFastAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return [
-            Instruction(
-                function,
-                -1,
-                "LOAD_CONST",
-                self.value.value
-                if isinstance(self.value, ConstantAccessExpression)
-                else function.target.__globals__.get(self.value.name_token.text),
-            )
-        ] + (self.target.emit_bytecodes(function, scope) if self.target else [])
+        value = self.name_token.text
+
+        if value.isdigit():
+            value = int(value)
+
+        return [Instruction(function, -1, "LOAD_FAST", value)] + (
+            self.target.emit_bytecodes(function, scope) if self.target else []
+        )
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.LoadFastAssembly import (
     AbstractLoadFastAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadFastAssembly(AbstractLoadFastAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.LoadGlobalAssembly import (
-    AbstractLoadGlobalAssembly,
+from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
+    AbstractStoreGlobalAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class LoadGlobalAssembly(AbstractLoadGlobalAssembly):
+class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return [Instruction(function, -1, "LOAD_GLOBAL", value)] + (
-            self.target.emit_bytecodes(function, scope) if self.target else []
-        )
+        return (
+            [] if self.source is None else self.source.emit_bytecodes(function, scope)
+        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.OpAssembly import (
     AbstractOpAssembly,
     AbstractOperator,
 )
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class NandOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
@@ -89,14 +89,39 @@
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         return super().emit_bytecodes(function, scope, lhs, rhs) + [
             Instruction(function, -1, Opcodes.UNARY_NOT, bool)
         ]
 
 
+class OrEvalOperator(AbstractOperator):
+    def emit_bytecodes(
+        self,
+        function: MutableFunction,
+        scope: ParsingScope,
+        lhs: AbstractSourceExpression,
+        rhs: AbstractSourceExpression,
+    ) -> typing.List[Instruction]:
+        label_name = scope.scope_name_generator("or_skip_second")
+
+        bytecode = lhs.emit_bytecodes(function, scope)
+        bytecode += [
+            Instruction(function, -1, Opcodes.DUP_TOP),
+            Instruction(
+                function, -1, Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(label_name)
+            ),
+            Instruction(function, -1, Opcodes.POP_TOP),
+        ]
+        bytecode += rhs.emit_bytecodes(function, scope)
+        bytecode += [
+            Instruction(function, -1, Opcodes.BYTECODE_LABEL, label_name),
+        ]
+        return bytecode
+
+
 class XOROperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
@@ -344,14 +369,15 @@
         "issubclass": SubclassOfChecker(),
         "subclassof": SubclassOfChecker(),
         "hasattr": HasattrChecker(),
         "and": AndOperator(),
         "!and": NandOperator(),
         "nand": NandOperator(),
         "or": OrOperator(),
+        "oreval": OrEvalOperator(),
         "!or": NorOperator(),
         "nor": NorOperator(),
     }
 
     SINGLE_OPS = {
         "-": OpcodeBaseOperator(Opcodes.UNARY_NEGATIVE),
         "+": OpcodeBaseOperator(Opcodes.UNARY_POSITIVE),
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.PopElementAssembly import (
     AbstractPopElementAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class PopElementAssembly(AbstractPopElementAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.RaiseAssembly import (
     AbstractRaiseAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class RaiseAssembly(AbstractRaiseAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ReturnAssembly import (
     AbstractReturnAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class ReturnAssembly(AbstractReturnAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.StoreFastAssembly import (
-    AbstractStoreFastAssembly,
+from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
+    AbstractStoreGlobalAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class StoreFastAssembly(AbstractStoreFastAssembly):
+class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_FAST", value)]
+        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
-    AbstractStoreGlobalAssembly,
+from bytecodemanipulation.data.shared.instructions.StoreFastAssembly import (
+    AbstractStoreFastAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
+class StoreFastAssembly(AbstractStoreFastAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
+        ) + [Instruction(function, -1, "STORE_FAST", value)]
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
     AbstractWhileAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class WHILEAssembly(AbstractWhileAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
         if self.label_name is None:
             end = Instruction(function, -1, "NOP")
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/assembly_instructions.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/assembly_instructions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from bytecodemanipulation.data.shared.instructions import (
     MacroAssembly,
     MacroPasteAssembly,
     NamespaceAssembly,
     MacroImportAssembly,
+    AssertStaticInstruction,
     LoadAssembly,
     StoreAssembly,
     MacroReturnAssembly,
     RawAssembly,
 )
-from bytecodemanipulation.data.v3_11.instructions import (
+from bytecodemanipulation.data.v3_10.instructions import (
     CallAssembly,
     ClassDefinitionAssembly,
     ForEachAssembly,
     FunctionDefinitionAssembly,
     IfAssembly,
     JumpAssembly,
     LoadConstAssembly,
@@ -22,14 +23,16 @@
     PopElementAssembly,
     RaiseAssembly,
     ReturnAssembly,
     StoreFastAssembly,
     StoreGlobalAssembly,
     WhileAssembly,
     YieldAssembly,
+    AssertAssembly,
 )
 
 
 MacroAssembly.MacroAssembly.register()
 MacroPasteAssembly.MacroPasteAssembly.register()
 NamespaceAssembly.NamespaceAssembly.register()
 MacroImportAssembly.MacroImportAssembly.register()
+AssertStaticInstruction.AssertStaticInstruction.register()
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class CallAssembly(AbstractCallAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ClassDefinitionAssembly import (
     AbstractClassDefinitionAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
@@ -35,20 +35,20 @@
                 instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
             elif instr.opcode == Opcodes.DELETE_FAST:
                 instr.change_opcode(Opcodes.DELETE_NAME, arg_value=instr.arg_value)
 
         inner_bytecode += raw_inner_code
 
         if inner_bytecode:
-            inner_bytecode[-1].next_instruction = target.instructions[0]
+            inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
-        target.assemble_instructions_from_tree(inner_bytecode[0])
+        target.instruction_entry_point = inner_bytecode[0]
         target.reassign_to_function()
 
         code_obj = target.target.__code__
 
         bytecode = [
             Instruction(function, -1, Opcodes.LOAD_BUILD_CLASS),
             Instruction(function, -1, Opcodes.LOAD_CONST, code_obj),
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ForEachAssembly import (
     AbstractForEachAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class ForEachAssembly(AbstractForEachAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing
 
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
 )
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.util import LambdaInstructionWalker
 
 
 @Parser.register
 class FunctionDefinitionAssembly(AbstractFunctionDefinitionAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
@@ -42,22 +42,22 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                print(name, name(scope), is_static)
+                # print(name, name(scope), is_static)
                 inner_bytecode += [
                     Instruction(target, -1, Opcodes.LOAD_DEREF, name(scope) + "%inner"),
                     Instruction(target, -1, Opcodes.STORE_DEREF, name(scope)),
                 ]
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
-        inner_bytecode[-1].next_instruction = target.instructions[0]
+        inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
         def walk_label(instruction: Instruction):
             if instruction.opcode == Opcodes.BYTECODE_LABEL:
                 # print(instruction, instruction.next_instruction)
@@ -72,15 +72,15 @@
 
         def resolve_jump_to_label(ins: Instruction):
             if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
                 ins.change_arg_value(label_targets[ins.arg_value.name])
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
 
-        target.assemble_instructions_from_tree(inner_bytecode[0])
+        target.instruction_entry_point = inner_bytecode[0]
         del inner_bytecode
 
         has_kwarg = False
         for arg in self.args:
             if isinstance(arg, AbstractCallAssembly.IMPLEMENTATION.KwArg):
                 has_kwarg = True
                 break
@@ -110,14 +110,15 @@
             bytecode.append(
                 Instruction(
                     function, -1, Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
                 )
             )
 
         target.argument_count = len(self.args)
+        target.prepare_previous_instructions()
         code_object = target.create_code_obj()
 
         bytecode += [
             Instruction(function, -1, "LOAD_CONST", code_object),
             Instruction(
                 function,
                 -1,
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class IFAssembly(AbstractIFAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
 
         if self.label_name is None:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.JumpAssembly import (
     AbstractJumpAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class JumpAssembly(AbstractJumpAssembly):
     # JUMP <label name> [(IF <condition access>) | ('(' <expression> | <op expression> ')')]
 
     def emit_bytecodes(
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ConstantAccessExpression,
 )
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.LoadConstAssembly import (
     AbstractLoadConstAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadConstAssembly(AbstractLoadConstAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.LoadGlobalAssembly import (
     AbstractLoadGlobalAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadGlobalAssembly(AbstractLoadGlobalAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.data.shared.instructions.OpAssembly import AbstractOpAssembly
-from bytecodemanipulation.MutableFunction import Instruction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class OpAssembly(AbstractOpAssembly):
     BINARY_OPS = {
         "+": Opcodes.BINARY_ADD,
         "-": Opcodes.BINARY_SUBTRACT,
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.PopElementAssembly import (
     AbstractPopElementAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class PopElementAssembly(AbstractPopElementAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.RaiseAssembly import (
     AbstractRaiseAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class RaiseAssembly(AbstractRaiseAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ReturnAssembly import (
     AbstractReturnAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class ReturnAssembly(AbstractReturnAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.StoreFastAssembly import (
     AbstractStoreFastAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class StoreFastAssembly(AbstractStoreFastAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import typing
 
+from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
+    ConstantAccessExpression,
+)
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
-    AbstractStoreGlobalAssembly,
+from bytecodemanipulation.data.shared.instructions.LoadConstAssembly import (
+    AbstractLoadConstAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
+class LoadConstAssembly(AbstractLoadConstAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.name_token.text
-
-        if value.isdigit():
-            value = int(value)
-
-        return (
-            [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
+        return [
+            Instruction(
+                function,
+                -1,
+                "LOAD_CONST",
+                self.value.value
+                if isinstance(self.value, ConstantAccessExpression)
+                else function.target.__globals__.get(self.value.name_token.text),
+            )
+        ] + (self.target.emit_bytecodes(function, scope) if self.target else [])
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
     AbstractWhileAssembly,
 )
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class WHILEAssembly(AbstractWhileAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
         if self.label_name is None:
             end = Instruction(function, -1, "NOP")
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/data_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import json
 import logging
 import os
 import sys
-from bytecodemanipulation.Opcodes import Opcodes, init_maps, OPNAME2CODE
-from bytecodemanipulation import Opcodes as OpcodesM
+from bytecodemanipulation.opcodes.Opcodes import Opcodes, init_maps, OPNAME2CODE
+from bytecodemanipulation.opcodes import Opcodes as OpcodesM
 from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
 
 
 local = os.path.dirname(__file__)
 
 version = f"{sys.version_info.major}_{sys.version_info.minor}"
 folder = local + "/data/v" + version
@@ -20,27 +20,33 @@
 
 def load_opcode_data():
     opcode_data: dict = json.load(open(folder + "/opcodes.json"))
 
     valid_opcode_names = [
         key
         for key, value in Opcodes.__dict__.items()
-        if isinstance(value, int) and not key.startswith("__") and value < 256
+        if isinstance(value, int) and not key.startswith("__") and value != -1
     ]
 
     for key, opcode in opcode_data.items():
         if key not in valid_opcode_names:
             logging.warning(f"unknown opcode name encountered: {key} - Adding manually")
 
         setattr(Opcodes, key, opcode)
 
     for key in valid_opcode_names:
         if key not in opcode_data:
             setattr(Opcodes, key, -1)
 
+    virtual_opcode = 256
+    for key, value in Opcodes.__dict__.items():
+        if not key.startswith("__") and value == -1:
+            setattr(Opcodes, key, virtual_opcode)
+            virtual_opcode += 1
+
 
 def load_instruction_spec():
     spec_data = json.load(open(folder + "/instruction_spec.json"))
 
     for key, opcodes in spec_data.items():
         getattr(OpcodesM, key)[:] = map(OPNAME2CODE.__getitem__, opcodes)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/mixin_util.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/mixin_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import typing
 
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 def resolve_accesses(
     inject_target: MutableFunction, injected: MutableFunction
 ) -> typing.List[str]:
     BOUND_LOCALS = {}
     BOUND_CELL_VARIABLES = {}
 
-    for instruction in injected.instructions:
+    def visit(instruction):
         if instruction.has_local():
             instruction.change_arg_value(
                 injected.function_name + "::" + instruction.arg_value
             )
 
-    for instruction in injected.instructions:
+    inject_target.walk_instructions(visit)
+
+    def visit(instruction):
         if (
             instruction.opcode in (Opcodes.CALL_METHOD, Opcodes.CALL_FUNCTION)
             and instruction.arg <= 1
         ):
             source = next(instruction.trace_stack_position(instruction.arg))
 
             if source.opcode == Opcodes.LOAD_CONST:
                 target = source.arg_value
 
                 if not isinstance(target, classmethod):
-                    continue
+                    return
 
                 func_name = target.__name__
                 is_const = True
                 source_source = None
             elif source.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
                 source_source = next(source.trace_stack_position(0))
 
                 if (
                     source_source.opcode == Opcodes.LOAD_FAST
                     and source_source.arg_value in ("self", "cls")
                 ):
                     func_name = source.arg_value
                     is_const = False
                 else:
-                    continue
+                    return
             else:
-                continue
+                return
 
             if func_name == "resolve_local":
                 assert (
                     instruction.arg == 1
                 ), f"resolve_local() must be invoked with exactly one arg, got {instruction.arg}"
 
                 variable_name = next(instruction.trace_stack_position(0))
@@ -99,8 +101,10 @@
                 instruction.change_arg_value(BOUND_LOCALS[instruction.arg_value])
             elif instruction.arg_value in BOUND_CELL_VARIABLES:
                 instruction.change_opcode(instruction.opname.replace("FAST", "DEREF"))
                 instruction.change_arg_value(
                     BOUND_CELL_VARIABLES[instruction.arg_value]
                 )
 
+    injected.walk_instructions(visit)
+
     return list(BOUND_LOCALS.keys())
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/optimiser_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import traceback
 import typing
 from bytecodemanipulation.annotated_std import CONSTANT_BUILTIN_TYPES
 from bytecodemanipulation.annotated_std import CONSTANT_BUILTINS
 
-from bytecodemanipulation.MutableFunction import Instruction
+from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.Opcodes import Opcodes
-from bytecodemanipulation.Opcodes import SIDE_EFFECT_FREE_LOADS
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
+from bytecodemanipulation.opcodes.Opcodes import SIDE_EFFECT_FREE_LOADS
 from bytecodemanipulation.Specialization import ArgDescriptor
 from bytecodemanipulation.Specialization import MethodCallDescriptor
 from bytecodemanipulation.Specialization import SpecializationContainer
 
 OPCODE_TO_ATTR_SINGLE = {
     Opcodes.UNARY_POSITIVE: "__pos__",
     Opcodes.UNARY_NEGATIVE: "__neg__",
@@ -51,33 +51,25 @@
     (Opcodes.COMPARE_OP, 2): lambda a, b: a == b,
     (Opcodes.COMPARE_OP, 3): lambda a, b: a != b,
     (Opcodes.COMPARE_OP, 4): lambda a, b: a > b,
     (Opcodes.COMPARE_OP, 5): lambda a, b: a >= b,
 }
 
 
-def inline_const_value_pop_pairs(mutable: MutableFunction) -> bool:
+def inline_const_value_pop_pairs(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    for instruction in mutable.instructions:
+    def visit(instruction: Instruction):
+        nonlocal dirty
+
         if instruction.opcode == Opcodes.POP_TOP:
             try:
                 # print("search")
                 source = next(instruction.trace_stack_position(0))
             except StopIteration:
-                # source = next(instruction.trace_stack_position(0))
-
-                print("---")
-
-                for instr in mutable.instructions:
-                    print(instr)
-
-                print("---")
-                print(instruction)
-                print(instruction.get_priorities_previous())
                 raise
 
             # Inline LOAD_XX - POP pairs
             if source.opcode in SIDE_EFFECT_FREE_LOADS:
                 instruction.change_opcode(Opcodes.NOP)
                 source.change_opcode(Opcodes.NOP)
                 return True
@@ -95,31 +87,29 @@
                             function, "_OPTIMISER_CONTAINER"
                         ).is_side_effect_free_op
                     ):
                         instruction.change_opcode(Opcodes.NOP)
 
                         if func_resolve.arg == 0:
                             func_resolve.change_opcode(Opcodes.NOP)
-                            continue
+                            return
+
                         pops = func_resolve.arg
 
                         func_resolve.change_opcode(Opcodes.POP_TOP)
                         pops -= 1
 
                         if not pops:
-                            continue
+                            return
 
                         for _ in range(pops):
                             nop = Instruction.create(Opcodes.NOP)
                             nop.next_instruction = func_resolve.next_instruction
                             func_resolve.next_instruction = nop
 
-                        mutable.assemble_instructions_from_tree(
-                            mutable.instructions[0].optimise_tree()
-                        )
                         return True
 
             if source.opcode in (
                 Opcodes.BUILD_LIST,
                 Opcodes.BUILD_SET,
                 Opcodes.BUILD_MAP,
             ):
@@ -129,95 +119,102 @@
                     count *= 2
 
                 instruction.change_opcode(Opcodes.NOP)
 
                 if count == 0:
                     source.change_opcode(Opcodes.NOP)
                     dirty = True
-                    continue
+                    return
 
                 source.change_opcode(Opcodes.POP_TOP)
 
                 if count == 1:
                     dirty = True
-                    continue
+                    return
 
                 count -= 1
 
                 for _ in range(count):
                     nop = Instruction.create(Opcodes.NOP)
                     nop.next_instruction = source.next_instruction
                     source.next_instruction = nop
 
-                mutable.assemble_instructions_from_tree(
-                    mutable.instructions[0].optimise_tree()
-                )
-                return True
+    mutable.walk_instructions(visit)
 
     return dirty
 
 
-def remove_local_var_assign_without_use(mutable: MutableFunction) -> bool:
+def remove_local_var_assign_without_use(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    last_loads_of_local = [-1] * len(mutable.shared_variable_names)
+    last_loads_of_local = {}
 
-    for instruction in mutable.instructions:
+    def fill_info(instruction: Instruction):
         if instruction.opcode == Opcodes.LOAD_FAST:
-            last_loads_of_local[instruction.arg] = instruction.offset
+            last_loads_of_local[instruction.arg_value] = instruction.offset
 
-    for instruction in mutable.instructions:
+    def remove_instruction(instruction: Instruction):
         if (
             instruction.opcode in (Opcodes.STORE_FAST, Opcodes.DELETE_FAST)
-            and last_loads_of_local[instruction.arg] < instruction.offset
+            and last_loads_of_local.get(instruction.arg_value, -1) < instruction.offset
         ):
             instruction.change_opcode(Opcodes.POP_TOP)
+
+            nonlocal dirty
             dirty = True
 
+    mutable.walk_instructions(fill_info)
+    mutable.walk_instructions(remove_instruction)
+
     return dirty
 
 
-def inline_constant_method_invokes(mutable: MutableFunction) -> bool:
+def inline_constant_method_invokes(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    for instr in mutable.instructions:
-        if instr.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
-            target = next(instr.trace_stack_position(instr.arg))
+    def visit(instruction: Instruction):
+        if instruction.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
+            target = next(instruction.trace_stack_position(instruction.arg))
 
             if target.opcode == Opcodes.LOAD_CONST:
                 function: typing.Callable = target.arg_value
 
                 if function in CONSTANT_BUILTINS or (
                     hasattr(function, "_OPTIMISER_CONTAINER")
                     and getattr(function, "_OPTIMISER_CONTAINER").is_constant_op
                 ):
                     args = [
-                        next(instr.trace_stack_position(i))
-                        for i in range(instr.arg - 1, -1, -1)
+                        next(instruction.trace_stack_position(i))
+                        for i in range(instruction.arg - 1, -1, -1)
                     ]
 
                     if all(ins.opcode == Opcodes.LOAD_CONST for ins in args):
                         result = function(*(e.arg_value for e in args))
 
-                        instr.change_opcode(Opcodes.LOAD_CONST)
-                        instr.change_arg_value(result)
+                        instruction.change_opcode(Opcodes.LOAD_CONST)
+                        instruction.change_arg_value(result)
                         target.change_opcode(Opcodes.NOP)
 
                         for arg in args:
                             arg.change_opcode(Opcodes.NOP)
 
+                        nonlocal dirty
                         dirty = True
 
+    mutable.walk_instructions(visit)
+
     return dirty
 
 
-def inline_constant_binary_ops(mutable: MutableFunction) -> bool:
+def inline_constant_binary_ops(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    for instruction in mutable.instructions:
+    def visit(instruction: Instruction):
+        nonlocal dirty
+
         if (
             instruction.opcode in OPCODE_TO_ATTR_SINGLE
             or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_SINGLE
         ):
             method = OPCODE_TO_ATTR_SINGLE[
                 instruction.opcode
                 if instruction.opcode in OPCODE_TO_ATTR_SINGLE
@@ -237,20 +234,21 @@
                     if not callable(method) or not (
                         type(value) in CONSTANT_BUILTIN_TYPES
                         or (
                             hasattr(method, "_OPTIMISER_CONTAINER")
                             and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
                         )
                     ):
-                        continue
+                        return
 
                     try:
                         value = method()
                     except:
-                        continue
+                        traceback.print_exc()
+                        return
 
                     instruction.change_opcode(Opcodes.LOAD_CONST)
                     instruction.change_arg_value(value)
                     target.change_opcode(Opcodes.NOP)
                     dirty = True
 
         elif (
@@ -275,21 +273,21 @@
                     if not callable(method) or not (
                         type(value) in CONSTANT_BUILTIN_TYPES
                         or (
                             hasattr(method, "_OPTIMISER_CONTAINER")
                             and getattr(method, "_OPTIMISER_CONTAINER").is_constant_op
                         )
                     ):
-                        continue
+                        return
 
                 try:
                     value = method(arg.arg_value, target.arg_value)
                 except:
                     traceback.print_exc()
-                    continue
+                    return
 
                 instruction.change_opcode(Opcodes.LOAD_CONST)
                 instruction.change_arg_value(value)
                 target.change_opcode(Opcodes.NOP)
                 arg.change_opcode(Opcodes.NOP)
                 dirty = True
 
@@ -334,32 +332,36 @@
                 instruction.change_arg_value("".join(e.arg_value for e in args))
 
                 for arg in args:
                     arg.change_opcode(Opcodes.NOP)
 
                 dirty = True
 
+    mutable.walk_instructions(visit)
+
     return dirty
 
 
-def remove_branch_on_constant(mutable: MutableFunction) -> bool:
+def remove_branch_on_constant(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    for instruction in mutable.instructions:
+    def visit(instruction):
+        nonlocal dirty
+
         if (
             instruction.has_jump()
             and not instruction.has_unconditional_jump()
             and instruction.opcode not in (Opcodes.SETUP_FINALLY, Opcodes.SETUP_WITH)
         ):
             if instruction.previous_instructions is None:
                 if (
                     instruction.offset == 0
                     and instruction.opcode == Opcodes.SETUP_FINALLY
                 ):
-                    continue
+                    return
 
                 raise RuntimeError
 
             source = next(instruction.trace_stack_position(0))
 
             if source.opcode == Opcodes.LOAD_CONST:
                 flag = bool(source.arg_value)
@@ -375,15 +377,15 @@
                         instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
                     else:
                         source.change_opcode(Opcodes.NOP)
                         instruction.change_opcode(Opcodes.NOP)
 
                     dirty = True
 
-                    continue
+                    return
 
                 if instruction.opcode in (
                     Opcodes.POP_JUMP_IF_TRUE,
                     Opcodes.POP_JUMP_IF_FALSE,
                 ):
                     flag = bool(source.arg_value)
 
@@ -395,21 +397,23 @@
                     if flag:
                         instruction.change_opcode(Opcodes.JUMP_ABSOLUTE)
                     else:
                         instruction.change_opcode(Opcodes.NOP)
 
                     dirty = True
 
+    mutable.walk_instructions(visit)
+
     return dirty
 
 
-def inline_static_attribute_access(mutable: MutableFunction) -> bool:
+def inline_static_attribute_access(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
-    for instruction in mutable.instructions:
+    def visit(instruction: Instruction):
         if instruction.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
             source_instr = next(instruction.trace_stack_position(0))
 
             if source_instr.opcode == Opcodes.LOAD_CONST:
                 source: typing.Any = source_instr.arg_value
 
                 if hasattr(
@@ -425,35 +429,40 @@
                     # print(instruction)
 
                     use = next(instruction.trace_stack_position_use(0))
 
                     if use.opcode == Opcodes.CALL_METHOD:
                         use.change_opcode(Opcodes.CALL_FUNCTION)
 
+                    nonlocal dirty
                     dirty = True
 
+    mutable.walk_instructions(visit)
+
     return dirty
 
 
-def apply_specializations(mutable: MutableFunction) -> bool:
+def apply_specializations(mutable: MutableFunction, builder) -> bool:
     from bytecodemanipulation.Optimiser import _OptimisationContainer
 
     dirty = False
 
-    for instruction in mutable.instructions:
+    def visit(instruction: Instruction):
+        nonlocal dirty
+
         if instruction.opcode in (Opcodes.CALL_FUNCTION, Opcodes.CALL_METHOD):
             load_stack_pos = instruction.arg
             source = instruction.trace_normalized_stack_position(load_stack_pos)
             safe_source = next(instruction.trace_stack_position(load_stack_pos))
 
             if source and source.opcode == Opcodes.LOAD_CONST:
                 container = _OptimisationContainer.get_for_target(source.arg_value)
 
                 if not container.specializations:
-                    continue
+                    return
 
                 target_func = source.arg_value
 
                 spec = SpecializationContainer()
                 spec.target = mutable
                 spec.underlying_function = target_func
                 spec.method_call_descriptor = MethodCallDescriptor(
@@ -476,14 +485,16 @@
                     if spec.no_special:
                         continue
 
                     spec.apply()
                     dirty = True
                     break
 
+    mutable.walk_instructions(visit)
+
     return dirty
 
 
 def remove_nops(mutable: MutableFunction):
     root = mutable.instructions[0]
     root = root.optimise_tree()
     mutable.assemble_instructions_from_tree(root)
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation/util.py` & `bytecodemanipulation-0.3.1/bytecodemanipulation/util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.2.9
+Version: 0.3.1
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `bytecodemanipulation-0.2.9/bytecodemanipulation.egg-info/SOURCES.txt` & `bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 README.md
 pyproject.toml
 setup.py
 bytecodemanipulation/Emulator.py
 bytecodemanipulation/Mixin.py
 bytecodemanipulation/MutableFunction.py
 bytecodemanipulation/MutableFunctionHelpers.py
-bytecodemanipulation/Opcodes.py
 bytecodemanipulation/Optimiser.py
 bytecodemanipulation/Specialization.py
 bytecodemanipulation/TypeEnforcer.py
 bytecodemanipulation/__init__.py
 bytecodemanipulation/annotated_std.py
-bytecodemanipulation/compiler.py
 bytecodemanipulation/data_loader.py
 bytecodemanipulation/mixin_util.py
 bytecodemanipulation/optimise_self.py
 bytecodemanipulation/optimiser_util.py
 bytecodemanipulation/util.py
 bytecodemanipulation.egg-info/PKG-INFO
 bytecodemanipulation.egg-info/SOURCES.txt
@@ -51,14 +49,15 @@
 bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
 bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
 bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
 bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
 bytecodemanipulation/data/shared/expressions/__init__.py
 bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
 bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
 bytecodemanipulation/data/shared/instructions/CallAssembly.py
 bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
 bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
 bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
 bytecodemanipulation/data/shared/instructions/IfAssembly.py
 bytecodemanipulation/data/shared/instructions/JumpAssembly.py
 bytecodemanipulation/data/shared/instructions/LabelAssembly.py
@@ -122,14 +121,20 @@
 bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
 bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
 bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
 bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
 bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
 bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
 bytecodemanipulation/data/v3_11/instructions/__init__.py
+bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+bytecodemanipulation/opcodes/CodeObjectBuilder.py
+bytecodemanipulation/opcodes/ExceptionTable.py
+bytecodemanipulation/opcodes/Instruction.py
+bytecodemanipulation/opcodes/Opcodes.py
+bytecodemanipulation/opcodes/__init__.py
 tests/test_Assembly.py
 tests/test_InlineSystem.py
 tests/test_Mixin.py
 tests/test_MutableFunction.py
 tests/test_Operators.py
 tests/test_Optimiser.py
 tests/test_Specializations.py
```

### Comparing `bytecodemanipulation-0.2.9/setup.py` & `bytecodemanipulation-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.2.9",
+    version="0.3.1",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

### Comparing `bytecodemanipulation-0.2.9/tests/test_Assembly.py` & `bytecodemanipulation-0.3.1/tests/test_Assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -935,14 +935,16 @@
 """
             )
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
+        dis.dis(target)
+
         target(self)
 
         def compare():
             x = print("Hello World!")
 
         compare_optimized_results(self, target, compare, opt_ideal=2)
 
@@ -1593,15 +1595,15 @@
             )
             return result
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
-        # dis.dis(target)
+        dis.dis(target)
 
         self.assertEqual(target(), [1, 2, 3, 4])
 
     def test_for_loop_double(self):
         def target():
             iterable = [0, 1, 2, 3]
             iterable_2 = [1, 2, 3, 4]
@@ -1682,14 +1684,16 @@
         def target(x):
             assembly(
                 """
 ASSERT $x
 """
             )
 
+        dis.dis(target)
+
         target(1)
         self.assertRaises(AssertionError, lambda: target(0))
 
     def test_assert_with_message(self):
         @apply_operations
         def target(x):
             assembly(
@@ -1703,7 +1707,87 @@
 
         try:
             target(0)
         except AssertionError as e:
             self.assertEqual(e.args, ("Test Message",))
         else:
             self.assertTrue(False)
+
+    def test_assert_static(self):
+        @apply_operations
+        def target():
+            assembly("ASSERT_STATIC 1")
+
+        target()
+
+    def test_assert_static_fail(self):
+        def target():
+            assembly("ASSERT_STATIC 0")
+
+        try:
+            apply_operations(target)
+        except AssertionError as e:
+            self.assertEqual(e.args, ("assertion failed: expected <true-ish value>",))
+
+    def test_assert_static_fail_message(self):
+        def target():
+            assembly('ASSERT_STATIC 0 "hello world"')
+
+        try:
+            apply_operations(target)
+        except AssertionError as e:
+            self.assertEqual(e.args, ("assertion failed: hello world",))
+
+    def test_assert_static_fail_message_invalid(self):
+        def target():
+            assembly("ASSERT_STATIC 0 $x")
+
+        try:
+            apply_operations(target)
+        except AssertionError as e:
+            self.assertEqual(
+                e.args,
+                ("assertion failed: expected <true-ish value> (message not arrival)",),
+            )
+
+    def test_assert_static_dynamic_expression(self):
+        def target():
+            assembly("ASSERT_STATIC $a")
+
+        try:
+            apply_operations(target)
+        except SyntaxError as e:
+            self.assertEqual(e.args, ("Expected <static evaluate-able>",))
+
+    def test_assert_static_macro_static_parameter(self):
+        @apply_operations
+        def target():
+            assembly(
+                """
+MACRO test_assert_static_macro_static_parameter(a)
+{
+    ASSERT_STATIC &a
+}
+
+CALL MACRO test_assert_static_macro_static_parameter(1)
+"""
+            )
+
+        target()
+
+    def test_assert_static_macro_static_parameter_fail(self):
+        def target():
+            assembly(
+                """
+MACRO test_assert_static_macro_static_parameter_fail(a)
+{
+    ASSERT_STATIC &a
+}
+
+CALL MACRO test_assert_static_macro_static_parameter_fail(0)
+"""
+            )
+
+        try:
+            apply_operations(target)
+        except AssertionError as e:
+            self.assertEqual(e.args, ("assertion failed: expected <true-ish value>",))
```

### Comparing `bytecodemanipulation-0.2.9/tests/test_InlineSystem.py` & `bytecodemanipulation-0.3.1/tests/test_InlineSystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         insert()
         self.assertTrue(INVOKED)
         INVOKED = False
 
         main_mut = MutableFunction(main)
         insert_mut = MutableFunction(insert)
 
-        insert_method_into(main_mut, main_mut.instructions[0], insert_mut)
+        insert_method_into(main_mut, main_mut.instruction_entry_point, insert_mut)
         main_mut.reassign_to_function()
 
         main()
         self.assertTrue(INVOKED)
 
     def test_inline_call_simple(self):
         global call
```

### Comparing `bytecodemanipulation-0.2.9/tests/test_Mixin.py` & `bytecodemanipulation-0.3.1/tests/test_Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/tests/test_Operators.py` & `bytecodemanipulation-0.3.1/tests/test_Operators.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/tests/test_Optimiser.py` & `bytecodemanipulation-0.3.1/tests/test_Optimiser.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         container = _OptimisationContainer.get_for_target(
             Outer_test_inline_const_function_on_parent
         )
         container.run_optimisers()
 
         mutable = MutableFunction(Outer_test_inline_const_function_on_parent.target)
 
-        self.assertEqual(2, mutable.instructions[0].arg_value)
+        self.assertEqual(2, mutable.instruction_entry_point.arg_value)
 
     def test_branch_remover(self):
         def target():
             if False:
                 return 0
             return 1
 
@@ -158,21 +158,21 @@
 
     def test_remove_list_build(self):
         def target():
             [200, 400, 200]
             a = [10]
 
         mutable = MutableFunction(target)
-        remove_local_var_assign_without_use(mutable)
-        inline_const_value_pop_pairs(mutable)
-        inline_const_value_pop_pairs(mutable)
-        mutable.assemble_instructions_from_tree(mutable.instructions[0].optimise_tree())
+        builder = mutable.create_filled_builder()
+        remove_local_var_assign_without_use(mutable, builder)
+        inline_const_value_pop_pairs(mutable, builder)
+        inline_const_value_pop_pairs(mutable, builder)
         mutable.reassign_to_function()
 
-        self.assertEqual(mutable.instructions[0].arg_value, None)
+        self.assertEqual(mutable.instruction_entry_point.arg_value, None)
 
     # TODO: is there a way to make this work?
     # def test_remove_list_build_stacked(self):
     #     def target():
     #         [200, 400, 200, [342, 234]]
     #
     #     dis.dis(target)
@@ -189,23 +189,23 @@
     #     self.assertEqual(mutable.instructions[0].arg_value, None)
 
     def test_remove_list_build_stacked_2(self):
         def target():
             [200, 400, 200, (342, 234)]
 
         mutable = MutableFunction(target)
-        remove_local_var_assign_without_use(mutable)
-        inline_const_value_pop_pairs(mutable)
-        inline_const_value_pop_pairs(mutable)
-        mutable.assemble_instructions_from_tree(mutable.instructions[0].optimise_tree())
+        builder = mutable.create_filled_builder()
+        remove_local_var_assign_without_use(mutable, builder)
+        inline_const_value_pop_pairs(mutable, builder)
+        inline_const_value_pop_pairs(mutable, builder)
         mutable.reassign_to_function()
 
         # dis.dis(target)
 
-        self.assertEqual(mutable.instructions[0].arg_value, None)
+        self.assertEqual(mutable.instruction_entry_point.arg_value, None)
 
     def test_empty_range_from_invalid_range(self):
         @cache_global_name("range", lambda: range)
         def target():
             return range(2, 0)
 
         compare_optimized_results(self, target, lambda: tuple(), opt_ideal=2)
```

### Comparing `bytecodemanipulation-0.2.9/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.3.1/tests/test_StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.2.9/tests/test_issues.py` & `bytecodemanipulation-0.3.1/tests/test_issues.py`

 * *Files identical despite different names*

