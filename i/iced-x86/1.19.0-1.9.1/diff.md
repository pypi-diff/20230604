# Comparing `tmp/iced-x86-1.19.0.tar.gz` & `tmp/iced-x86-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iced-x86-1.19.0.tar", last modified: Sun Jun  4 15:32:29 2023, max compression
+gzip compressed data, was "dist/iced-x86-1.9.1.tar", last modified: Sun Dec  6 22:35:42 2020, max compression
```

## Comparing `iced-x86-1.19.0.tar` & `iced-x86-1.9.1.tar`

### file list

```diff
@@ -1,157 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-04 15:32:28.000000 iced-x86-1.19.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-04 15:32:28.000000 iced-x86-1.19.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-04 15:27:13.000000 iced-x86-1.19.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-06-04 15:32:29.000000 iced-x86-1.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34897 2023-06-04 15:27:13.000000 iced-x86-1.19.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/BlockEncoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_a.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_ae.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_b.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_be.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_e.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_g.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_ge.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_l.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_le.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_ne.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_np.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CC_p.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Code.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CodeSize.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/ConditionCode.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/ConstantOffsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/CpuidFeature.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Decoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/DecoderError.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/DecoderOptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Encoder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/EncodingKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/FastFormatter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/FlowControl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/FormatMnemonicOptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Formatter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/FormatterSyntax.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/FpuStackIncrementInfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Instruction.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/InstructionInfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/InstructionInfoFactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MandatoryPrefix.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MemoryOperand.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MemorySize.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MemorySizeExt.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MemorySizeInfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MemorySizeOptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Mnemonic.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MvexConvFn.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MvexEHBit.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MvexRegMemConv.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/MvexTupleTypeLutKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/OpAccess.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/OpCodeInfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/OpCodeOperandKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/OpCodeTableKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/OpKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/Register.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/RegisterExt.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/RegisterInfo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/RepPrefixKind.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/RflagsBits.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/RoundingControl.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/TupleType.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/UsedMemory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 15:27:13.000000 iced-x86-1.19.0/docs/src/UsedRegister.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-04 15:27:13.000000 iced-x86-1.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 15:27:13.000000 iced-x86-1.19.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 15:27:13.000000 iced-x86-1.19.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-04 15:32:29.000000 iced-x86-1.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-04 15:27:13.000000 iced-x86-1.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/block_encoder.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/constant_offsets.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/decoder.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/encoder.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/enum_utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/fast_formatter.rs
--rw-r--r--   0 runner    (1001) docker     (123)    47972 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/formatter.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_ae.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_be.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_e.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_g.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_ge.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_le.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_ne.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_np.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CC_p.py
--rw-r--r--   0 runner    (1001) docker     (123)   734962 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/Code.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CodeSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/ConditionCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/CpuidFeature.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/DecoderError.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/DecoderOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/EncodingKind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/FlowControl.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/FormatMnemonicOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/FormatterSyntax.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MandatoryPrefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    15627 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MemorySize.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MemorySizeOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   109217 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/Mnemonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MvexConvFn.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MvexEHBit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MvexRegMemConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/MvexTupleTypeLutKind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/OpAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/OpCodeOperandKind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/OpCodeTableKind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/OpKind.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/Register.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/RepPrefixKind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/RflagsBits.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/RoundingControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/TupleType.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   225538 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/_iced_x86_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/iced_x86/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 15:32:29.000000 iced-x86-1.19.0/src/iced_x86.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)   176639 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/instruction.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/memory_operand.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/memory_size_ext.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/memory_size_info.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/op_code_info.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20699 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/register_ext.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/register_info.rs
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-04 15:27:13.000000 iced-x86-1.19.0/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:32:29.000000 iced-x86-1.19.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/block_encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/fast_formatter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/formatter_gas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/formatter_intel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/formatter_masm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/formatter_nasm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/formatter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    91088 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/instr_create_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/instruction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/memory_operand_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/memory_size_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/op_code_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-04 15:27:13.000000 iced-x86-1.19.0/tests/register_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 22:35:42.000000 iced-x86-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)       46 2020-12-06 22:30:55.000000 iced-x86-1.9.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 22:35:42.000000 iced-x86-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     4630 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6296 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/formatter_nasm_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6308 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/formatter_masm_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6314 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/formatter_gas_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3468 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/info_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7277 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10273 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/formatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2940 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/block_encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39290 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/instruction_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7093 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/op_code_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6297 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/formatter_intel_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3209 2020-12-06 22:30:55.000000 iced-x86-1.9.1/tests/fast_formatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      689 2020-12-06 22:30:55.000000 iced-x86-1.9.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2020-12-06 22:35:42.000000 iced-x86-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      149 2020-12-06 22:30:55.000000 iced-x86-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     6787 2020-12-06 22:30:55.000000 iced-x86-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2020-12-06 22:30:55.000000 iced-x86-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     9623 2020-12-06 22:35:42.000000 iced-x86-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2696 2020-12-06 22:30:55.000000 iced-x86-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/
+-rw-r--r--   0 runner    (1001) docker     (116)    24657 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/op_code_info.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     2947 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_constants.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    15275 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/decoder.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     7412 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/encoder.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     5573 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/enum_utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86/
+-rw-r--r--   0 runner    (1001) docker     (116)     1603 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/RoundingControl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1694 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/MemorySizeOptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9614 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/Register.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1477 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_p.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1907 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/TupleType.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2136 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/RflagsBits.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1543 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_ae.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3096 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)   566488 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/Code.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10193 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/OpCodeOperandKind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1538 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_b.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1508 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/FormatterSyntax.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_a.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_be.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2205 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/OpAccess.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1600 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/MandatoryPrefix.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_le.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1528 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_ne.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12091 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CpuidFeature.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5880 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/OpKind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_l.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2621 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/FlowControl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_ge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1527 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/EncodingKind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_g.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11516 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/MemorySize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1662 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/DecoderError.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1520 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/FormatMnemonicOptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    62492 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/Mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)     3671 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/DecoderOptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35718 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/_iced_x86_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (116)     2270 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/ConditionCode.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1540 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CodeSize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1687 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/OpCodeTableKind.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_np.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1514 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/iced_x86/CC_e.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)     1766 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     9623 2020-12-06 22:35:42.000000 iced-x86-1.9.1/src/iced_x86.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    48404 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/formatter.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    73045 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/instruction.rs
+-rw-r--r--   0 runner    (1001) docker     (116)    11354 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/info.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     3901 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/constant_offsets.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4156 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     4951 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/block_encoder.rs
+-rw-r--r--   0 runner    (1001) docker     (116)     8121 2020-12-06 22:30:55.000000 iced-x86-1.9.1/src/fast_formatter.rs
```

### Comparing `iced-x86-1.19.0/LICENSE.txt` & `iced-x86-1.9.1/src/iced_x86/CC_g.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,45 @@
-https://github.com/icedland/iced
-Copyright (C) 2018-present iced project and contributors
+#
+# Copyright (C) 2018-2019 de4dot@gmail.com
+#
+# Permission is hereby granted, free of charge, to any person obtaining
+# a copy of this software and associated documentation files (the
+# "Software"), to deal in the Software without restriction, including
+# without limitation the rights to use, copy, modify, merge, publish,
+# distribute, sublicense, and/or sell copies of the Software, and to
+# permit persons to whom the Software is furnished to do so, subject to
+# the following conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+#
 
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+# ⚠️This file was generated by GENERATOR!🦹‍♂️
+
+# pylint: disable=invalid-name
+# pylint: disable=line-too-long
+# pylint: disable=too-many-lines
+
+"""
+Mnemonic condition code selector (eg. ``JG`` / ``JNLE``)
+"""
+
+from typing import List
+
+G: int = 0
+"""
+``JG``, ``CMOVG``, ``SETG``
+"""
+NLE: int = 1
+"""
+``JNLE``, ``CMOVNLE``, ``SETNLE``
+"""
+
+__all__: List[str] = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iced-x86-1.19.0/src/constant_offsets.rs` & `iced-x86-1.9.1/src/constant_offsets.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,85 @@
-// SPDX-License-Identifier: MIT
-// Copyright (C) 2018-present iced project and contributors
+/*
+Copyright (C) 2018-2019 de4dot@gmail.com
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+*/
 
 use core::hash::{Hash, Hasher};
 use pyo3::class::basic::CompareOp;
 use pyo3::prelude::*;
+use pyo3::PyObjectProtocol;
 use std::collections::hash_map::DefaultHasher;
 
 /// Contains the offsets of the displacement and immediate.
 ///
 /// Call :class:`Decoder.get_constant_offsets` or :class:`Encoder.get_constant_offsets` to get the
 /// offsets of the constants after the instruction has been decoded/encoded.
-#[pyclass(module = "iced_x86._iced_x86_py")]
-#[pyo3(text_signature = "(/)")]
-#[derive(Copy, Clone)]
-pub(crate) struct ConstantOffsets {
+#[pyclass(module = "_iced_x86_py")]
+#[text_signature = "(/)"]
+pub struct ConstantOffsets {
 	pub(crate) offsets: iced_x86::ConstantOffsets,
 }
 
 #[pymethods]
 impl ConstantOffsets {
-	/// int: (``u32``) The offset of the displacement, if any
+	/// int: (``usize``) The offset of the displacement, if any
 	#[getter]
-	fn displacement_offset(&self) -> u32 {
-		self.offsets.displacement_offset() as u32
+	fn displacement_offset(&self) -> usize {
+		self.offsets.displacement_offset()
 	}
 
-	/// int: (``u32``) Size in bytes of the displacement, or 0 if there's no displacement
+	/// int: (``usize``) Size in bytes of the displacement, or 0 if there's no displacement
 	#[getter]
-	fn displacement_size(&self) -> u32 {
-		self.offsets.displacement_size() as u32
+	fn displacement_size(&self) -> usize {
+		self.offsets.displacement_size()
 	}
 
-	/// int: (``u32``) The offset of the first immediate, if any.
+	/// int: (``usize``) The offset of the first immediate, if any.
 	///
 	/// This field can be invalid even if the operand has an immediate if it's an immediate that isn't part
 	/// of the instruction stream, eg. ``SHL AL,1``.
 	#[getter]
-	fn immediate_offset(&self) -> u32 {
-		self.offsets.immediate_offset() as u32
+	fn immediate_offset(&self) -> usize {
+		self.offsets.immediate_offset()
 	}
 
-	/// int: (``u32``) Size in bytes of the first immediate, or 0 if there's no immediate
+	/// int: (``usize``) Size in bytes of the first immediate, or 0 if there's no immediate
 	#[getter]
-	fn immediate_size(&self) -> u32 {
-		self.offsets.immediate_size() as u32
+	fn immediate_size(&self) -> usize {
+		self.offsets.immediate_size()
 	}
 
-	/// int: (``u32``) The offset of the second immediate, if any.
+	/// int: (``usize``) The offset of the second immediate, if any.
 	#[getter]
-	fn immediate_offset2(&self) -> u32 {
-		self.offsets.immediate_offset2() as u32
+	fn immediate_offset2(&self) -> usize {
+		self.offsets.immediate_offset2()
 	}
 
-	/// int: (``u32``) Size in bytes of the second immediate, or 0 if there's no second immediate
+	/// int: (``usize``) Size in bytes of the second immediate, or 0 if there's no second immediate
 	#[getter]
-	fn immediate_size2(&self) -> u32 {
-		self.offsets.immediate_size2() as u32
+	fn immediate_size2(&self) -> usize {
+		self.offsets.immediate_size2()
 	}
 
 	/// bool: ``True`` if :class:`ConstantOffsets.displacement_offset` and :class:`ConstantOffsets.displacement_size` are valid
 	#[getter]
 	fn has_displacement(&self) -> bool {
 		self.offsets.has_displacement()
 	}
@@ -71,50 +91,19 @@
 	}
 
 	/// bool: ``True`` if :class:`ConstantOffsets.immediate_offset2` and :class:`ConstantOffsets.immediate_size2` are valid
 	#[getter]
 	fn has_immediate2(&self) -> bool {
 		self.offsets.has_immediate2()
 	}
+}
 
-	/// Returns a copy of this instance.
-	///
-	/// Returns:
-	///     ConstantOffsets: A copy of this instance
-	///
-	/// This is identical to :class:`ConstantOffsets.copy`
-	#[pyo3(text_signature = "($self, /)")]
-	fn __copy__(&self) -> Self {
-		*self
-	}
-
-	/// Returns a copy of this instance.
-	///
-	/// Args:
-	///     memo (Any): memo dict
-	///
-	/// Returns:
-	///     ConstantOffsets: A copy of this instance
-	///
-	/// This is identical to :class:`ConstantOffsets.copy`
-	#[pyo3(text_signature = "($self, memo, /)")]
-	fn __deepcopy__(&self, _memo: &PyAny) -> Self {
-		*self
-	}
-
-	/// Returns a copy of this instance.
-	///
-	/// Returns:
-	///     ConstantOffsets: A copy of this instance
-	#[pyo3(text_signature = "($self, /)")]
-	fn copy(&self) -> Self {
-		*self
-	}
-
-	fn __richcmp__(&self, other: PyRef<'_, ConstantOffsets>, op: CompareOp) -> PyObject {
+#[pyproto]
+impl PyObjectProtocol for ConstantOffsets {
+	fn __richcmp__(&self, other: PyRef<ConstantOffsets>, op: CompareOp) -> PyObject {
 		match op {
 			CompareOp::Eq => (self.offsets == other.offsets).into_py(other.py()),
 			CompareOp::Ne => (self.offsets != other.offsets).into_py(other.py()),
 			_ => other.py().NotImplemented(),
 		}
 	}
```

### Comparing `iced-x86-1.19.0/src/decoder.rs` & `iced-x86-1.9.1/src/decoder.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,66 @@
-// SPDX-License-Identifier: MIT
-// Copyright (C) 2018-present iced project and contributors
+/*
+Copyright (C) 2018-2019 de4dot@gmail.com
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+*/
 
 use crate::constant_offsets::ConstantOffsets;
 use crate::instruction::Instruction;
-use crate::utils::to_value_error;
 use core::slice;
 use pyo3::class::iter::IterNextOutput;
-use pyo3::exceptions::PyTypeError;
-use pyo3::gc::PyVisit;
+use pyo3::exceptions::{PyTypeError, PyValueError};
+use pyo3::gc::{PyGCProtocol, PyVisit};
 use pyo3::prelude::*;
 use pyo3::types::{PyByteArray, PyBytes};
-use pyo3::PyTraverseError;
+use pyo3::{PyIterProtocol, PyTraverseError};
 
 enum DecoderDataRef {
 	None,
 	Vec(Vec<u8>),
 	PyObj(PyObject),
 }
 
 /// Decodes 16/32/64-bit x86 instructions
 ///
 /// Args:
 ///     bitness (int): 16, 32 or 64
 ///     data (bytes, bytearray): Data to decode. For best PERF, use :class:`bytes` since it's immutable and nothing gets copied.
 ///     options (:class:`DecoderOptions`): (default = :class:`DecoderOptions.NONE`) Decoder options, eg. :class:`DecoderOptions.NO_INVALID_CHECK` | :class:`DecoderOptions.AMD`
-///     ip (int): (``u64``) (default = ``0``) ``RIP`` value
 ///
 /// Raises:
 ///     ValueError: If `bitness` is invalid
 ///     TypeError: If `data` is not a supported type
 ///
 /// Examples:
 ///
 /// .. testcode::
 ///
 ///     from iced_x86 import *
 ///
 ///     data = b"\x86\x64\x32\x16\xF0\xF2\x83\x00\x5A\x62\xC1\xFE\xCB\x6F\xD3"
-///     decoder = Decoder(64, data, ip=0x1234_5678)
+///     decoder = Decoder(64, data)
+///     decoder.ip = 0x1234_5678
 ///
 ///     # The decoder is iterable
 ///     for instr in decoder:
 ///         print(f"Decoded: IP=0x{instr.ip:X}: {instr}")
 ///
 /// Output:
 ///
@@ -55,15 +74,16 @@
 ///
 ///     from iced_x86 import *
 ///
 ///     # xchg ah,[rdx+rsi+16h]
 ///     # xacquire lock add dword ptr [rax],5Ah
 ///     # vmovdqu64 zmm18{k3}{z},zmm11
 ///     data = b"\x86\x64\x32\x16\xF0\xF2\x83\x00\x5A\x62\xC1\xFE\xCB\x6F\xD3"
-///     decoder = Decoder(64, data, ip=0x1234_5678)
+///     decoder = Decoder(64, data)
+///     decoder.ip = 0x1234_5678
 ///
 ///     instr1 = decoder.decode()
 ///     assert instr1.code == Code.XCHG_RM8_R8
 ///     assert instr1.mnemonic == Mnemonic.XCHG
 ///     assert instr1.len == 4
 ///
 ///     instr2 = decoder.decode()
@@ -82,57 +102,64 @@
 ///
 /// .. testcode::
 ///
 ///     from iced_x86 import *
 ///
 ///     # lock add esi,ecx   # lock not allowed
 ///     data = b"\xF0\x01\xCE"
-///     decoder = Decoder(64, data, ip=0x1234_5678)
+///     decoder = Decoder(64, data)
+///     decoder.ip = 0x1234_5678
 ///     instr = decoder.decode()
 ///     assert instr.code == Code.INVALID
 ///
 ///     # We want to decode some instructions with invalid encodings
-///     decoder = Decoder(64, data, DecoderOptions.NO_INVALID_CHECK, 0x1234_5678)
+///     decoder = Decoder(64, data, DecoderOptions.NO_INVALID_CHECK)
+///     decoder.ip = 0x1234_5678
 ///     instr = decoder.decode()
 ///     assert instr.code == Code.ADD_RM32_R32
 ///     assert instr.has_lock_prefix
-#[pyclass(module = "iced_x86._iced_x86_py")]
-#[pyo3(text_signature = "(bitness, data, options, ip, /)")]
-pub(crate) struct Decoder {
+#[pyclass(module = "_iced_x86_py")]
+#[text_signature = "(bitness, data, options, /)"]
+pub struct Decoder {
 	// * If the decoder ctor was called with a `bytes` object, data_ref is PyObj(`bytes` object)
 	//   and the decoder holds a ref to its data.
 	// * If the decoder ctor was called with a `bytearray` object, data_ref is Vec(copy of `bytearray` data)
 	//   and the decoder holds a reference to this copied data.
 	data_ref: DecoderDataRef,
 	decoder: iced_x86::Decoder<'static>,
 }
 
+// iced_x86::Decoder has read only pointer fields which are !Send
+unsafe impl Send for Decoder {}
+
 #[pymethods]
 impl Decoder {
 	#[new]
-	#[args(options = 0, ip = 0)]
-	fn new(bitness: u32, data: &PyAny, options: u32, ip: u64) -> PyResult<Self> {
-		// #[args] line assumption
-		const _: () = assert!(iced_x86::DecoderOptions::NONE == 0);
+	#[args(options = 0)]
+	fn new(bitness: u32, data: &PyAny, options: u32) -> PyResult<Self> {
+		match bitness {
+			16 | 32 | 64 => {}
+			_ => return Err(PyValueError::new_err("bitness must be 16, 32 or 64")),
+		}
 
 		let (data_ref, decoder_data): (DecoderDataRef, &'static [u8]) = if let Ok(bytes) = <PyBytes as PyTryFrom>::try_from(data) {
 			let slice_data = bytes.as_bytes();
 			let decoder_data = unsafe { slice::from_raw_parts(slice_data.as_ptr(), slice_data.len()) };
 			(DecoderDataRef::PyObj(bytes.into()), decoder_data)
 		} else if let Ok(bytearray) = <PyByteArray as PyTryFrom>::try_from(data) {
 			//TODO: support bytearray without copying its data by getting a ref to its data every time the Decoder is used (also update the ctor args docs)
 			let vec_data: Vec<_> = unsafe { bytearray.as_bytes().into() };
 			let decoder_data = unsafe { slice::from_raw_parts(vec_data.as_ptr(), vec_data.len()) };
 			(DecoderDataRef::Vec(vec_data), decoder_data)
 		} else {
-			//TODO: support memoryview (also update docs and get_temporary_byte_array_ref and the message below)
+			//TODO: support memoryview
 			return Err(PyTypeError::new_err("Expected one of these types: bytes, bytearray"));
 		};
 
-		let decoder = iced_x86::Decoder::try_with_ip(bitness, decoder_data, ip, options).map_err(to_value_error)?;
+		let decoder = iced_x86::Decoder::new(bitness, decoder_data, options);
 		Ok(Decoder { data_ref, decoder })
 	}
 
 	/// int: (``u64``) The current ``IP``/``EIP``/``RIP`` value, see also :class:`Decoder.position`
 	///
 	/// Note:
 	///     The setter only updates the IP value, it does not change the data position, use the :class:`Decoder.position` setter to change the position.
@@ -172,15 +199,16 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # nop and pause
 	///     data = b"\x90\xF3\x90"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///
 	///     assert decoder.position == 0
 	///     assert decoder.max_position == 3
 	///     instr = decoder.decode()
 	///     assert decoder.position == 1
 	///     assert instr.code == Code.NOPD
 	///
@@ -197,16 +225,21 @@
 	///     assert decoder.position == 3
 	#[getter]
 	fn position(&self) -> usize {
 		self.decoder.position()
 	}
 
 	#[setter]
-	fn set_position(&mut self, new_value: usize) -> PyResult<()> {
-		self.decoder.set_position(new_value).map_err(to_value_error)
+	fn set_position(&mut self, new_pos: usize) -> PyResult<()> {
+		if new_pos > self.decoder.max_position() {
+			Err(PyValueError::new_err("Invalid position"))
+		} else {
+			self.decoder.set_position(new_pos);
+			Ok(())
+		}
 	}
 
 	/// bool: Returns ``True`` if there's at least one more byte to decode.
 	///
 	/// It doesn't verify that the next instruction is valid, it only checks if there's
 	/// at least one more byte to read. See also :class:`Decoder.position` and :class:`Decoder.max_position`.
 	///
@@ -217,15 +250,16 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # nop and an incomplete instruction
 	///     data = b"\x90\xF3\x0F"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///
 	///     # 3 bytes left to read
 	///     assert decoder.can_decode
 	///     instr = decoder.decode()
 	///     assert instr.code == Code.NOPD
 	///
 	///     # 2 bytes left to read
@@ -264,15 +298,16 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # xrelease lock add [rax],ebx
 	///     data = b"\xF0\xF3\x01\x18"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///     instr = decoder.decode()
 	///
 	///     assert instr.code == Code.ADD_RM32_R32
 	///     assert instr.mnemonic == Mnemonic.ADD
 	///     assert instr.len == 4
 	///     assert instr.op_count == 2
 	///
@@ -286,15 +321,15 @@
 	///     assert instr.memory_size == MemorySize.UINT32
 	///
 	///     assert instr.op1_kind == OpKind.REGISTER
 	///     assert instr.op1_register == Register.EBX
 	///
 	///     assert instr.has_lock_prefix
 	///     assert instr.has_xrelease_prefix
-	#[pyo3(text_signature = "($self, /)")]
+	#[text_signature = "($self, /)"]
 	fn decode(&mut self) -> Instruction {
 		Instruction { instr: self.decoder.decode() }
 	}
 
 	/// Decodes the next instruction.
 	///
 	/// The difference between this method and :class:`Decoder.decode` is that this method doesn't need to
@@ -309,15 +344,16 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # xrelease lock add [rax],ebx
 	///     data = b"\xF0\xF3\x01\x18"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///     instr = Instruction()
 	///     decoder.decode_out(instr)
 	///
 	///     assert instr.code == Code.ADD_RM32_R32
 	///     assert instr.mnemonic == Mnemonic.ADD
 	///     assert instr.len == 4
 	///     assert instr.op_count == 2
@@ -332,15 +368,15 @@
 	///     assert instr.memory_size == MemorySize.UINT32
 	///
 	///     assert instr.op1_kind == OpKind.REGISTER
 	///     assert instr.op1_register == Register.EBX
 	///
 	///     assert instr.has_lock_prefix
 	///     assert instr.has_xrelease_prefix
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction, /)"]
 	fn decode_out(&mut self, instruction: &mut Instruction) {
 		self.decoder.decode_out(&mut instruction.instr)
 	}
 
 	/// Gets the offsets of the constants (memory displacement and immediate) in the decoded instruction.
 	///
 	/// The caller can check if there are any relocations at those addresses.
@@ -358,53 +394,59 @@
 	///     from iced_x86 import *
 	///
 	///     # nop
 	///     # xor dword ptr [rax-5AA5EDCCh],5Ah
 	///     #              00  01  02  03  04  05  06
 	///     #            \opc\mrm\displacement___\imm
 	///     data = b"\x90\x83\xB3\x34\x12\x5A\xA5\x5A"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///     assert decoder.decode().code == Code.NOPD
 	///     instr = decoder.decode()
 	///     co = decoder.get_constant_offsets(instr)
 	///
 	///     assert co.has_displacement
 	///     assert co.displacement_offset == 2
 	///     assert co.displacement_size == 4
 	///     assert co.has_immediate
 	///     assert co.immediate_offset == 6
 	///     assert co.immediate_size == 1
 	///     # It's not an instruction with two immediates (e.g. enter)
 	///     assert not co.has_immediate2
 	///     assert co.immediate_offset2 == 0
 	///     assert co.immediate_size2 == 0
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction, /)"]
 	fn get_constant_offsets(&self, instruction: &Instruction) -> ConstantOffsets {
 		ConstantOffsets { offsets: self.decoder.get_constant_offsets(&instruction.instr) }
 	}
+}
 
-	fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
+#[pyproto]
+impl PyGCProtocol for Decoder {
+	fn __traverse__(&self, visit: PyVisit) -> Result<(), PyTraverseError> {
 		if let DecoderDataRef::PyObj(ref data_obj) = self.data_ref {
 			visit.call(data_obj)?
 		}
 		Ok(())
 	}
 
 	fn __clear__(&mut self) {
 		if let DecoderDataRef::PyObj(_) = self.data_ref {
-			self.decoder = iced_x86::Decoder::new(64, b"", iced_x86::DecoderOptions::NONE);
 			self.data_ref = DecoderDataRef::None;
 		}
 	}
+}
 
-	fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
+#[pyproto]
+impl PyIterProtocol for Decoder {
+	fn __iter__(slf: PyRef<Self>) -> PyRef<Self> {
 		slf
 	}
 
-	fn __next__(mut slf: PyRefMut<'_, Self>) -> IterNextOutput<Instruction, ()> {
-		if slf.can_decode() {
+	fn __next__(mut slf: PyRefMut<Self>) -> IterNextOutput<Instruction, ()> {
+		if slf.decoder.can_decode() {
 			IterNextOutput::Yield(slf.decode())
 		} else {
 			IterNextOutput::Return(())
 		}
 	}
 }
```

### Comparing `iced-x86-1.19.0/src/encoder.rs` & `iced-x86-1.9.1/src/encoder.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,93 @@
-// SPDX-License-Identifier: MIT
-// Copyright (C) 2018-present iced project and contributors
+/*
+Copyright (C) 2018-2019 de4dot@gmail.com
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+*/
 
 use crate::constant_offsets::ConstantOffsets;
 use crate::instruction::Instruction;
-use crate::utils::to_value_error;
+use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
 /// Encodes instructions decoded by the decoder or instructions created by other code.
 ///
 /// See also :class:`BlockEncoder` which can encode any number of instructions.
 ///
 /// Args:
 ///     bitness (int): 16, 32 or 64
-///     capacity (int): (default = 0) Initial capacity of the byte buffer
 ///
 /// Raises:
 ///     ValueError: If `bitness` is invalid
 ///
 /// Examples:
 ///
 /// .. testcode::
 ///
 ///     from iced_x86 import *
 ///
 ///     # xchg ah,[rdx+rsi+16h]
 ///     data = b"\x86\x64\x32\x16"
-///     decoder = Decoder(64, data, ip=0x1234_5678)
+///     decoder = Decoder(64, data)
+///     decoder.ip = 0x1234_5678
 ///     instr = decoder.decode()
 ///
 ///     encoder = Encoder(64)
 ///     try:
 ///         instr_len = encoder.encode(instr, 0x5555_5555)
 ///         assert instr_len == 4
 ///     except ValueError as ex:
 ///         print(f"Failed to encode the instruction: {ex}")
 ///         raise
 ///
 ///     # We're done, take ownership of the buffer
 ///     buffer = encoder.take_buffer()
 ///     assert buffer == b"\x86\x64\x32\x16"
-#[pyclass(module = "iced_x86._iced_x86_py")]
-#[pyo3(text_signature = "(bitness, capacity, /)")]
-pub(crate) struct Encoder {
+#[pyclass(module = "_iced_x86_py")]
+#[text_signature = "(bitness, capacity, /)"]
+pub struct Encoder {
 	encoder: iced_x86::Encoder,
 }
 
 #[pymethods]
 impl Encoder {
 	#[new]
 	#[args(capacity = 0)]
 	fn new(bitness: u32, capacity: usize) -> PyResult<Self> {
-		let encoder = iced_x86::Encoder::try_with_capacity(bitness, capacity).map_err(to_value_error)?;
-		Ok(Self { encoder })
+		match bitness {
+			16 | 32 | 64 => {}
+			_ => return Err(PyValueError::new_err("bitness must be 16, 32 or 64")),
+		}
+
+		Ok(Self { encoder: iced_x86::Encoder::with_capacity(bitness, capacity) })
 	}
 
 	/// Encodes an instruction and returns the size of the encoded instruction
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction to encode
-	///     `rip` (int): (``u64``) ``RIP`` of the encoded instruction
+	///     `rip`(int): (``u64``) ``RIP`` of the encoded instruction
 	///
 	/// Returns:
 	///     int: Size of the encoded instruction
 	///
 	/// Raises:
 	///     ValueError: If it failed to encode the instruction (eg. a target branch / RIP-rel operand is too far away)
 	///
@@ -71,32 +95,36 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # je short $+4
 	///     data = b"\x75\x02"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///     instr = decoder.decode()
 	///
 	///     encoder = Encoder(64)
 	///     try:
 	///         # Use a different IP (orig rip + 0x10)
 	///         instr_len = encoder.encode(instr, 0x1234_5688)
 	///         assert instr_len == 2
 	///     except ValueError as ex:
 	///         print(f"Failed to encode the instruction: {ex}")
 	///         raise
 	///
 	///     # We're done, take ownership of the buffer
 	///     buffer = encoder.take_buffer()
 	///     assert buffer == b"\x75\xF2"
-	#[pyo3(text_signature = "($self, instruction, rip, /)")]
+	#[text_signature = "($self, instruction, rip, /)"]
 	fn encode(&mut self, instruction: &Instruction, rip: u64) -> PyResult<usize> {
-		self.encoder.encode(&instruction.instr, rip).map_err(to_value_error)
+		match self.encoder.encode(&instruction.instr, rip) {
+			Ok(len) => Ok(len),
+			Err(err) => Err(PyValueError::new_err(format!("{}", err))),
+		}
 	}
 
 	/// Writes a byte to the output buffer
 	///
 	/// Args:
 	///     `value` (int): (``u8``) Value to write
 	///
@@ -104,15 +132,16 @@
 	///
 	/// .. testcode::
 	///
 	///     from iced_x86 import *
 	///
 	///     # je short $+4
 	///     data = b"\x75\x02"
-	///     decoder = Decoder(64, data, ip=0x1234_5678)
+	///     decoder = Decoder(64, data)
+	///     decoder.ip = 0x1234_5678
 	///     instr = decoder.decode()
 	///
 	///     encoder = Encoder(64)
 	///     # Add a random byte
 	///     encoder.write_u8(0x90)
 	///
 	///     try:
@@ -125,38 +154,38 @@
 	///
 	///     # Add a random byte
 	///     encoder.write_u8(0x90)
 	///
 	///     # We're done, take ownership of the buffer
 	///     buffer = encoder.take_buffer()
 	///     assert buffer == b"\x90\x75\xF2\x90"
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value, /)"]
 	fn write_u8(&mut self, value: u8) {
 		self.encoder.write_u8(value)
 	}
 
 	/// Returns the buffer and initializes the internal buffer to an empty array.
 	///
 	/// Should be called when you've encoded all instructions and need the raw instruction bytes.
 	///
 	/// Returns:
 	///     bytes: The encoded instructions
-	#[pyo3(text_signature = "($self, /)")]
-	fn take_buffer<'py>(&mut self, py: Python<'py>) -> &'py PyBytes {
+	#[text_signature = "($self, /)"]
+	fn take_buffer<'py>(&mut self, py: Python<'py>) -> PyResult<&'py PyBytes> {
 		let buffer = self.encoder.take_buffer();
-		PyBytes::new(py, &buffer)
+		Ok(PyBytes::new(py, &buffer))
 	}
 
 	/// Gets the offsets of the constants (memory displacement and immediate) in the encoded instruction.
 	///
 	/// The caller can use this information to add relocations if needed.
 	///
 	/// Returns:
 	///     ConstantOffsets: Offsets and sizes of immediates
-	#[pyo3(text_signature = "($self, /)")]
+	#[text_signature = "($self, /)"]
 	fn get_constant_offsets(&self) -> ConstantOffsets {
 		ConstantOffsets { offsets: self.encoder.get_constant_offsets() }
 	}
 
 	/// bool: Disables 2-byte VEX encoding and encodes all VEX instructions with the 3-byte VEX encoding
 	#[getter]
 	fn prevent_vex2(&self) -> bool {
@@ -208,24 +237,13 @@
 	}
 
 	#[setter]
 	fn set_evex_lig(&mut self, new_value: u32) {
 		self.encoder.set_evex_lig(new_value)
 	}
 
-	/// int: (``u8``) Value of the ``MVEX.W`` bit to use if it's an instruction that ignores the bit. Default is 0.
-	#[getter]
-	fn mvex_wig(&self) -> u32 {
-		self.encoder.mvex_wig()
-	}
-
-	#[setter]
-	fn set_mvex_wig(&mut self, new_value: u32) {
-		self.encoder.set_mvex_wig(new_value)
-	}
-
-	/// int: Gets the bitness (16, 32 or 64)
+	/// Gets the bitness (16, 32 or 64)
 	#[getter]
 	fn bitness(&self) -> u32 {
 		self.encoder.bitness()
 	}
 }
```

### Comparing `iced-x86-1.19.0/src/formatter.rs` & `iced-x86-1.9.1/src/formatter.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,35 @@
-// SPDX-License-Identifier: MIT
-// Copyright (C) 2018-present iced project and contributors
+/*
+Copyright (C) 2018-2019 de4dot@gmail.com
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+*/
 
 use crate::enum_utils::{
 	to_cc_a, to_cc_ae, to_cc_b, to_cc_be, to_cc_e, to_cc_g, to_cc_ge, to_cc_l, to_cc_le, to_cc_ne, to_cc_np, to_cc_p, to_memory_size_options,
 	to_register,
 };
 use crate::instruction::Instruction;
-use crate::utils::to_value_error;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 
 // GENERATOR-BEGIN: FormatterSyntax
 // ⚠️This was generated by GENERATOR!🦹‍♂️
 /// Formatter syntax (GNU Assembler, Intel XED, masm, nasm)
 #[allow(dead_code)]
@@ -41,17 +60,17 @@
 ///     decoder = Decoder(64, data)
 ///     instr = decoder.decode()
 ///
 ///     formatter = Formatter(FormatterSyntax.MASM)
 ///     formatter.uppercase_mnemonics = True
 ///     disasm = formatter.format(instr)
 ///     assert disasm == "VCVTNE2PS2BF16 zmm2{k5}{z},zmm6,dword bcst [rax+4]"
-#[pyclass(module = "iced_x86._iced_x86_py")]
-#[pyo3(text_signature = "(syntax, /)")]
-pub(crate) struct Formatter {
+#[pyclass(module = "_iced_x86_py")]
+#[text_signature = "(syntax, /)"]
+pub struct Formatter {
 	fmt_output: String,
 	formatter: Box<dyn iced_x86::Formatter>,
 }
 
 unsafe impl Send for Formatter {}
 
 #[pymethods]
@@ -76,70 +95,69 @@
 	/// Formats the whole instruction: prefixes, mnemonic, operands
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction to format
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction)"]
 	fn format(&mut self, instruction: &Instruction) -> &str {
 		self.fmt_output.clear();
 		self.formatter.format(&instruction.instr, &mut self.fmt_output);
 		&self.fmt_output
 	}
 
 	/// Formats the mnemonic and any prefixes
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction to format
 	///     `options` (:class:`FormatMnemonicOptions`): (default = :class:`FormatMnemonicOptions.NONE`) Options
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, instruction, options, /)")]
+	#[text_signature = "($self, instruction, options)"]
 	#[args(options = 0)]
 	fn format_mnemonic(&mut self, instruction: &Instruction, options: u32) -> &str {
-		// #[args] line assumption
-		const _: () = assert!(iced_x86::FormatMnemonicOptions::NONE == 0);
-
+		const_assert_eq!(0, iced_x86::FormatMnemonicOptions::NONE);
 		self.fmt_output.clear();
 		self.formatter.format_mnemonic_options(&instruction.instr, &mut self.fmt_output, options);
 		&self.fmt_output
 	}
 
 	/// Gets the number of operands that will be formatted. A formatter can add and remove operands
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction
 	///
 	/// Returns:
 	///     int: Operand count
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction)"]
 	fn operand_count(&mut self, instruction: &Instruction) -> u32 {
 		self.formatter.operand_count(&instruction.instr)
 	}
 
 	/// Returns the operand access but only if it's an operand added by the formatter.
 	///
-	/// If it's an operand that is part of :class:`Instruction`, you should call eg. :class:`InstructionInfoFactory.info`.
+	/// If it's an operand that is part of :class:`Instruction`, you should call eg. `InstructionInfoFactory::info`.
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction
 	///     `operand` (int): Operand number, 0-based. This is a formatter operand and isn't necessarily the same as an instruction operand. See :class:`Formatter.operand_count`
 	///
 	/// Returns:
 	///     :class:`OpAccess`, None: Operand access or ``None``
 	///
 	/// Raises:
 	///     ValueError: If `operand` is invalid
-	#[pyo3(text_signature = "($self, instruction, operand, /)")]
+	#[text_signature = "($self, instruction, operand)"]
 	fn op_access(&mut self, instruction: &Instruction, operand: u32) -> PyResult<Option<u32>> {
-		self.formatter
-			.op_access(&instruction.instr, operand)
-			.map_or_else(|_| Err(PyValueError::new_err("Invalid operand")), |res| Ok(res.map(|v| v as u32)))
+		match self.formatter.op_access(&instruction.instr, operand) {
+			Ok(res) => Ok(res.map(|v| v as u32)),
+			Err(_) => Err(PyValueError::new_err("Invalid operand")),
+		}
 	}
 
 	/// Converts a formatter operand index to an instruction operand index.
 	///
 	/// Returns ``None`` if it's an operand added by the formatter
 	///
 	/// Args:
@@ -147,17 +165,17 @@
 	///     `operand` (int): Operand number, 0-based. This is a formatter operand and isn't necessarily the same as an instruction operand. See :class:`Formatter.operand_count`
 	///
 	/// Returns:
 	///     int, None: Instruction operand or ``None`` if it's an operand added by the formatter
 	///
 	/// Raises:
 	///     ValueError: If `operand` is invalid
-	#[pyo3(text_signature = "($self, instruction, operand, /)")]
+	#[text_signature = "($self, instruction, operand)"]
 	fn get_instruction_operand(&mut self, instruction: &Instruction, operand: u32) -> PyResult<Option<u32>> {
-		self.formatter.get_instruction_operand(&instruction.instr, operand).map_err(to_value_error)
+		self.formatter.get_instruction_operand(&instruction.instr, operand).map_err(|_| PyValueError::new_err("Invalid operand"))
 	}
 
 	/// Converts an instruction operand index to a formatter operand index.
 	///
 	/// Returns ``None`` if the instruction operand isn't used by the formatter
 	///
 	/// Args:
@@ -165,726 +183,728 @@
 	///     `instruction_operand` (int): Instruction operand
 	///
 	/// Returns:
 	///     int, None: Instruction operand or ``None`` if the instruction operand isn't used by the formatter
 	///
 	/// Raises:
 	///     ValueError: If `instruction_operand` is invalid
-	#[pyo3(text_signature = "($self, instruction, instruction_operand, /)")]
+	#[text_signature = "($self, instruction, instruction_operand)"]
 	fn get_formatter_operand(&mut self, instruction: &Instruction, instruction_operand: u32) -> PyResult<Option<u32>> {
-		self.formatter.get_formatter_operand(&instruction.instr, instruction_operand).map_err(to_value_error)
+		self.formatter
+			.get_formatter_operand(&instruction.instr, instruction_operand)
+			.map_err(|_| PyValueError::new_err("Invalid instruction operand"))
 	}
 
 	/// Formats an operand.
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction
 	///     `operand` (int): Operand number, 0-based. This is a formatter operand and isn't necessarily the same as an instruction operand. See :class:`Formatter.operand_count`
 	///
 	/// Returns:
 	///     str: The formatted string
 	///
 	/// Raises:
 	///     ValueError: If `operand` is invalid
-	#[pyo3(text_signature = "($self, instruction, operand, /)")]
+	#[text_signature = "($self, instruction, operand)"]
 	fn format_operand(&mut self, instruction: &Instruction, operand: u32) -> PyResult<&str> {
 		self.fmt_output.clear();
-		self.formatter.format_operand(&instruction.instr, &mut self.fmt_output, operand).map_err(to_value_error)?;
+		self.formatter.format_operand(&instruction.instr, &mut self.fmt_output, operand).map_err(|_| PyValueError::new_err("Invalid operand"))?;
 		Ok(&self.fmt_output)
 	}
 
 	/// Formats an operand separator
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction)"]
 	fn format_operand_separator(&mut self, instruction: &Instruction) -> &str {
 		self.fmt_output.clear();
 		self.formatter.format_operand_separator(&instruction.instr, &mut self.fmt_output);
 		&self.fmt_output
 	}
 
 	/// Formats all operands
 	///
 	/// Args:
 	///     `instruction` (Instruction): Instruction to format
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, instruction, /)")]
+	#[text_signature = "($self, instruction)"]
 	fn format_all_operands(&mut self, instruction: &Instruction) -> &str {
 		self.fmt_output.clear();
 		self.formatter.format_all_operands(&instruction.instr, &mut self.fmt_output);
 		&self.fmt_output
 	}
 
 	/// Formats a register
 	///
 	/// Args:
 	///     `register` (:class:`Register`): Register
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, register, /)")]
+	#[text_signature = "($self, register)"]
 	fn format_register(&mut self, register: u32) -> PyResult<&str> {
 		Ok(self.formatter.format_register(to_register(register)?))
 	}
 
 	/// Formats a ``i8``
 	///
 	/// Args:
 	///     `value` (int): (``i8``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_i8(&mut self, value: i8) -> &str {
 		self.formatter.format_i8(value)
 	}
 
 	/// Formats a ``i16``
 	///
 	/// Args:
 	///     `value` (int): (``i16``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_i16(&mut self, value: i16) -> &str {
 		self.formatter.format_i16(value)
 	}
 
 	/// Formats a ``i32``
 	///
 	/// Args:
 	///     `value` (int): (``i32``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_i32(&mut self, value: i32) -> &str {
 		self.formatter.format_i32(value)
 	}
 
 	/// Formats a ``i64``
 	///
 	/// Args:
 	///     `value` (int): (``i64``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_i64(&mut self, value: i64) -> &str {
 		self.formatter.format_i64(value)
 	}
 
 	/// Formats a ``u8``
 	///
 	/// Args:
 	///     `value` (int): (``u8``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_u8(&mut self, value: u8) -> &str {
 		self.formatter.format_u8(value)
 	}
 
 	/// Formats a ``u16``
 	///
 	/// Args:
 	///     `value` (int): (``u16``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_u16(&mut self, value: u16) -> &str {
 		self.formatter.format_u16(value)
 	}
 
 	/// Formats a ``u32``
 	///
 	/// Args:
 	///     `value` (int): (``u32``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_u32(&mut self, value: u32) -> &str {
 		self.formatter.format_u32(value)
 	}
 
 	/// Formats a ``u64``
 	///
 	/// Args:
 	///     `value` (int): (``u64``) Value
 	///
 	/// Returns:
 	///     str: The formatted string
-	#[pyo3(text_signature = "($self, value, /)")]
+	#[text_signature = "($self, value)"]
 	fn format_u64(&mut self, value: u64) -> &str {
 		self.formatter.format_u64(value)
 	}
 
-	/// bool: Prefixes are uppercased
+	/// bool: Prefixes are upper cased
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``REP stosd``
-	/// 👍          ``False``   ``rep stosd``
+	/// ✔️          ``False``   ``rep stosd``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_prefixes(&self) -> bool {
 		self.formatter.options().uppercase_prefixes()
 	}
 
 	#[setter]
-	fn set_uppercase_prefixes(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_prefixes(new_value);
+	fn set_uppercase_prefixes(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_prefixes(value);
 	}
 
-	/// bool: Mnemonics are uppercased
+	/// bool: Mnemonics are upper cased
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``MOV rcx,rax``
-	/// 👍          ``False``   ``mov rcx,rax``
+	/// ✔️          ``False``   ``mov rcx,rax``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_mnemonics(&self) -> bool {
 		self.formatter.options().uppercase_mnemonics()
 	}
 
 	#[setter]
-	fn set_uppercase_mnemonics(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_mnemonics(new_value);
+	fn set_uppercase_mnemonics(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_mnemonics(value);
 	}
 
-	/// bool: Registers are uppercased
+	/// bool: Registers are upper cased
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov RCX,[RAX+RDX*8]``
-	/// 👍          ``False``   ``mov rcx,[rax+rdx*8]``
+	/// ✔️          ``False``   ``mov rcx,[rax+rdx*8]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_registers(&self) -> bool {
 		self.formatter.options().uppercase_registers()
 	}
 
 	#[setter]
-	fn set_uppercase_registers(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_registers(new_value);
+	fn set_uppercase_registers(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_registers(value);
 	}
 
-	/// bool: Keywords are uppercased (eg. ``BYTE PTR``, ``SHORT``)
+	/// bool: Keywords are upper cased (eg. ``BYTE PTR``, ``SHORT``)
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov BYTE PTR [rcx],12h``
-	/// 👍          ``False``   ``mov byte ptr [rcx],12h``
+	/// ✔️          ``False``   ``mov byte ptr [rcx],12h``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_keywords(&self) -> bool {
 		self.formatter.options().uppercase_keywords()
 	}
 
 	#[setter]
-	fn set_uppercase_keywords(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_keywords(new_value);
+	fn set_uppercase_keywords(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_keywords(value);
 	}
 
-	/// bool: Uppercase decorators, eg. ``{z}``, ``{sae}``, ``{rd-sae}`` (but not opmask registers: ``{k1}``)
+	/// bool: Upper case decorators, eg. ``{z}``, ``{sae}``, ``{rd-sae}`` (but not op mask registers: ``{k1}``)
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``vunpcklps xmm2{k5}{Z},xmm6,dword bcst [rax+4]``
-	/// 👍          ``False``   ``vunpcklps xmm2{k5}{z},xmm6,dword bcst [rax+4]``
+	/// ✔️          ``False``   ``vunpcklps xmm2{k5}{z},xmm6,dword bcst [rax+4]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_decorators(&self) -> bool {
 		self.formatter.options().uppercase_decorators()
 	}
 
 	#[setter]
-	fn set_uppercase_decorators(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_decorators(new_value);
+	fn set_uppercase_decorators(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_decorators(value);
 	}
 
-	/// bool: Everything is uppercased, except numbers and their prefixes/suffixes
+	/// bool: Everything is upper cased, except numbers and their prefixes/suffixes
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``MOV EAX,GS:[RCX*4+0ffh]``
-	/// 👍          ``False``   ``mov eax,gs:[rcx*4+0ffh]``
+	/// ✔️          ``False``   ``mov eax,gs:[rcx*4+0ffh]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_all(&self) -> bool {
 		self.formatter.options().uppercase_all()
 	}
 
 	#[setter]
-	fn set_uppercase_all(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_all(new_value);
+	fn set_uppercase_all(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_all(value);
 	}
 
 	/// int: (``u32``) Character index (0-based) where the first operand is formatted. Can be set to 0 to format it immediately after the mnemonic.
 	/// At least one space or tab is always added between the mnemonic and the first operand.
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``0``      ``mov•rcx,rbp``
+	/// ✔️          ``0``      ``mov•rcx,rbp``
 	/// \           ``8``      ``mov•••••rcx,rbp``
 	/// =========== ========== ================================================
 	#[getter]
 	fn first_operand_char_index(&self) -> u32 {
 		self.formatter.options().first_operand_char_index()
 	}
 
 	#[setter]
-	fn set_first_operand_char_index(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_first_operand_char_index(new_value);
+	fn set_first_operand_char_index(&mut self, value: u32) {
+		self.formatter.options_mut().set_first_operand_char_index(value);
 	}
 
 	/// int: (``u32``) Size of a tab character or 0 to use spaces
 	///
 	/// Default: ``0``
 	#[getter]
 	fn tab_size(&self) -> u32 {
 		self.formatter.options().tab_size()
 	}
 
 	#[setter]
-	fn set_tab_size(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_tab_size(new_value);
+	fn set_tab_size(&mut self, value: u32) {
+		self.formatter.options_mut().set_tab_size(value);
 	}
 
 	/// bool: Add a space after the operand separator
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov rax, rcx``
-	/// 👍          ``False``   ``mov rax,rcx``
+	/// ✔️          ``False``   ``mov rax,rcx``
 	/// =========== ========== ================================================
 	#[getter]
 	fn space_after_operand_separator(&self) -> bool {
 		self.formatter.options().space_after_operand_separator()
 	}
 
 	#[setter]
-	fn set_space_after_operand_separator(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_space_after_operand_separator(new_value);
+	fn set_space_after_operand_separator(&mut self, value: bool) {
+		self.formatter.options_mut().set_space_after_operand_separator(value);
 	}
 
 	/// bool: Add a space between the memory expression and the brackets
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[ rcx+rdx ]``
-	/// 👍          ``False``   ``mov eax,[rcx+rdx]``
+	/// ✔️          ``False``   ``mov eax,[rcx+rdx]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn space_after_memory_bracket(&self) -> bool {
 		self.formatter.options().space_after_memory_bracket()
 	}
 
 	#[setter]
-	fn set_space_after_memory_bracket(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_space_after_memory_bracket(new_value);
+	fn set_space_after_memory_bracket(&mut self, value: bool) {
+		self.formatter.options_mut().set_space_after_memory_bracket(value);
 	}
 
 	/// bool: Add spaces between memory operand ``+`` and ``-`` operators
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[rcx + rdx*8 - 80h]``
-	/// 👍          ``False``   ``mov eax,[rcx+rdx*8-80h]``
+	/// ✔️          ``False``   ``mov eax,[rcx+rdx*8-80h]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn space_between_memory_add_operators(&self) -> bool {
 		self.formatter.options().space_between_memory_add_operators()
 	}
 
 	#[setter]
-	fn set_space_between_memory_add_operators(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_space_between_memory_add_operators(new_value);
+	fn set_space_between_memory_add_operators(&mut self, value: bool) {
+		self.formatter.options_mut().set_space_between_memory_add_operators(value);
 	}
 
 	/// bool: Add spaces between memory operand ``*`` operator
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[rcx+rdx * 8-80h]``
-	/// 👍          ``False``   ``mov eax,[rcx+rdx*8-80h]``
+	/// ✔️          ``False``   ``mov eax,[rcx+rdx*8-80h]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn space_between_memory_mul_operators(&self) -> bool {
 		self.formatter.options().space_between_memory_mul_operators()
 	}
 
 	#[setter]
-	fn set_space_between_memory_mul_operators(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_space_between_memory_mul_operators(new_value);
+	fn set_space_between_memory_mul_operators(&mut self, value: bool) {
+		self.formatter.options_mut().set_space_between_memory_mul_operators(value);
 	}
 
 	/// bool: Show memory operand scale value before the index register
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[8*rdx]``
-	/// 👍          ``False``   ``mov eax,[rdx*8]``
+	/// ✔️          ``False``   ``mov eax,[rdx*8]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn scale_before_index(&self) -> bool {
 		self.formatter.options().scale_before_index()
 	}
 
 	#[setter]
-	fn set_scale_before_index(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_scale_before_index(new_value);
+	fn set_scale_before_index(&mut self, value: bool) {
+		self.formatter.options_mut().set_scale_before_index(value);
 	}
 
 	/// bool: Always show the scale value even if it's ``*1``
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[rbx+rcx*1]``
-	/// 👍          ``False``   ``mov eax,[rbx+rcx]``
+	/// ✔️          ``False``   ``mov eax,[rbx+rcx]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn always_show_scale(&self) -> bool {
 		self.formatter.options().always_show_scale()
 	}
 
 	#[setter]
-	fn set_always_show_scale(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_always_show_scale(new_value);
+	fn set_always_show_scale(&mut self, value: bool) {
+		self.formatter.options_mut().set_always_show_scale(value);
 	}
 
 	/// bool: Always show the effective segment register.
 	///
 	/// If the option is ``False``, only show the segment register if there's a segment override prefix.
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,ds:[ecx]``
-	/// 👍          ``False``   ``mov eax,[ecx]``
+	/// ✔️          ``False``   ``mov eax,[ecx]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn always_show_segment_register(&self) -> bool {
 		self.formatter.options().always_show_segment_register()
 	}
 
 	#[setter]
-	fn set_always_show_segment_register(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_always_show_segment_register(new_value);
+	fn set_always_show_segment_register(&mut self, value: bool) {
+		self.formatter.options_mut().set_always_show_segment_register(value);
 	}
 
 	/// bool: Show zero displacements
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[rcx*2+0]``
-	/// 👍          ``False``   ``mov eax,[rcx*2]``
+	/// ✔️          ``False``   ``mov eax,[rcx*2]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn show_zero_displacements(&self) -> bool {
 		self.formatter.options().show_zero_displacements()
 	}
 
 	#[setter]
-	fn set_show_zero_displacements(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_show_zero_displacements(new_value);
+	fn set_show_zero_displacements(&mut self, value: bool) {
+		self.formatter.options_mut().set_show_zero_displacements(value);
 	}
 
 	/// str: Hex number prefix or an empty string, eg. ``"0x"``
 	///
 	/// Default: ``""`` (masm/nasm/intel), ``"0x"`` (gas)
 	#[getter]
 	fn hex_prefix(&self) -> &str {
 		self.formatter.options().hex_prefix()
 	}
 
 	#[setter]
-	fn set_hex_prefix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_hex_prefix_string(new_value);
+	fn set_hex_prefix(&mut self, value: String) {
+		self.formatter.options_mut().set_hex_prefix_string(value);
 	}
 
 	/// str: Hex number suffix or an empty string, eg. ``"h"``
 	///
 	/// Default: ``"h"`` (masm/nasm/intel), ``""`` (gas)
 	#[getter]
 	fn hex_suffix(&self) -> &str {
 		self.formatter.options().hex_suffix()
 	}
 
 	#[setter]
-	fn set_hex_suffix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_hex_suffix_string(new_value);
+	fn set_hex_suffix(&mut self, value: String) {
+		self.formatter.options_mut().set_hex_suffix_string(value);
 	}
 
 	/// int: (``u8``) Size of a digit group, see also :class:`Formatter.digit_separator`
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``0``      ``0x12345678``
-	/// 👍          ``4``      ``0x1234_5678``
+	/// ✔️          ``4``      ``0x1234_5678``
 	/// =========== ========== ================================================
 	#[getter]
 	fn hex_digit_group_size(&self) -> u32 {
 		self.formatter.options().hex_digit_group_size()
 	}
 
 	#[setter]
-	fn set_hex_digit_group_size(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_hex_digit_group_size(new_value);
+	fn set_hex_digit_group_size(&mut self, value: u32) {
+		self.formatter.options_mut().set_hex_digit_group_size(value);
 	}
 
 	/// str: Decimal number prefix or an empty string
 	///
 	/// Default: ``""``
 	#[getter]
 	fn decimal_prefix(&self) -> &str {
 		self.formatter.options().decimal_prefix()
 	}
 
 	#[setter]
-	fn set_decimal_prefix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_decimal_prefix_string(new_value);
+	fn set_decimal_prefix(&mut self, value: String) {
+		self.formatter.options_mut().set_decimal_prefix_string(value);
 	}
 
 	/// str: Decimal number suffix or an empty string
 	///
 	/// Default: ``""``
 	#[getter]
 	fn decimal_suffix(&self) -> &str {
 		self.formatter.options().decimal_suffix()
 	}
 
 	#[setter]
-	fn set_decimal_suffix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_decimal_suffix_string(new_value);
+	fn set_decimal_suffix(&mut self, value: String) {
+		self.formatter.options_mut().set_decimal_suffix_string(value);
 	}
 
 	/// int: (``u8``) Size of a digit group, see also :class:`Formatter.digit_separator`
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``0``      ``12345678``
-	/// 👍          ``3``      ``12_345_678``
+	/// ✔️          ``3``      ``12_345_678``
 	/// =========== ========== ================================================
 	#[getter]
 	fn decimal_digit_group_size(&self) -> u32 {
 		self.formatter.options().decimal_digit_group_size()
 	}
 
 	#[setter]
-	fn set_decimal_digit_group_size(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_decimal_digit_group_size(new_value);
+	fn set_decimal_digit_group_size(&mut self, value: u32) {
+		self.formatter.options_mut().set_decimal_digit_group_size(value);
 	}
 
 	/// str: Octal number prefix or an empty string
 	///
 	/// Default: ``""`` (masm/nasm/intel), ``"0"`` (gas)
 	#[getter]
 	fn octal_prefix(&self) -> &str {
 		self.formatter.options().octal_prefix()
 	}
 
 	#[setter]
-	fn set_octal_prefix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_octal_prefix_string(new_value);
+	fn set_octal_prefix(&mut self, value: String) {
+		self.formatter.options_mut().set_octal_prefix_string(value);
 	}
 
 	/// str: Octal number suffix or an empty string
 	///
 	/// Default: ``"o"`` (masm/nasm/intel), ``""`` (gas)
 	#[getter]
 	fn octal_suffix(&self) -> &str {
 		self.formatter.options().octal_suffix()
 	}
 
 	#[setter]
-	fn set_octal_suffix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_octal_suffix_string(new_value);
+	fn set_octal_suffix(&mut self, value: String) {
+		self.formatter.options_mut().set_octal_suffix_string(value);
 	}
 
 	/// int: (``u8``) Size of a digit group, see also :class:`Formatter.digit_separator`
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``0``      ``12345670``
-	/// 👍          ``4``      ``1234_5670``
+	/// ✔️          ``4``      ``1234_5670``
 	/// =========== ========== ================================================
 	#[getter]
 	fn octal_digit_group_size(&self) -> u32 {
 		self.formatter.options().octal_digit_group_size()
 	}
 
 	#[setter]
-	fn set_octal_digit_group_size(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_octal_digit_group_size(new_value);
+	fn set_octal_digit_group_size(&mut self, value: u32) {
+		self.formatter.options_mut().set_octal_digit_group_size(value);
 	}
 
 	/// str: Binary number prefix or an empty string
 	///
 	/// Default: ``""`` (masm/nasm/intel), ``"0b"`` (gas)
 	#[getter]
 	fn binary_prefix(&self) -> &str {
 		self.formatter.options().binary_prefix()
 	}
 
 	#[setter]
-	fn set_binary_prefix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_binary_prefix_string(new_value);
+	fn set_binary_prefix(&mut self, value: String) {
+		self.formatter.options_mut().set_binary_prefix_string(value);
 	}
 
 	/// str: Binary number suffix or an empty string
 	///
 	/// Default: ``"b"`` (masm/nasm/intel), ``""`` (gas)
 	#[getter]
 	fn binary_suffix(&self) -> &str {
 		self.formatter.options().binary_suffix()
 	}
 
 	#[setter]
-	fn set_binary_suffix(&mut self, new_value: String) {
-		self.formatter.options_mut().set_binary_suffix_string(new_value);
+	fn set_binary_suffix(&mut self, value: String) {
+		self.formatter.options_mut().set_binary_suffix_string(value);
 	}
 
 	/// int: (``u8``) Size of a digit group, see also :class:`Formatter.digit_separator`
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``0``      ``11010111``
-	/// 👍          ``4``      ``1101_0111``
+	/// ✔️          ``4``      ``1101_0111``
 	/// =========== ========== ================================================
 	#[getter]
 	fn binary_digit_group_size(&self) -> u32 {
 		self.formatter.options().binary_digit_group_size()
 	}
 
 	#[setter]
-	fn set_binary_digit_group_size(&mut self, new_value: u32) {
-		self.formatter.options_mut().set_binary_digit_group_size(new_value);
+	fn set_binary_digit_group_size(&mut self, value: u32) {
+		self.formatter.options_mut().set_binary_digit_group_size(value);
 	}
 
 	/// str: Digit separator or an empty string. See also eg. :class:`Formatter.hex_digit_group_size`
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``""``     ``0x12345678``
+	/// ✔️          ``""``     ``0x12345678``
 	/// \           ``"_"``    ``0x1234_5678``
 	/// =========== ========== ================================================
 	#[getter]
 	fn digit_separator(&self) -> &str {
 		self.formatter.options().digit_separator()
 	}
 
 	#[setter]
-	fn set_digit_separator(&mut self, new_value: String) {
-		self.formatter.options_mut().set_digit_separator_string(new_value);
+	fn set_digit_separator(&mut self, value: String) {
+		self.formatter.options_mut().set_digit_separator_string(value);
 	}
 
-	/// bool: Add leading zeros to hexadecimal/octal/binary numbers.
+	/// bool: Add leading zeroes to hexadecimal/octal/binary numbers.
 	///
-	/// This option has no effect on branch targets and displacements, use :class:`Formatter.branch_leading_zeros`
-	/// and :class:`Formatter.displacement_leading_zeros`.
+	/// This option has no effect on branch targets and displacements, use :class:`Formatter.branch_leading_zeroes`
+	/// and :class:`Formatter.displacement_leading_zeroes`.
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``0x0000000A``/``0000000Ah``
-	/// 👍          ``False``   ``0xA``/``0Ah``
+	/// ✔️          ``False``   ``0xA``/``0Ah``
 	/// =========== ========== ================================================
 	#[getter]
-	fn leading_zeros(&self) -> bool {
-		self.formatter.options().leading_zeros()
+	fn leading_zeroes(&self) -> bool {
+		self.formatter.options().leading_zeroes()
 	}
 
 	#[setter]
-	fn set_leading_zeros(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_leading_zeros(new_value);
+	fn set_leading_zeroes(&mut self, value: bool) {
+		self.formatter.options_mut().set_leading_zeroes(value);
 	}
 
-	/// bool: Use uppercase hex digits
+	/// bool: Use upper case hex digits
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``0xFF``
+	/// ✔️          ``True``   ``0xFF``
 	/// \           ``False``   ``0xff``
 	/// =========== ========== ================================================
 	#[getter]
 	fn uppercase_hex(&self) -> bool {
 		self.formatter.options().uppercase_hex()
 	}
 
 	#[setter]
-	fn set_uppercase_hex(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_uppercase_hex(new_value);
+	fn set_uppercase_hex(&mut self, value: bool) {
+		self.formatter.options_mut().set_uppercase_hex(value);
 	}
 
 	/// bool: Small hex numbers (-9 .. 9) are shown in decimal
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``9``
+	/// ✔️          ``True``   ``9``
 	/// \           ``False``   ``0x9``
 	/// =========== ========== ================================================
 	#[getter]
 	fn small_hex_numbers_in_decimal(&self) -> bool {
 		self.formatter.options().small_hex_numbers_in_decimal()
 	}
 
 	#[setter]
-	fn set_small_hex_numbers_in_decimal(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_small_hex_numbers_in_decimal(new_value);
+	fn set_small_hex_numbers_in_decimal(&mut self, value: bool) {
+		self.formatter.options_mut().set_small_hex_numbers_in_decimal(value);
 	}
 
 	/// bool: Add a leading zero to hex numbers if there's no prefix and the number starts with hex digits ``A-F``
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``0FFh``
+	/// ✔️          ``True``   ``0FFh``
 	/// \           ``False``   ``FFh``
 	/// =========== ========== ================================================
 	#[getter]
 	fn add_leading_zero_to_hex_numbers(&self) -> bool {
 		self.formatter.options().add_leading_zero_to_hex_numbers()
 	}
 
 	#[setter]
-	fn set_add_leading_zero_to_hex_numbers(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_add_leading_zero_to_hex_numbers(new_value);
+	fn set_add_leading_zero_to_hex_numbers(&mut self, value: bool) {
+		self.formatter.options_mut().set_add_leading_zero_to_hex_numbers(value);
 	}
 
 	/// int: Number base (``2``, ``8``, ``10``, ``16``)
 	///
 	/// Raises:
 	///     ValueError: If it's an invalid number base
 	///
@@ -896,509 +916,509 @@
 			iced_x86::NumberBase::Octal => 8,
 			iced_x86::NumberBase::Decimal => 10,
 			iced_x86::NumberBase::Hexadecimal => 16,
 		}
 	}
 
 	#[setter]
-	fn set_number_base(&mut self, new_value: u32) -> PyResult<()> {
-		let base = match new_value {
+	fn set_number_base(&mut self, value: u32) -> PyResult<()> {
+		let base = match value {
 			2 => iced_x86::NumberBase::Binary,
 			8 => iced_x86::NumberBase::Octal,
 			10 => iced_x86::NumberBase::Decimal,
 			16 => iced_x86::NumberBase::Hexadecimal,
 			_ => return Err(PyValueError::new_err("Invalid number base")),
 		};
 		self.formatter.options_mut().set_number_base(base);
 		Ok(())
 	}
 
-	/// bool: Add leading zeros to branch offsets. Used by ``CALL NEAR``, ``CALL FAR``, ``JMP NEAR``, ``JMP FAR``, ``Jcc``, ``LOOP``, ``LOOPcc``, ``XBEGIN``
+	/// bool: Add leading zeroes to branch offsets. Used by ``CALL NEAR``, ``CALL FAR``, ``JMP NEAR``, ``JMP FAR``, ``Jcc``, ``LOOP``, ``LOOPcc``, ``XBEGIN``
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``je 00000123h``
+	/// ✔️          ``True``   ``je 00000123h``
 	/// \           ``False``   ``je 123h``
 	/// =========== ========== ================================================
 	#[getter]
-	fn branch_leading_zeros(&self) -> bool {
-		self.formatter.options().branch_leading_zeros()
+	fn branch_leading_zeroes(&self) -> bool {
+		self.formatter.options().branch_leading_zeroes()
 	}
 
 	#[setter]
-	fn set_branch_leading_zeros(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_branch_leading_zeros(new_value);
+	fn set_branch_leading_zeroes(&mut self, value: bool) {
+		self.formatter.options_mut().set_branch_leading_zeroes(value);
 	}
 
 	/// bool: Show immediate operands as signed numbers
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,-1``
-	/// 👍          ``False``   ``mov eax,FFFFFFFF``
+	/// ✔️          ``False``   ``mov eax,FFFFFFFF``
 	/// =========== ========== ================================================
 	#[getter]
 	fn signed_immediate_operands(&self) -> bool {
 		self.formatter.options().signed_immediate_operands()
 	}
 
 	#[setter]
-	fn set_signed_immediate_operands(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_signed_immediate_operands(new_value);
+	fn set_signed_immediate_operands(&mut self, value: bool) {
+		self.formatter.options_mut().set_signed_immediate_operands(value);
 	}
 
 	/// bool: Displacements are signed numbers
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``mov al,[eax-2000h]``
+	/// ✔️          ``True``   ``mov al,[eax-2000h]``
 	/// \           ``False``   ``mov al,[eax+0FFFFE000h]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn signed_memory_displacements(&self) -> bool {
 		self.formatter.options().signed_memory_displacements()
 	}
 
 	#[setter]
-	fn set_signed_memory_displacements(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_signed_memory_displacements(new_value);
+	fn set_signed_memory_displacements(&mut self, value: bool) {
+		self.formatter.options_mut().set_signed_memory_displacements(value);
 	}
 
-	/// bool: Add leading zeros to displacements
+	/// bool: Add leading zeroes to displacements
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov al,[eax+00000012h]``
-	/// 👍          ``False``   ``mov al,[eax+12h]``
+	/// ✔️          ``False``   ``mov al,[eax+12h]``
 	/// =========== ========== ================================================
 	#[getter]
-	fn displacement_leading_zeros(&self) -> bool {
-		self.formatter.options().displacement_leading_zeros()
+	fn displacement_leading_zeroes(&self) -> bool {
+		self.formatter.options().displacement_leading_zeroes()
 	}
 
 	#[setter]
-	fn set_displacement_leading_zeros(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_displacement_leading_zeros(new_value);
+	fn set_displacement_leading_zeroes(&mut self, value: bool) {
+		self.formatter.options_mut().set_displacement_leading_zeroes(value);
 	}
 
 	/// :class:`MemorySizeOptions`: Options that control if the memory size (eg. ``DWORD PTR``) is shown or not.
 	///
 	/// This is ignored by the gas (AT&T) formatter.
 	///
 	/// Default: :class:`MemorySizeOptions.DEFAULT`
 	#[getter]
 	fn memory_size_options(&self) -> u32 {
 		self.formatter.options().memory_size_options() as u32
 	}
 
 	#[setter]
-	fn set_memory_size_options(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_memory_size_options(to_memory_size_options(new_value)?);
+	fn set_memory_size_options(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_memory_size_options(to_memory_size_options(value)?);
 		Ok(())
 	}
 
 	/// bool: Show ``RIP+displ`` or the virtual address
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[rip+12345678h]``
-	/// 👍          ``False``   ``mov eax,[1029384756AFBECDh]``
+	/// ✔️          ``False``   ``mov eax,[1029384756AFBECDh]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn rip_relative_addresses(&self) -> bool {
 		self.formatter.options().rip_relative_addresses()
 	}
 
 	#[setter]
-	fn set_rip_relative_addresses(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_rip_relative_addresses(new_value);
+	fn set_rip_relative_addresses(&mut self, value: bool) {
+		self.formatter.options_mut().set_rip_relative_addresses(value);
 	}
 
 	/// bool: Show ``NEAR``, ``SHORT``, etc if it's a branch instruction
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``je short 1234h``
+	/// ✔️          ``True``   ``je short 1234h``
 	/// \           ``False``   ``je 1234h``
 	/// =========== ========== ================================================
 	#[getter]
 	fn show_branch_size(&self) -> bool {
 		self.formatter.options().show_branch_size()
 	}
 
 	#[setter]
-	fn set_show_branch_size(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_show_branch_size(new_value);
+	fn set_show_branch_size(&mut self, value: bool) {
+		self.formatter.options_mut().set_show_branch_size(value);
 	}
 
 	/// bool: Use pseudo instructions
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``vcmpnltsd xmm2,xmm6,xmm3``
+	/// ✔️          ``True``   ``vcmpnltsd xmm2,xmm6,xmm3``
 	/// \           ``False``   ``vcmpsd xmm2,xmm6,xmm3,5``
 	/// =========== ========== ================================================
 	#[getter]
 	fn use_pseudo_ops(&self) -> bool {
 		self.formatter.options().use_pseudo_ops()
 	}
 
 	#[setter]
-	fn set_use_pseudo_ops(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_use_pseudo_ops(new_value);
+	fn set_use_pseudo_ops(&mut self, value: bool) {
+		self.formatter.options_mut().set_use_pseudo_ops(value);
 	}
 
 	/// bool: Show the original value after the symbol name
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,[myfield (12345678)]``
-	/// 👍          ``False``   ``mov eax,[myfield]``
+	/// ✔️          ``False``   ``mov eax,[myfield]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn show_symbol_address(&self) -> bool {
 		self.formatter.options().show_symbol_address()
 	}
 
 	#[setter]
-	fn set_show_symbol_address(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_show_symbol_address(new_value);
+	fn set_show_symbol_address(&mut self, value: bool) {
+		self.formatter.options_mut().set_show_symbol_address(value);
 	}
 
 	/// bool: (gas only): If ``True``, the formatter doesn't add ``%`` to registers
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``mov eax,ecx``
-	/// 👍          ``False``   ``mov %eax,%ecx``
+	/// ✔️          ``False``   ``mov %eax,%ecx``
 	/// =========== ========== ================================================
 	#[getter]
 	fn gas_naked_registers(&self) -> bool {
 		self.formatter.options().gas_naked_registers()
 	}
 
 	#[setter]
-	fn set_gas_naked_registers(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_gas_naked_registers(new_value);
+	fn set_gas_naked_registers(&mut self, value: bool) {
+		self.formatter.options_mut().set_gas_naked_registers(value);
 	}
 
 	/// bool: (gas only): Shows the mnemonic size suffix even when not needed
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``movl %eax,%ecx``
-	/// 👍          ``False``   ``mov %eax,%ecx``
+	/// ✔️          ``False``   ``mov %eax,%ecx``
 	/// =========== ========== ================================================
 	#[getter]
 	fn gas_show_mnemonic_size_suffix(&self) -> bool {
 		self.formatter.options().gas_show_mnemonic_size_suffix()
 	}
 
 	#[setter]
-	fn set_gas_show_mnemonic_size_suffix(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_gas_show_mnemonic_size_suffix(new_value);
+	fn set_gas_show_mnemonic_size_suffix(&mut self, value: bool) {
+		self.formatter.options_mut().set_gas_show_mnemonic_size_suffix(value);
 	}
 
 	/// bool: (gas only): Add a space after the comma if it's a memory operand
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``(%eax, %ecx, 2)``
-	/// 👍          ``False``   ``(%eax,%ecx,2)``
+	/// ✔️          ``False``   ``(%eax,%ecx,2)``
 	/// =========== ========== ================================================
 	#[getter]
 	fn gas_space_after_memory_operand_comma(&self) -> bool {
 		self.formatter.options().gas_space_after_memory_operand_comma()
 	}
 
 	#[setter]
-	fn set_gas_space_after_memory_operand_comma(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_gas_space_after_memory_operand_comma(new_value);
+	fn set_gas_space_after_memory_operand_comma(&mut self, value: bool) {
+		self.formatter.options_mut().set_gas_space_after_memory_operand_comma(value);
 	}
 
 	/// bool: (masm only): Add a ``DS`` segment override even if it's not present. Used if it's 16/32-bit code and mem op is a displ
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``mov eax,ds:[12345678]``
+	/// ✔️          ``True``   ``mov eax,ds:[12345678]``
 	/// \           ``False``   ``mov eax,[12345678]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn masm_add_ds_prefix32(&self) -> bool {
 		self.formatter.options().masm_add_ds_prefix32()
 	}
 
 	#[setter]
-	fn set_masm_add_ds_prefix32(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_masm_add_ds_prefix32(new_value);
+	fn set_masm_add_ds_prefix32(&mut self, value: bool) {
+		self.formatter.options_mut().set_masm_add_ds_prefix32(value);
 	}
 
 	/// bool: (masm only): Show symbols in brackets
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``[ecx+symbol]`` / ``[symbol]``
+	/// ✔️          ``True``   ``[ecx+symbol]`` / ``[symbol]``
 	/// \           ``False``   ``symbol[ecx]`` / ``symbol``
 	/// =========== ========== ================================================
 	#[getter]
 	fn masm_symbol_displ_in_brackets(&self) -> bool {
 		self.formatter.options().masm_symbol_displ_in_brackets()
 	}
 
 	#[setter]
-	fn set_masm_symbol_displ_in_brackets(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_masm_symbol_displ_in_brackets(new_value);
+	fn set_masm_symbol_displ_in_brackets(&mut self, value: bool) {
+		self.formatter.options_mut().set_masm_symbol_displ_in_brackets(value);
 	}
 
 	/// bool: (masm only): Show displacements in brackets
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
-	/// 👍          ``True``   ``[ecx+1234h]``
+	/// ✔️          ``True``   ``[ecx+1234h]``
 	/// \           ``False``   ``1234h[ecx]``
 	/// =========== ========== ================================================
 	#[getter]
 	fn masm_displ_in_brackets(&self) -> bool {
 		self.formatter.options().masm_displ_in_brackets()
 	}
 
 	#[setter]
-	fn set_masm_displ_in_brackets(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_masm_displ_in_brackets(new_value);
+	fn set_masm_displ_in_brackets(&mut self, value: bool) {
+		self.formatter.options_mut().set_masm_displ_in_brackets(value);
 	}
 
 	/// bool: (nasm only): Shows ``BYTE``, ``WORD``, ``DWORD`` or ``QWORD`` if it's a sign extended immediate operand value
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``or rcx,byte -1``
-	/// 👍          ``False``   ``or rcx,-1``
+	/// ✔️          ``False``   ``or rcx,-1``
 	/// =========== ========== ================================================
 	#[getter]
 	fn nasm_show_sign_extended_immediate_size(&self) -> bool {
 		self.formatter.options().nasm_show_sign_extended_immediate_size()
 	}
 
 	#[setter]
-	fn set_nasm_show_sign_extended_immediate_size(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_nasm_show_sign_extended_immediate_size(new_value);
+	fn set_nasm_show_sign_extended_immediate_size(&mut self, value: bool) {
+		self.formatter.options_mut().set_nasm_show_sign_extended_immediate_size(value);
 	}
 
 	/// bool: Use ``st(0)`` instead of ``st`` if ``st`` can be used. Ignored by the nasm formatter.
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``fadd st(0),st(3)``
-	/// 👍          ``False``   ``fadd st,st(3)``
+	/// ✔️          ``False``   ``fadd st,st(3)``
 	/// =========== ========== ================================================
 	#[getter]
 	fn prefer_st0(&self) -> bool {
 		self.formatter.options().prefer_st0()
 	}
 
 	#[setter]
-	fn set_prefer_st0(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_prefer_st0(new_value);
+	fn set_prefer_st0(&mut self, value: bool) {
+		self.formatter.options_mut().set_prefer_st0(value);
 	}
 
 	/// bool: Show useless prefixes. If it has useless prefixes, it could be data and not code.
 	///
 	/// =========== ========== ================================================
 	/// Default     Value      Example
 	/// =========== ========== ================================================
 	/// \           ``True``   ``es rep add eax,ecx``
-	/// 👍          ``False``   ``add eax,ecx``
+	/// ✔️          ``False``   ``add eax,ecx``
 	/// =========== ========== ================================================
 	#[getter]
 	fn show_useless_prefixes(&self) -> bool {
 		self.formatter.options().show_useless_prefixes()
 	}
 
 	#[setter]
-	fn set_show_useless_prefixes(&mut self, new_value: bool) {
-		self.formatter.options_mut().set_show_useless_prefixes(new_value)
+	fn set_show_useless_prefixes(&mut self, value: bool) {
+		self.formatter.options_mut().set_show_useless_prefixes(value)
 	}
 
 	/// :class:`CC_b`: Mnemonic condition code selector (eg. ``JB`` / ``JC`` / ``JNAE``)
 	///
 	/// Default: ``JB``, ``CMOVB``, ``SETB``
 	#[getter]
 	fn cc_b(&self) -> u32 {
 		self.formatter.options().cc_b() as u32
 	}
 
 	#[setter]
-	fn set_cc_b(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_b(to_cc_b(new_value)?);
+	fn set_cc_b(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_b(to_cc_b(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_ae`: Mnemonic condition code selector (eg. ``JAE`` / ``JNB`` / ``JNC``)
 	///
 	/// Default: ``JAE``, ``CMOVAE``, ``SETAE``
 	#[getter]
 	fn cc_ae(&self) -> u32 {
 		self.formatter.options().cc_ae() as u32
 	}
 
 	#[setter]
-	fn set_cc_ae(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_ae(to_cc_ae(new_value)?);
+	fn set_cc_ae(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_ae(to_cc_ae(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_e`: Mnemonic condition code selector (eg. ``JE`` / ``JZ``)
 	///
 	/// Default: ``JE``, ``CMOVE``, ``SETE``, ``LOOPE``, ``REPE``
 	#[getter]
 	fn cc_e(&self) -> u32 {
 		self.formatter.options().cc_e() as u32
 	}
 
 	#[setter]
-	fn set_cc_e(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_e(to_cc_e(new_value)?);
+	fn set_cc_e(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_e(to_cc_e(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_ne`: Mnemonic condition code selector (eg. ``JNE`` / ``JNZ``)
 	///
 	/// Default: ``JNE``, ``CMOVNE``, ``SETNE``, ``LOOPNE``, ``REPNE``
 	#[getter]
 	fn cc_ne(&self) -> u32 {
 		self.formatter.options().cc_ne() as u32
 	}
 
 	#[setter]
-	fn set_cc_ne(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_ne(to_cc_ne(new_value)?);
+	fn set_cc_ne(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_ne(to_cc_ne(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_be`: Mnemonic condition code selector (eg. ``JBE`` / ``JNA``)
 	///
 	/// Default: ``JBE``, ``CMOVBE``, ``SETBE``
 	#[getter]
 	fn cc_be(&self) -> u32 {
 		self.formatter.options().cc_be() as u32
 	}
 
 	#[setter]
-	fn set_cc_be(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_be(to_cc_be(new_value)?);
+	fn set_cc_be(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_be(to_cc_be(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_a`: Mnemonic condition code selector (eg. ``JA`` / ``JNBE``)
 	///
 	/// Default: ``JA``, ``CMOVA``, ``SETA``
 	#[getter]
 	fn cc_a(&self) -> u32 {
 		self.formatter.options().cc_a() as u32
 	}
 
 	#[setter]
-	fn set_cc_a(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_a(to_cc_a(new_value)?);
+	fn set_cc_a(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_a(to_cc_a(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_p`: Mnemonic condition code selector (eg. ``JP`` / ``JPE``)
 	///
 	/// Default: ``JP``, ``CMOVP``, ``SETP``
 	#[getter]
 	fn cc_p(&self) -> u32 {
 		self.formatter.options().cc_p() as u32
 	}
 
 	#[setter]
-	fn set_cc_p(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_p(to_cc_p(new_value)?);
+	fn set_cc_p(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_p(to_cc_p(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_np`: Mnemonic condition code selector (eg. ``JNP`` / ``JPO``)
 	///
 	/// Default: ``JNP``, ``CMOVNP``, ``SETNP``
 	#[getter]
 	fn cc_np(&self) -> u32 {
 		self.formatter.options().cc_np() as u32
 	}
 
 	#[setter]
-	fn set_cc_np(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_np(to_cc_np(new_value)?);
+	fn set_cc_np(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_np(to_cc_np(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_l`: Mnemonic condition code selector (eg. ``JL`` / ``JNGE``)
 	///
 	/// Default: ``JL``, ``CMOVL``, ``SETL``
 	#[getter]
 	fn cc_l(&self) -> u32 {
 		self.formatter.options().cc_l() as u32
 	}
 
 	#[setter]
-	fn set_cc_l(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_l(to_cc_l(new_value)?);
+	fn set_cc_l(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_l(to_cc_l(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_ge`: Mnemonic condition code selector (eg. ``JGE`` / ``JNL``)
 	///
 	/// Default: ``JGE``, ``CMOVGE``, ``SETGE``
 	#[getter]
 	fn cc_ge(&self) -> u32 {
 		self.formatter.options().cc_ge() as u32
 	}
 
 	#[setter]
-	fn set_cc_ge(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_ge(to_cc_ge(new_value)?);
+	fn set_cc_ge(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_ge(to_cc_ge(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_le`: Mnemonic condition code selector (eg. ``JLE`` / ``JNG``)
 	///
 	/// Default: ``JLE``, ``CMOVLE``, ``SETLE``
 	#[getter]
 	fn cc_le(&self) -> u32 {
 		self.formatter.options().cc_le() as u32
 	}
 
 	#[setter]
-	fn set_cc_le(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_le(to_cc_le(new_value)?);
+	fn set_cc_le(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_le(to_cc_le(value)?);
 		Ok(())
 	}
 
 	/// :class:`CC_g`: Mnemonic condition code selector (eg. ``JG`` / ``JNLE``)
 	///
 	/// Default: ``JG``, ``CMOVG``, ``SETG``
 	#[getter]
 	fn cc_g(&self) -> u32 {
 		self.formatter.options().cc_g() as u32
 	}
 
 	#[setter]
-	fn set_cc_g(&mut self, new_value: u32) -> PyResult<()> {
-		self.formatter.options_mut().set_cc_g(to_cc_g(new_value)?);
+	fn set_cc_g(&mut self, value: u32) -> PyResult<()> {
+		self.formatter.options_mut().set_cc_g(to_cc_g(value)?);
 		Ok(())
 	}
 }
```

### Comparing `iced-x86-1.19.0/src/iced_x86/Code.py` & `iced-x86-1.9.1/src/iced_x86/Code.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49113 +1,43187 @@
-# SPDX-License-Identifier: MIT
-# Copyright (C) 2018-present iced project and contributors
+#
+# Copyright (C) 2018-2019 de4dot@gmail.com
+#
+# Permission is hereby granted, free of charge, to any person obtaining
+# a copy of this software and associated documentation files (the
+# "Software"), to deal in the Software without restriction, including
+# without limitation the rights to use, copy, modify, merge, publish,
+# distribute, sublicense, and/or sell copies of the Software, and to
+# permit persons to whom the Software is furnished to do so, subject to
+# the following conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+#
 
 # ⚠️This file was generated by GENERATOR!🦹‍♂️
 
 # pylint: disable=invalid-name
 # pylint: disable=line-too-long
 # pylint: disable=too-many-lines
 
 """
 x86 instruction code
 """
 
-import typing
-if typing.TYPE_CHECKING:
-	from ._iced_x86_py import Code
-else:
-	Code = int
+from typing import List
 
-INVALID: Code = 0 # type: ignore
+INVALID: int = 0
 """
 It's an invalid instruction, eg. it's a new unknown instruction, garbage or there's not enough bytes to decode the instruction etc.
 """
-DECLAREBYTE: Code = 1 # type: ignore
+DECLAREBYTE: int = 1
 """
 A ``db``/``.byte`` asm directive that can store 1-16 bytes
 """
-DECLAREWORD: Code = 2 # type: ignore
+DECLAREWORD: int = 2
 """
 A ``dw``/``.word`` asm directive that can store 1-8 words
 """
-DECLAREDWORD: Code = 3 # type: ignore
+DECLAREDWORD: int = 3
 """
 A ``dd``/``.int`` asm directive that can store 1-4 dwords
 """
-DECLAREQWORD: Code = 4 # type: ignore
+DECLAREQWORD: int = 4
 """
 A ``dq``/``.quad`` asm directive that can store 1-2 qwords
 """
-ADD_RM8_R8: Code = 5 # type: ignore
+ADD_RM8_R8: int = 5
 """
 ``ADD r/m8, r8``
 
 ``00 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_RM16_R16: Code = 6 # type: ignore
+ADD_RM16_R16: int = 6
 """
 ``ADD r/m16, r16``
 
 ``o16 01 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_RM32_R32: Code = 7 # type: ignore
+ADD_RM32_R32: int = 7
 """
 ``ADD r/m32, r32``
 
 ``o32 01 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADD_RM64_R64: Code = 8 # type: ignore
+ADD_RM64_R64: int = 8
 """
 ``ADD r/m64, r64``
 
 ``o64 01 /r``
 
 ``X64``
 
 ``64-bit``
 """
-ADD_R8_RM8: Code = 9 # type: ignore
+ADD_R8_RM8: int = 9
 """
 ``ADD r8, r/m8``
 
 ``02 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_R16_RM16: Code = 10 # type: ignore
+ADD_R16_RM16: int = 10
 """
 ``ADD r16, r/m16``
 
 ``o16 03 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_R32_RM32: Code = 11 # type: ignore
+ADD_R32_RM32: int = 11
 """
 ``ADD r32, r/m32``
 
 ``o32 03 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADD_R64_RM64: Code = 12 # type: ignore
+ADD_R64_RM64: int = 12
 """
 ``ADD r64, r/m64``
 
 ``o64 03 /r``
 
 ``X64``
 
 ``64-bit``
 """
-ADD_AL_IMM8: Code = 13 # type: ignore
+ADD_AL_IMM8: int = 13
 """
 ``ADD AL, imm8``
 
 ``04 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_AX_IMM16: Code = 14 # type: ignore
+ADD_AX_IMM16: int = 14
 """
 ``ADD AX, imm16``
 
 ``o16 05 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_EAX_IMM32: Code = 15 # type: ignore
+ADD_EAX_IMM32: int = 15
 """
 ``ADD EAX, imm32``
 
 ``o32 05 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADD_RAX_IMM32: Code = 16 # type: ignore
+ADD_RAX_IMM32: int = 16
 """
 ``ADD RAX, imm32``
 
 ``o64 05 id``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHW_ES: Code = 17 # type: ignore
+PUSHW_ES: int = 17
 """
 ``PUSH ES``
 
 ``o16 06``
 
 ``8086+``
 
 ``16/32-bit``
 """
-PUSHD_ES: Code = 18 # type: ignore
+PUSHD_ES: int = 18
 """
 ``PUSH ES``
 
 ``o32 06``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPW_ES: Code = 19 # type: ignore
+POPW_ES: int = 19
 """
 ``POP ES``
 
 ``o16 07``
 
 ``8086+``
 
 ``16/32-bit``
 """
-POPD_ES: Code = 20 # type: ignore
+POPD_ES: int = 20
 """
 ``POP ES``
 
 ``o32 07``
 
 ``386+``
 
 ``16/32-bit``
 """
-OR_RM8_R8: Code = 21 # type: ignore
+OR_RM8_R8: int = 21
 """
 ``OR r/m8, r8``
 
 ``08 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_RM16_R16: Code = 22 # type: ignore
+OR_RM16_R16: int = 22
 """
 ``OR r/m16, r16``
 
 ``o16 09 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_RM32_R32: Code = 23 # type: ignore
+OR_RM32_R32: int = 23
 """
 ``OR r/m32, r32``
 
 ``o32 09 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OR_RM64_R64: Code = 24 # type: ignore
+OR_RM64_R64: int = 24
 """
 ``OR r/m64, r64``
 
 ``o64 09 /r``
 
 ``X64``
 
 ``64-bit``
 """
-OR_R8_RM8: Code = 25 # type: ignore
+OR_R8_RM8: int = 25
 """
 ``OR r8, r/m8``
 
 ``0A /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_R16_RM16: Code = 26 # type: ignore
+OR_R16_RM16: int = 26
 """
 ``OR r16, r/m16``
 
 ``o16 0B /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_R32_RM32: Code = 27 # type: ignore
+OR_R32_RM32: int = 27
 """
 ``OR r32, r/m32``
 
 ``o32 0B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OR_R64_RM64: Code = 28 # type: ignore
+OR_R64_RM64: int = 28
 """
 ``OR r64, r/m64``
 
 ``o64 0B /r``
 
 ``X64``
 
 ``64-bit``
 """
-OR_AL_IMM8: Code = 29 # type: ignore
+OR_AL_IMM8: int = 29
 """
 ``OR AL, imm8``
 
 ``0C ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_AX_IMM16: Code = 30 # type: ignore
+OR_AX_IMM16: int = 30
 """
 ``OR AX, imm16``
 
 ``o16 0D iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_EAX_IMM32: Code = 31 # type: ignore
+OR_EAX_IMM32: int = 31
 """
 ``OR EAX, imm32``
 
 ``o32 0D id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OR_RAX_IMM32: Code = 32 # type: ignore
+OR_RAX_IMM32: int = 32
 """
 ``OR RAX, imm32``
 
 ``o64 0D id``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHW_CS: Code = 33 # type: ignore
+PUSHW_CS: int = 33
 """
 ``PUSH CS``
 
 ``o16 0E``
 
 ``8086+``
 
 ``16/32-bit``
 """
-PUSHD_CS: Code = 34 # type: ignore
+PUSHD_CS: int = 34
 """
 ``PUSH CS``
 
 ``o32 0E``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPW_CS: Code = 35 # type: ignore
+POPW_CS: int = 35
 """
 ``POP CS``
 
 ``o16 0F``
 
 ``8086``
 
 ``16-bit``
 """
-ADC_RM8_R8: Code = 36 # type: ignore
+ADC_RM8_R8: int = 36
 """
 ``ADC r/m8, r8``
 
 ``10 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_RM16_R16: Code = 37 # type: ignore
+ADC_RM16_R16: int = 37
 """
 ``ADC r/m16, r16``
 
 ``o16 11 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_RM32_R32: Code = 38 # type: ignore
+ADC_RM32_R32: int = 38
 """
 ``ADC r/m32, r32``
 
 ``o32 11 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADC_RM64_R64: Code = 39 # type: ignore
+ADC_RM64_R64: int = 39
 """
 ``ADC r/m64, r64``
 
 ``o64 11 /r``
 
 ``X64``
 
 ``64-bit``
 """
-ADC_R8_RM8: Code = 40 # type: ignore
+ADC_R8_RM8: int = 40
 """
 ``ADC r8, r/m8``
 
 ``12 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_R16_RM16: Code = 41 # type: ignore
+ADC_R16_RM16: int = 41
 """
 ``ADC r16, r/m16``
 
 ``o16 13 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_R32_RM32: Code = 42 # type: ignore
+ADC_R32_RM32: int = 42
 """
 ``ADC r32, r/m32``
 
 ``o32 13 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADC_R64_RM64: Code = 43 # type: ignore
+ADC_R64_RM64: int = 43
 """
 ``ADC r64, r/m64``
 
 ``o64 13 /r``
 
 ``X64``
 
 ``64-bit``
 """
-ADC_AL_IMM8: Code = 44 # type: ignore
+ADC_AL_IMM8: int = 44
 """
 ``ADC AL, imm8``
 
 ``14 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_AX_IMM16: Code = 45 # type: ignore
+ADC_AX_IMM16: int = 45
 """
 ``ADC AX, imm16``
 
 ``o16 15 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_EAX_IMM32: Code = 46 # type: ignore
+ADC_EAX_IMM32: int = 46
 """
 ``ADC EAX, imm32``
 
 ``o32 15 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADC_RAX_IMM32: Code = 47 # type: ignore
+ADC_RAX_IMM32: int = 47
 """
 ``ADC RAX, imm32``
 
 ``o64 15 id``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHW_SS: Code = 48 # type: ignore
+PUSHW_SS: int = 48
 """
 ``PUSH SS``
 
 ``o16 16``
 
 ``8086+``
 
 ``16/32-bit``
 """
-PUSHD_SS: Code = 49 # type: ignore
+PUSHD_SS: int = 49
 """
 ``PUSH SS``
 
 ``o32 16``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPW_SS: Code = 50 # type: ignore
+POPW_SS: int = 50
 """
 ``POP SS``
 
 ``o16 17``
 
 ``8086+``
 
 ``16/32-bit``
 """
-POPD_SS: Code = 51 # type: ignore
+POPD_SS: int = 51
 """
 ``POP SS``
 
 ``o32 17``
 
 ``386+``
 
 ``16/32-bit``
 """
-SBB_RM8_R8: Code = 52 # type: ignore
+SBB_RM8_R8: int = 52
 """
 ``SBB r/m8, r8``
 
 ``18 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_RM16_R16: Code = 53 # type: ignore
+SBB_RM16_R16: int = 53
 """
 ``SBB r/m16, r16``
 
 ``o16 19 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_RM32_R32: Code = 54 # type: ignore
+SBB_RM32_R32: int = 54
 """
 ``SBB r/m32, r32``
 
 ``o32 19 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SBB_RM64_R64: Code = 55 # type: ignore
+SBB_RM64_R64: int = 55
 """
 ``SBB r/m64, r64``
 
 ``o64 19 /r``
 
 ``X64``
 
 ``64-bit``
 """
-SBB_R8_RM8: Code = 56 # type: ignore
+SBB_R8_RM8: int = 56
 """
 ``SBB r8, r/m8``
 
 ``1A /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_R16_RM16: Code = 57 # type: ignore
+SBB_R16_RM16: int = 57
 """
 ``SBB r16, r/m16``
 
 ``o16 1B /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_R32_RM32: Code = 58 # type: ignore
+SBB_R32_RM32: int = 58
 """
 ``SBB r32, r/m32``
 
 ``o32 1B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SBB_R64_RM64: Code = 59 # type: ignore
+SBB_R64_RM64: int = 59
 """
 ``SBB r64, r/m64``
 
 ``o64 1B /r``
 
 ``X64``
 
 ``64-bit``
 """
-SBB_AL_IMM8: Code = 60 # type: ignore
+SBB_AL_IMM8: int = 60
 """
 ``SBB AL, imm8``
 
 ``1C ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_AX_IMM16: Code = 61 # type: ignore
+SBB_AX_IMM16: int = 61
 """
 ``SBB AX, imm16``
 
 ``o16 1D iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_EAX_IMM32: Code = 62 # type: ignore
+SBB_EAX_IMM32: int = 62
 """
 ``SBB EAX, imm32``
 
 ``o32 1D id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SBB_RAX_IMM32: Code = 63 # type: ignore
+SBB_RAX_IMM32: int = 63
 """
 ``SBB RAX, imm32``
 
 ``o64 1D id``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHW_DS: Code = 64 # type: ignore
+PUSHW_DS: int = 64
 """
 ``PUSH DS``
 
 ``o16 1E``
 
 ``8086+``
 
 ``16/32-bit``
 """
-PUSHD_DS: Code = 65 # type: ignore
+PUSHD_DS: int = 65
 """
 ``PUSH DS``
 
 ``o32 1E``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPW_DS: Code = 66 # type: ignore
+POPW_DS: int = 66
 """
 ``POP DS``
 
 ``o16 1F``
 
 ``8086+``
 
 ``16/32-bit``
 """
-POPD_DS: Code = 67 # type: ignore
+POPD_DS: int = 67
 """
 ``POP DS``
 
 ``o32 1F``
 
 ``386+``
 
 ``16/32-bit``
 """
-AND_RM8_R8: Code = 68 # type: ignore
+AND_RM8_R8: int = 68
 """
 ``AND r/m8, r8``
 
 ``20 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_RM16_R16: Code = 69 # type: ignore
+AND_RM16_R16: int = 69
 """
 ``AND r/m16, r16``
 
 ``o16 21 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_RM32_R32: Code = 70 # type: ignore
+AND_RM32_R32: int = 70
 """
 ``AND r/m32, r32``
 
 ``o32 21 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-AND_RM64_R64: Code = 71 # type: ignore
+AND_RM64_R64: int = 71
 """
 ``AND r/m64, r64``
 
 ``o64 21 /r``
 
 ``X64``
 
 ``64-bit``
 """
-AND_R8_RM8: Code = 72 # type: ignore
+AND_R8_RM8: int = 72
 """
 ``AND r8, r/m8``
 
 ``22 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_R16_RM16: Code = 73 # type: ignore
+AND_R16_RM16: int = 73
 """
 ``AND r16, r/m16``
 
 ``o16 23 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_R32_RM32: Code = 74 # type: ignore
+AND_R32_RM32: int = 74
 """
 ``AND r32, r/m32``
 
 ``o32 23 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-AND_R64_RM64: Code = 75 # type: ignore
+AND_R64_RM64: int = 75
 """
 ``AND r64, r/m64``
 
 ``o64 23 /r``
 
 ``X64``
 
 ``64-bit``
 """
-AND_AL_IMM8: Code = 76 # type: ignore
+AND_AL_IMM8: int = 76
 """
 ``AND AL, imm8``
 
 ``24 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_AX_IMM16: Code = 77 # type: ignore
+AND_AX_IMM16: int = 77
 """
 ``AND AX, imm16``
 
 ``o16 25 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_EAX_IMM32: Code = 78 # type: ignore
+AND_EAX_IMM32: int = 78
 """
 ``AND EAX, imm32``
 
 ``o32 25 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-AND_RAX_IMM32: Code = 79 # type: ignore
+AND_RAX_IMM32: int = 79
 """
 ``AND RAX, imm32``
 
 ``o64 25 id``
 
 ``X64``
 
 ``64-bit``
 """
-DAA: Code = 80 # type: ignore
+DAA: int = 80
 """
 ``DAA``
 
 ``27``
 
 ``8086+``
 
 ``16/32-bit``
 """
-SUB_RM8_R8: Code = 81 # type: ignore
+SUB_RM8_R8: int = 81
 """
 ``SUB r/m8, r8``
 
 ``28 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_RM16_R16: Code = 82 # type: ignore
+SUB_RM16_R16: int = 82
 """
 ``SUB r/m16, r16``
 
 ``o16 29 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_RM32_R32: Code = 83 # type: ignore
+SUB_RM32_R32: int = 83
 """
 ``SUB r/m32, r32``
 
 ``o32 29 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SUB_RM64_R64: Code = 84 # type: ignore
+SUB_RM64_R64: int = 84
 """
 ``SUB r/m64, r64``
 
 ``o64 29 /r``
 
 ``X64``
 
 ``64-bit``
 """
-SUB_R8_RM8: Code = 85 # type: ignore
+SUB_R8_RM8: int = 85
 """
 ``SUB r8, r/m8``
 
 ``2A /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_R16_RM16: Code = 86 # type: ignore
+SUB_R16_RM16: int = 86
 """
 ``SUB r16, r/m16``
 
 ``o16 2B /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_R32_RM32: Code = 87 # type: ignore
+SUB_R32_RM32: int = 87
 """
 ``SUB r32, r/m32``
 
 ``o32 2B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SUB_R64_RM64: Code = 88 # type: ignore
+SUB_R64_RM64: int = 88
 """
 ``SUB r64, r/m64``
 
 ``o64 2B /r``
 
 ``X64``
 
 ``64-bit``
 """
-SUB_AL_IMM8: Code = 89 # type: ignore
+SUB_AL_IMM8: int = 89
 """
 ``SUB AL, imm8``
 
 ``2C ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_AX_IMM16: Code = 90 # type: ignore
+SUB_AX_IMM16: int = 90
 """
 ``SUB AX, imm16``
 
 ``o16 2D iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_EAX_IMM32: Code = 91 # type: ignore
+SUB_EAX_IMM32: int = 91
 """
 ``SUB EAX, imm32``
 
 ``o32 2D id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SUB_RAX_IMM32: Code = 92 # type: ignore
+SUB_RAX_IMM32: int = 92
 """
 ``SUB RAX, imm32``
 
 ``o64 2D id``
 
 ``X64``
 
 ``64-bit``
 """
-DAS: Code = 93 # type: ignore
+DAS: int = 93
 """
 ``DAS``
 
 ``2F``
 
 ``8086+``
 
 ``16/32-bit``
 """
-XOR_RM8_R8: Code = 94 # type: ignore
+XOR_RM8_R8: int = 94
 """
 ``XOR r/m8, r8``
 
 ``30 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_RM16_R16: Code = 95 # type: ignore
+XOR_RM16_R16: int = 95
 """
 ``XOR r/m16, r16``
 
 ``o16 31 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_RM32_R32: Code = 96 # type: ignore
+XOR_RM32_R32: int = 96
 """
 ``XOR r/m32, r32``
 
 ``o32 31 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XOR_RM64_R64: Code = 97 # type: ignore
+XOR_RM64_R64: int = 97
 """
 ``XOR r/m64, r64``
 
 ``o64 31 /r``
 
 ``X64``
 
 ``64-bit``
 """
-XOR_R8_RM8: Code = 98 # type: ignore
+XOR_R8_RM8: int = 98
 """
 ``XOR r8, r/m8``
 
 ``32 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_R16_RM16: Code = 99 # type: ignore
+XOR_R16_RM16: int = 99
 """
 ``XOR r16, r/m16``
 
 ``o16 33 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_R32_RM32: Code = 100 # type: ignore
+XOR_R32_RM32: int = 100
 """
 ``XOR r32, r/m32``
 
 ``o32 33 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XOR_R64_RM64: Code = 101 # type: ignore
+XOR_R64_RM64: int = 101
 """
 ``XOR r64, r/m64``
 
 ``o64 33 /r``
 
 ``X64``
 
 ``64-bit``
 """
-XOR_AL_IMM8: Code = 102 # type: ignore
+XOR_AL_IMM8: int = 102
 """
 ``XOR AL, imm8``
 
 ``34 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_AX_IMM16: Code = 103 # type: ignore
+XOR_AX_IMM16: int = 103
 """
 ``XOR AX, imm16``
 
 ``o16 35 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_EAX_IMM32: Code = 104 # type: ignore
+XOR_EAX_IMM32: int = 104
 """
 ``XOR EAX, imm32``
 
 ``o32 35 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XOR_RAX_IMM32: Code = 105 # type: ignore
+XOR_RAX_IMM32: int = 105
 """
 ``XOR RAX, imm32``
 
 ``o64 35 id``
 
 ``X64``
 
 ``64-bit``
 """
-AAA: Code = 106 # type: ignore
+AAA: int = 106
 """
 ``AAA``
 
 ``37``
 
 ``8086+``
 
 ``16/32-bit``
 """
-CMP_RM8_R8: Code = 107 # type: ignore
+CMP_RM8_R8: int = 107
 """
 ``CMP r/m8, r8``
 
 ``38 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_RM16_R16: Code = 108 # type: ignore
+CMP_RM16_R16: int = 108
 """
 ``CMP r/m16, r16``
 
 ``o16 39 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_RM32_R32: Code = 109 # type: ignore
+CMP_RM32_R32: int = 109
 """
 ``CMP r/m32, r32``
 
 ``o32 39 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMP_RM64_R64: Code = 110 # type: ignore
+CMP_RM64_R64: int = 110
 """
 ``CMP r/m64, r64``
 
 ``o64 39 /r``
 
 ``X64``
 
 ``64-bit``
 """
-CMP_R8_RM8: Code = 111 # type: ignore
+CMP_R8_RM8: int = 111
 """
 ``CMP r8, r/m8``
 
 ``3A /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_R16_RM16: Code = 112 # type: ignore
+CMP_R16_RM16: int = 112
 """
 ``CMP r16, r/m16``
 
 ``o16 3B /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_R32_RM32: Code = 113 # type: ignore
+CMP_R32_RM32: int = 113
 """
 ``CMP r32, r/m32``
 
 ``o32 3B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMP_R64_RM64: Code = 114 # type: ignore
+CMP_R64_RM64: int = 114
 """
 ``CMP r64, r/m64``
 
 ``o64 3B /r``
 
 ``X64``
 
 ``64-bit``
 """
-CMP_AL_IMM8: Code = 115 # type: ignore
+CMP_AL_IMM8: int = 115
 """
 ``CMP AL, imm8``
 
 ``3C ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_AX_IMM16: Code = 116 # type: ignore
+CMP_AX_IMM16: int = 116
 """
 ``CMP AX, imm16``
 
 ``o16 3D iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_EAX_IMM32: Code = 117 # type: ignore
+CMP_EAX_IMM32: int = 117
 """
 ``CMP EAX, imm32``
 
 ``o32 3D id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMP_RAX_IMM32: Code = 118 # type: ignore
+CMP_RAX_IMM32: int = 118
 """
 ``CMP RAX, imm32``
 
 ``o64 3D id``
 
 ``X64``
 
 ``64-bit``
 """
-AAS: Code = 119 # type: ignore
+AAS: int = 119
 """
 ``AAS``
 
 ``3F``
 
 ``8086+``
 
 ``16/32-bit``
 """
-INC_R16: Code = 120 # type: ignore
+INC_R16: int = 120
 """
 ``INC r16``
 
 ``o16 40+rw``
 
 ``8086+``
 
 ``16/32-bit``
 """
-INC_R32: Code = 121 # type: ignore
+INC_R32: int = 121
 """
 ``INC r32``
 
 ``o32 40+rd``
 
 ``386+``
 
 ``16/32-bit``
 """
-DEC_R16: Code = 122 # type: ignore
+DEC_R16: int = 122
 """
 ``DEC r16``
 
 ``o16 48+rw``
 
 ``8086+``
 
 ``16/32-bit``
 """
-DEC_R32: Code = 123 # type: ignore
+DEC_R32: int = 123
 """
 ``DEC r32``
 
 ``o32 48+rd``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSH_R16: Code = 124 # type: ignore
+PUSH_R16: int = 124
 """
 ``PUSH r16``
 
 ``o16 50+rw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-PUSH_R32: Code = 125 # type: ignore
+PUSH_R32: int = 125
 """
 ``PUSH r32``
 
 ``o32 50+rd``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSH_R64: Code = 126 # type: ignore
+PUSH_R64: int = 126
 """
 ``PUSH r64``
 
 ``o64 50+ro``
 
 ``X64``
 
 ``64-bit``
 """
-POP_R16: Code = 127 # type: ignore
+POP_R16: int = 127
 """
 ``POP r16``
 
 ``o16 58+rw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-POP_R32: Code = 128 # type: ignore
+POP_R32: int = 128
 """
 ``POP r32``
 
 ``o32 58+rd``
 
 ``386+``
 
 ``16/32-bit``
 """
-POP_R64: Code = 129 # type: ignore
+POP_R64: int = 129
 """
 ``POP r64``
 
 ``o64 58+ro``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHAW: Code = 130 # type: ignore
+PUSHAW: int = 130
 """
 ``PUSHA``
 
 ``o16 60``
 
 ``186+``
 
 ``16/32-bit``
 """
-PUSHAD: Code = 131 # type: ignore
+PUSHAD: int = 131
 """
 ``PUSHAD``
 
 ``o32 60``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPAW: Code = 132 # type: ignore
+POPAW: int = 132
 """
 ``POPA``
 
 ``o16 61``
 
 ``186+``
 
 ``16/32-bit``
 """
-POPAD: Code = 133 # type: ignore
+POPAD: int = 133
 """
 ``POPAD``
 
 ``o32 61``
 
 ``386+``
 
 ``16/32-bit``
 """
-BOUND_R16_M1616: Code = 134 # type: ignore
+BOUND_R16_M1616: int = 134
 """
 ``BOUND r16, m16&16``
 
 ``o16 62 /r``
 
 ``186+``
 
 ``16/32-bit``
 """
-BOUND_R32_M3232: Code = 135 # type: ignore
+BOUND_R32_M3232: int = 135
 """
 ``BOUND r32, m32&32``
 
 ``o32 62 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-ARPL_RM16_R16: Code = 136 # type: ignore
+ARPL_RM16_R16: int = 136
 """
 ``ARPL r/m16, r16``
 
 ``o16 63 /r``
 
 ``286+``
 
 ``16/32-bit``
 """
-ARPL_R32M16_R32: Code = 137 # type: ignore
+ARPL_R32M16_R32: int = 137
 """
 ``ARPL r32/m16, r32``
 
 ``o32 63 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOVSXD_R16_RM16: Code = 138 # type: ignore
+MOVSXD_R16_RM16: int = 138
 """
 ``MOVSXD r16, r/m16``
 
 ``o16 63 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOVSXD_R32_RM32: Code = 139 # type: ignore
+MOVSXD_R32_RM32: int = 139
 """
 ``MOVSXD r32, r/m32``
 
 ``o32 63 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOVSXD_R64_RM32: Code = 140 # type: ignore
+MOVSXD_R64_RM32: int = 140
 """
 ``MOVSXD r64, r/m32``
 
 ``o64 63 /r``
 
 ``X64``
 
 ``64-bit``
 """
-PUSH_IMM16: Code = 141 # type: ignore
+PUSH_IMM16: int = 141
 """
 ``PUSH imm16``
 
 ``o16 68 iw``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-PUSHD_IMM32: Code = 142 # type: ignore
+PUSHD_IMM32: int = 142
 """
 ``PUSH imm32``
 
 ``o32 68 id``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSHQ_IMM32: Code = 143 # type: ignore
+PUSHQ_IMM32: int = 143
 """
 ``PUSH imm32``
 
 ``o64 68 id``
 
 ``X64``
 
 ``64-bit``
 """
-IMUL_R16_RM16_IMM16: Code = 144 # type: ignore
+IMUL_R16_RM16_IMM16: int = 144
 """
 ``IMUL r16, r/m16, imm16``
 
 ``o16 69 /r iw``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-IMUL_R32_RM32_IMM32: Code = 145 # type: ignore
+IMUL_R32_RM32_IMM32: int = 145
 """
 ``IMUL r32, r/m32, imm32``
 
 ``o32 69 /r id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IMUL_R64_RM64_IMM32: Code = 146 # type: ignore
+IMUL_R64_RM64_IMM32: int = 146
 """
 ``IMUL r64, r/m64, imm32``
 
 ``o64 69 /r id``
 
 ``X64``
 
 ``64-bit``
 """
-PUSHW_IMM8: Code = 147 # type: ignore
+PUSHW_IMM8: int = 147
 """
 ``PUSH imm8``
 
 ``o16 6A ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-PUSHD_IMM8: Code = 148 # type: ignore
+PUSHD_IMM8: int = 148
 """
 ``PUSH imm8``
 
 ``o32 6A ib``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSHQ_IMM8: Code = 149 # type: ignore
+PUSHQ_IMM8: int = 149
 """
 ``PUSH imm8``
 
 ``o64 6A ib``
 
 ``X64``
 
 ``64-bit``
 """
-IMUL_R16_RM16_IMM8: Code = 150 # type: ignore
+IMUL_R16_RM16_IMM8: int = 150
 """
 ``IMUL r16, r/m16, imm8``
 
 ``o16 6B /r ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-IMUL_R32_RM32_IMM8: Code = 151 # type: ignore
+IMUL_R32_RM32_IMM8: int = 151
 """
 ``IMUL r32, r/m32, imm8``
 
 ``o32 6B /r ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IMUL_R64_RM64_IMM8: Code = 152 # type: ignore
+IMUL_R64_RM64_IMM8: int = 152
 """
 ``IMUL r64, r/m64, imm8``
 
 ``o64 6B /r ib``
 
 ``X64``
 
 ``64-bit``
 """
-INSB_M8_DX: Code = 153 # type: ignore
+INSB_M8_DX: int = 153
 """
 ``INSB``
 
 ``6C``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-INSW_M16_DX: Code = 154 # type: ignore
+INSW_M16_DX: int = 154
 """
 ``INSW``
 
 ``o16 6D``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-INSD_M32_DX: Code = 155 # type: ignore
+INSD_M32_DX: int = 155
 """
 ``INSD``
 
 ``o32 6D``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OUTSB_DX_M8: Code = 156 # type: ignore
+OUTSB_DX_M8: int = 156
 """
 ``OUTSB``
 
 ``6E``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-OUTSW_DX_M16: Code = 157 # type: ignore
+OUTSW_DX_M16: int = 157
 """
 ``OUTSW``
 
 ``o16 6F``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-OUTSD_DX_M32: Code = 158 # type: ignore
+OUTSD_DX_M32: int = 158
 """
 ``OUTSD``
 
 ``o32 6F``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JO_REL8_16: Code = 159 # type: ignore
+JO_REL8_16: int = 159
 """
 ``JO rel8``
 
 ``o16 70 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JO_REL8_32: Code = 160 # type: ignore
+JO_REL8_32: int = 160
 """
 ``JO rel8``
 
 ``o32 70 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JO_REL8_64: Code = 161 # type: ignore
+JO_REL8_64: int = 161
 """
 ``JO rel8``
 
 ``o64 70 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JNO_REL8_16: Code = 162 # type: ignore
+JNO_REL8_16: int = 162
 """
 ``JNO rel8``
 
 ``o16 71 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JNO_REL8_32: Code = 163 # type: ignore
+JNO_REL8_32: int = 163
 """
 ``JNO rel8``
 
 ``o32 71 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNO_REL8_64: Code = 164 # type: ignore
+JNO_REL8_64: int = 164
 """
 ``JNO rel8``
 
 ``o64 71 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JB_REL8_16: Code = 165 # type: ignore
+JB_REL8_16: int = 165
 """
 ``JB rel8``
 
 ``o16 72 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JB_REL8_32: Code = 166 # type: ignore
+JB_REL8_32: int = 166
 """
 ``JB rel8``
 
 ``o32 72 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JB_REL8_64: Code = 167 # type: ignore
+JB_REL8_64: int = 167
 """
 ``JB rel8``
 
 ``o64 72 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JAE_REL8_16: Code = 168 # type: ignore
+JAE_REL8_16: int = 168
 """
 ``JAE rel8``
 
 ``o16 73 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JAE_REL8_32: Code = 169 # type: ignore
+JAE_REL8_32: int = 169
 """
 ``JAE rel8``
 
 ``o32 73 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JAE_REL8_64: Code = 170 # type: ignore
+JAE_REL8_64: int = 170
 """
 ``JAE rel8``
 
 ``o64 73 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JE_REL8_16: Code = 171 # type: ignore
+JE_REL8_16: int = 171
 """
 ``JE rel8``
 
 ``o16 74 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JE_REL8_32: Code = 172 # type: ignore
+JE_REL8_32: int = 172
 """
 ``JE rel8``
 
 ``o32 74 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JE_REL8_64: Code = 173 # type: ignore
+JE_REL8_64: int = 173
 """
 ``JE rel8``
 
 ``o64 74 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JNE_REL8_16: Code = 174 # type: ignore
+JNE_REL8_16: int = 174
 """
 ``JNE rel8``
 
 ``o16 75 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JNE_REL8_32: Code = 175 # type: ignore
+JNE_REL8_32: int = 175
 """
 ``JNE rel8``
 
 ``o32 75 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNE_REL8_64: Code = 176 # type: ignore
+JNE_REL8_64: int = 176
 """
 ``JNE rel8``
 
 ``o64 75 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JBE_REL8_16: Code = 177 # type: ignore
+JBE_REL8_16: int = 177
 """
 ``JBE rel8``
 
 ``o16 76 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JBE_REL8_32: Code = 178 # type: ignore
+JBE_REL8_32: int = 178
 """
 ``JBE rel8``
 
 ``o32 76 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JBE_REL8_64: Code = 179 # type: ignore
+JBE_REL8_64: int = 179
 """
 ``JBE rel8``
 
 ``o64 76 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JA_REL8_16: Code = 180 # type: ignore
+JA_REL8_16: int = 180
 """
 ``JA rel8``
 
 ``o16 77 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JA_REL8_32: Code = 181 # type: ignore
+JA_REL8_32: int = 181
 """
 ``JA rel8``
 
 ``o32 77 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JA_REL8_64: Code = 182 # type: ignore
+JA_REL8_64: int = 182
 """
 ``JA rel8``
 
 ``o64 77 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JS_REL8_16: Code = 183 # type: ignore
+JS_REL8_16: int = 183
 """
 ``JS rel8``
 
 ``o16 78 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JS_REL8_32: Code = 184 # type: ignore
+JS_REL8_32: int = 184
 """
 ``JS rel8``
 
 ``o32 78 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JS_REL8_64: Code = 185 # type: ignore
+JS_REL8_64: int = 185
 """
 ``JS rel8``
 
 ``o64 78 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JNS_REL8_16: Code = 186 # type: ignore
+JNS_REL8_16: int = 186
 """
 ``JNS rel8``
 
 ``o16 79 cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JNS_REL8_32: Code = 187 # type: ignore
+JNS_REL8_32: int = 187
 """
 ``JNS rel8``
 
 ``o32 79 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNS_REL8_64: Code = 188 # type: ignore
+JNS_REL8_64: int = 188
 """
 ``JNS rel8``
 
 ``o64 79 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JP_REL8_16: Code = 189 # type: ignore
+JP_REL8_16: int = 189
 """
 ``JP rel8``
 
 ``o16 7A cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JP_REL8_32: Code = 190 # type: ignore
+JP_REL8_32: int = 190
 """
 ``JP rel8``
 
 ``o32 7A cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JP_REL8_64: Code = 191 # type: ignore
+JP_REL8_64: int = 191
 """
 ``JP rel8``
 
 ``o64 7A cb``
 
 ``X64``
 
 ``64-bit``
 """
-JNP_REL8_16: Code = 192 # type: ignore
+JNP_REL8_16: int = 192
 """
 ``JNP rel8``
 
 ``o16 7B cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JNP_REL8_32: Code = 193 # type: ignore
+JNP_REL8_32: int = 193
 """
 ``JNP rel8``
 
 ``o32 7B cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNP_REL8_64: Code = 194 # type: ignore
+JNP_REL8_64: int = 194
 """
 ``JNP rel8``
 
 ``o64 7B cb``
 
 ``X64``
 
 ``64-bit``
 """
-JL_REL8_16: Code = 195 # type: ignore
+JL_REL8_16: int = 195
 """
 ``JL rel8``
 
 ``o16 7C cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JL_REL8_32: Code = 196 # type: ignore
+JL_REL8_32: int = 196
 """
 ``JL rel8``
 
 ``o32 7C cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JL_REL8_64: Code = 197 # type: ignore
+JL_REL8_64: int = 197
 """
 ``JL rel8``
 
 ``o64 7C cb``
 
 ``X64``
 
 ``64-bit``
 """
-JGE_REL8_16: Code = 198 # type: ignore
+JGE_REL8_16: int = 198
 """
 ``JGE rel8``
 
 ``o16 7D cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JGE_REL8_32: Code = 199 # type: ignore
+JGE_REL8_32: int = 199
 """
 ``JGE rel8``
 
 ``o32 7D cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JGE_REL8_64: Code = 200 # type: ignore
+JGE_REL8_64: int = 200
 """
 ``JGE rel8``
 
 ``o64 7D cb``
 
 ``X64``
 
 ``64-bit``
 """
-JLE_REL8_16: Code = 201 # type: ignore
+JLE_REL8_16: int = 201
 """
 ``JLE rel8``
 
 ``o16 7E cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JLE_REL8_32: Code = 202 # type: ignore
+JLE_REL8_32: int = 202
 """
 ``JLE rel8``
 
 ``o32 7E cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JLE_REL8_64: Code = 203 # type: ignore
+JLE_REL8_64: int = 203
 """
 ``JLE rel8``
 
 ``o64 7E cb``
 
 ``X64``
 
 ``64-bit``
 """
-JG_REL8_16: Code = 204 # type: ignore
+JG_REL8_16: int = 204
 """
 ``JG rel8``
 
 ``o16 7F cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JG_REL8_32: Code = 205 # type: ignore
+JG_REL8_32: int = 205
 """
 ``JG rel8``
 
 ``o32 7F cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JG_REL8_64: Code = 206 # type: ignore
+JG_REL8_64: int = 206
 """
 ``JG rel8``
 
 ``o64 7F cb``
 
 ``X64``
 
 ``64-bit``
 """
-ADD_RM8_IMM8: Code = 207 # type: ignore
+ADD_RM8_IMM8: int = 207
 """
 ``ADD r/m8, imm8``
 
 ``80 /0 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_RM8_IMM8: Code = 208 # type: ignore
+OR_RM8_IMM8: int = 208
 """
 ``OR r/m8, imm8``
 
 ``80 /1 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_RM8_IMM8: Code = 209 # type: ignore
+ADC_RM8_IMM8: int = 209
 """
 ``ADC r/m8, imm8``
 
 ``80 /2 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_RM8_IMM8: Code = 210 # type: ignore
+SBB_RM8_IMM8: int = 210
 """
 ``SBB r/m8, imm8``
 
 ``80 /3 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_RM8_IMM8: Code = 211 # type: ignore
+AND_RM8_IMM8: int = 211
 """
 ``AND r/m8, imm8``
 
 ``80 /4 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_RM8_IMM8: Code = 212 # type: ignore
+SUB_RM8_IMM8: int = 212
 """
 ``SUB r/m8, imm8``
 
 ``80 /5 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_RM8_IMM8: Code = 213 # type: ignore
+XOR_RM8_IMM8: int = 213
 """
 ``XOR r/m8, imm8``
 
 ``80 /6 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_RM8_IMM8: Code = 214 # type: ignore
+CMP_RM8_IMM8: int = 214
 """
 ``CMP r/m8, imm8``
 
 ``80 /7 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_RM16_IMM16: Code = 215 # type: ignore
+ADD_RM16_IMM16: int = 215
 """
 ``ADD r/m16, imm16``
 
 ``o16 81 /0 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_RM32_IMM32: Code = 216 # type: ignore
+ADD_RM32_IMM32: int = 216
 """
 ``ADD r/m32, imm32``
 
 ``o32 81 /0 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADD_RM64_IMM32: Code = 217 # type: ignore
+ADD_RM64_IMM32: int = 217
 """
 ``ADD r/m64, imm32``
 
 ``o64 81 /0 id``
 
 ``X64``
 
 ``64-bit``
 """
-OR_RM16_IMM16: Code = 218 # type: ignore
+OR_RM16_IMM16: int = 218
 """
 ``OR r/m16, imm16``
 
 ``o16 81 /1 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_RM32_IMM32: Code = 219 # type: ignore
+OR_RM32_IMM32: int = 219
 """
 ``OR r/m32, imm32``
 
 ``o32 81 /1 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OR_RM64_IMM32: Code = 220 # type: ignore
+OR_RM64_IMM32: int = 220
 """
 ``OR r/m64, imm32``
 
 ``o64 81 /1 id``
 
 ``X64``
 
 ``64-bit``
 """
-ADC_RM16_IMM16: Code = 221 # type: ignore
+ADC_RM16_IMM16: int = 221
 """
 ``ADC r/m16, imm16``
 
 ``o16 81 /2 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_RM32_IMM32: Code = 222 # type: ignore
+ADC_RM32_IMM32: int = 222
 """
 ``ADC r/m32, imm32``
 
 ``o32 81 /2 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADC_RM64_IMM32: Code = 223 # type: ignore
+ADC_RM64_IMM32: int = 223
 """
 ``ADC r/m64, imm32``
 
 ``o64 81 /2 id``
 
 ``X64``
 
 ``64-bit``
 """
-SBB_RM16_IMM16: Code = 224 # type: ignore
+SBB_RM16_IMM16: int = 224
 """
 ``SBB r/m16, imm16``
 
 ``o16 81 /3 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_RM32_IMM32: Code = 225 # type: ignore
+SBB_RM32_IMM32: int = 225
 """
 ``SBB r/m32, imm32``
 
 ``o32 81 /3 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SBB_RM64_IMM32: Code = 226 # type: ignore
+SBB_RM64_IMM32: int = 226
 """
 ``SBB r/m64, imm32``
 
 ``o64 81 /3 id``
 
 ``X64``
 
 ``64-bit``
 """
-AND_RM16_IMM16: Code = 227 # type: ignore
+AND_RM16_IMM16: int = 227
 """
 ``AND r/m16, imm16``
 
 ``o16 81 /4 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_RM32_IMM32: Code = 228 # type: ignore
+AND_RM32_IMM32: int = 228
 """
 ``AND r/m32, imm32``
 
 ``o32 81 /4 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-AND_RM64_IMM32: Code = 229 # type: ignore
+AND_RM64_IMM32: int = 229
 """
 ``AND r/m64, imm32``
 
 ``o64 81 /4 id``
 
 ``X64``
 
 ``64-bit``
 """
-SUB_RM16_IMM16: Code = 230 # type: ignore
+SUB_RM16_IMM16: int = 230
 """
 ``SUB r/m16, imm16``
 
 ``o16 81 /5 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_RM32_IMM32: Code = 231 # type: ignore
+SUB_RM32_IMM32: int = 231
 """
 ``SUB r/m32, imm32``
 
 ``o32 81 /5 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SUB_RM64_IMM32: Code = 232 # type: ignore
+SUB_RM64_IMM32: int = 232
 """
 ``SUB r/m64, imm32``
 
 ``o64 81 /5 id``
 
 ``X64``
 
 ``64-bit``
 """
-XOR_RM16_IMM16: Code = 233 # type: ignore
+XOR_RM16_IMM16: int = 233
 """
 ``XOR r/m16, imm16``
 
 ``o16 81 /6 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_RM32_IMM32: Code = 234 # type: ignore
+XOR_RM32_IMM32: int = 234
 """
 ``XOR r/m32, imm32``
 
 ``o32 81 /6 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XOR_RM64_IMM32: Code = 235 # type: ignore
+XOR_RM64_IMM32: int = 235
 """
 ``XOR r/m64, imm32``
 
 ``o64 81 /6 id``
 
 ``X64``
 
 ``64-bit``
 """
-CMP_RM16_IMM16: Code = 236 # type: ignore
+CMP_RM16_IMM16: int = 236
 """
 ``CMP r/m16, imm16``
 
 ``o16 81 /7 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_RM32_IMM32: Code = 237 # type: ignore
+CMP_RM32_IMM32: int = 237
 """
 ``CMP r/m32, imm32``
 
 ``o32 81 /7 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMP_RM64_IMM32: Code = 238 # type: ignore
+CMP_RM64_IMM32: int = 238
 """
 ``CMP r/m64, imm32``
 
 ``o64 81 /7 id``
 
 ``X64``
 
 ``64-bit``
 """
-ADD_RM8_IMM8_82: Code = 239 # type: ignore
+ADD_RM8_IMM8_82: int = 239
 """
 ``ADD r/m8, imm8``
 
 ``82 /0 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-OR_RM8_IMM8_82: Code = 240 # type: ignore
+OR_RM8_IMM8_82: int = 240
 """
 ``OR r/m8, imm8``
 
 ``82 /1 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-ADC_RM8_IMM8_82: Code = 241 # type: ignore
+ADC_RM8_IMM8_82: int = 241
 """
 ``ADC r/m8, imm8``
 
 ``82 /2 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-SBB_RM8_IMM8_82: Code = 242 # type: ignore
+SBB_RM8_IMM8_82: int = 242
 """
 ``SBB r/m8, imm8``
 
 ``82 /3 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-AND_RM8_IMM8_82: Code = 243 # type: ignore
+AND_RM8_IMM8_82: int = 243
 """
 ``AND r/m8, imm8``
 
 ``82 /4 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-SUB_RM8_IMM8_82: Code = 244 # type: ignore
+SUB_RM8_IMM8_82: int = 244
 """
 ``SUB r/m8, imm8``
 
 ``82 /5 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-XOR_RM8_IMM8_82: Code = 245 # type: ignore
+XOR_RM8_IMM8_82: int = 245
 """
 ``XOR r/m8, imm8``
 
 ``82 /6 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-CMP_RM8_IMM8_82: Code = 246 # type: ignore
+CMP_RM8_IMM8_82: int = 246
 """
 ``CMP r/m8, imm8``
 
 ``82 /7 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-ADD_RM16_IMM8: Code = 247 # type: ignore
+ADD_RM16_IMM8: int = 247
 """
 ``ADD r/m16, imm8``
 
 ``o16 83 /0 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADD_RM32_IMM8: Code = 248 # type: ignore
+ADD_RM32_IMM8: int = 248
 """
 ``ADD r/m32, imm8``
 
 ``o32 83 /0 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADD_RM64_IMM8: Code = 249 # type: ignore
+ADD_RM64_IMM8: int = 249
 """
 ``ADD r/m64, imm8``
 
 ``o64 83 /0 ib``
 
 ``X64``
 
 ``64-bit``
 """
-OR_RM16_IMM8: Code = 250 # type: ignore
+OR_RM16_IMM8: int = 250
 """
 ``OR r/m16, imm8``
 
 ``o16 83 /1 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OR_RM32_IMM8: Code = 251 # type: ignore
+OR_RM32_IMM8: int = 251
 """
 ``OR r/m32, imm8``
 
 ``o32 83 /1 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OR_RM64_IMM8: Code = 252 # type: ignore
+OR_RM64_IMM8: int = 252
 """
 ``OR r/m64, imm8``
 
 ``o64 83 /1 ib``
 
 ``X64``
 
 ``64-bit``
 """
-ADC_RM16_IMM8: Code = 253 # type: ignore
+ADC_RM16_IMM8: int = 253
 """
 ``ADC r/m16, imm8``
 
 ``o16 83 /2 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ADC_RM32_IMM8: Code = 254 # type: ignore
+ADC_RM32_IMM8: int = 254
 """
 ``ADC r/m32, imm8``
 
 ``o32 83 /2 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ADC_RM64_IMM8: Code = 255 # type: ignore
+ADC_RM64_IMM8: int = 255
 """
 ``ADC r/m64, imm8``
 
 ``o64 83 /2 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SBB_RM16_IMM8: Code = 256 # type: ignore
+SBB_RM16_IMM8: int = 256
 """
 ``SBB r/m16, imm8``
 
 ``o16 83 /3 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SBB_RM32_IMM8: Code = 257 # type: ignore
+SBB_RM32_IMM8: int = 257
 """
 ``SBB r/m32, imm8``
 
 ``o32 83 /3 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SBB_RM64_IMM8: Code = 258 # type: ignore
+SBB_RM64_IMM8: int = 258
 """
 ``SBB r/m64, imm8``
 
 ``o64 83 /3 ib``
 
 ``X64``
 
 ``64-bit``
 """
-AND_RM16_IMM8: Code = 259 # type: ignore
+AND_RM16_IMM8: int = 259
 """
 ``AND r/m16, imm8``
 
 ``o16 83 /4 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-AND_RM32_IMM8: Code = 260 # type: ignore
+AND_RM32_IMM8: int = 260
 """
 ``AND r/m32, imm8``
 
 ``o32 83 /4 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-AND_RM64_IMM8: Code = 261 # type: ignore
+AND_RM64_IMM8: int = 261
 """
 ``AND r/m64, imm8``
 
 ``o64 83 /4 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SUB_RM16_IMM8: Code = 262 # type: ignore
+SUB_RM16_IMM8: int = 262
 """
 ``SUB r/m16, imm8``
 
 ``o16 83 /5 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SUB_RM32_IMM8: Code = 263 # type: ignore
+SUB_RM32_IMM8: int = 263
 """
 ``SUB r/m32, imm8``
 
 ``o32 83 /5 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SUB_RM64_IMM8: Code = 264 # type: ignore
+SUB_RM64_IMM8: int = 264
 """
 ``SUB r/m64, imm8``
 
 ``o64 83 /5 ib``
 
 ``X64``
 
 ``64-bit``
 """
-XOR_RM16_IMM8: Code = 265 # type: ignore
+XOR_RM16_IMM8: int = 265
 """
 ``XOR r/m16, imm8``
 
 ``o16 83 /6 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XOR_RM32_IMM8: Code = 266 # type: ignore
+XOR_RM32_IMM8: int = 266
 """
 ``XOR r/m32, imm8``
 
 ``o32 83 /6 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XOR_RM64_IMM8: Code = 267 # type: ignore
+XOR_RM64_IMM8: int = 267
 """
 ``XOR r/m64, imm8``
 
 ``o64 83 /6 ib``
 
 ``X64``
 
 ``64-bit``
 """
-CMP_RM16_IMM8: Code = 268 # type: ignore
+CMP_RM16_IMM8: int = 268
 """
 ``CMP r/m16, imm8``
 
 ``o16 83 /7 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMP_RM32_IMM8: Code = 269 # type: ignore
+CMP_RM32_IMM8: int = 269
 """
 ``CMP r/m32, imm8``
 
 ``o32 83 /7 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMP_RM64_IMM8: Code = 270 # type: ignore
+CMP_RM64_IMM8: int = 270
 """
 ``CMP r/m64, imm8``
 
 ``o64 83 /7 ib``
 
 ``X64``
 
 ``64-bit``
 """
-TEST_RM8_R8: Code = 271 # type: ignore
+TEST_RM8_R8: int = 271
 """
 ``TEST r/m8, r8``
 
 ``84 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM16_R16: Code = 272 # type: ignore
+TEST_RM16_R16: int = 272
 """
 ``TEST r/m16, r16``
 
 ``o16 85 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM32_R32: Code = 273 # type: ignore
+TEST_RM32_R32: int = 273
 """
 ``TEST r/m32, r32``
 
 ``o32 85 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-TEST_RM64_R64: Code = 274 # type: ignore
+TEST_RM64_R64: int = 274
 """
 ``TEST r/m64, r64``
 
 ``o64 85 /r``
 
 ``X64``
 
 ``64-bit``
 """
-XCHG_RM8_R8: Code = 275 # type: ignore
+XCHG_RM8_R8: int = 275
 """
 ``XCHG r/m8, r8``
 
 ``86 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XCHG_RM16_R16: Code = 276 # type: ignore
+XCHG_RM16_R16: int = 276
 """
 ``XCHG r/m16, r16``
 
 ``o16 87 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XCHG_RM32_R32: Code = 277 # type: ignore
+XCHG_RM32_R32: int = 277
 """
 ``XCHG r/m32, r32``
 
 ``o32 87 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XCHG_RM64_R64: Code = 278 # type: ignore
+XCHG_RM64_R64: int = 278
 """
 ``XCHG r/m64, r64``
 
 ``o64 87 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_RM8_R8: Code = 279 # type: ignore
+MOV_RM8_R8: int = 279
 """
 ``MOV r/m8, r8``
 
 ``88 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_RM16_R16: Code = 280 # type: ignore
+MOV_RM16_R16: int = 280
 """
 ``MOV r/m16, r16``
 
 ``o16 89 /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_RM32_R32: Code = 281 # type: ignore
+MOV_RM32_R32: int = 281
 """
 ``MOV r/m32, r32``
 
 ``o32 89 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_RM64_R64: Code = 282 # type: ignore
+MOV_RM64_R64: int = 282
 """
 ``MOV r/m64, r64``
 
 ``o64 89 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_R8_RM8: Code = 283 # type: ignore
+MOV_R8_RM8: int = 283
 """
 ``MOV r8, r/m8``
 
 ``8A /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_R16_RM16: Code = 284 # type: ignore
+MOV_R16_RM16: int = 284
 """
 ``MOV r16, r/m16``
 
 ``o16 8B /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_R32_RM32: Code = 285 # type: ignore
+MOV_R32_RM32: int = 285
 """
 ``MOV r32, r/m32``
 
 ``o32 8B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_R64_RM64: Code = 286 # type: ignore
+MOV_R64_RM64: int = 286
 """
 ``MOV r64, r/m64``
 
 ``o64 8B /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_RM16_SREG: Code = 287 # type: ignore
+MOV_RM16_SREG: int = 287
 """
 ``MOV r/m16, Sreg``
 
 ``o16 8C /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_R32M16_SREG: Code = 288 # type: ignore
+MOV_R32M16_SREG: int = 288
 """
 ``MOV r32/m16, Sreg``
 
 ``o32 8C /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_R64M16_SREG: Code = 289 # type: ignore
+MOV_R64M16_SREG: int = 289
 """
 ``MOV r64/m16, Sreg``
 
 ``o64 8C /r``
 
 ``X64``
 
 ``64-bit``
 """
-LEA_R16_M: Code = 290 # type: ignore
+LEA_R16_M: int = 290
 """
 ``LEA r16, m``
 
 ``o16 8D /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-LEA_R32_M: Code = 291 # type: ignore
+LEA_R32_M: int = 291
 """
 ``LEA r32, m``
 
 ``o32 8D /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LEA_R64_M: Code = 292 # type: ignore
+LEA_R64_M: int = 292
 """
 ``LEA r64, m``
 
 ``o64 8D /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_SREG_RM16: Code = 293 # type: ignore
+MOV_SREG_RM16: int = 293
 """
 ``MOV Sreg, r/m16``
 
 ``o16 8E /r``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_SREG_R32M16: Code = 294 # type: ignore
+MOV_SREG_R32M16: int = 294
 """
 ``MOV Sreg, r32/m16``
 
 ``o32 8E /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_SREG_R64M16: Code = 295 # type: ignore
+MOV_SREG_R64M16: int = 295
 """
 ``MOV Sreg, r64/m16``
 
 ``o64 8E /r``
 
 ``X64``
 
 ``64-bit``
 """
-POP_RM16: Code = 296 # type: ignore
+POP_RM16: int = 296
 """
 ``POP r/m16``
 
 ``o16 8F /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-POP_RM32: Code = 297 # type: ignore
+POP_RM32: int = 297
 """
 ``POP r/m32``
 
 ``o32 8F /0``
 
 ``386+``
 
 ``16/32-bit``
 """
-POP_RM64: Code = 298 # type: ignore
+POP_RM64: int = 298
 """
 ``POP r/m64``
 
 ``o64 8F /0``
 
 ``X64``
 
 ``64-bit``
 """
-NOPW: Code = 299 # type: ignore
+NOPW: int = 299
 """
 ``NOP``
 
 ``o16 90``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NOPD: Code = 300 # type: ignore
+NOPD: int = 300
 """
 ``NOP``
 
 ``o32 90``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NOPQ: Code = 301 # type: ignore
+NOPQ: int = 301
 """
 ``NOP``
 
 ``o64 90``
 
 ``8086+``
 
 ``64-bit``
 """
-XCHG_R16_AX: Code = 302 # type: ignore
+XCHG_R16_AX: int = 302
 """
 ``XCHG r16, AX``
 
 ``o16 90+rw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XCHG_R32_EAX: Code = 303 # type: ignore
+XCHG_R32_EAX: int = 303
 """
 ``XCHG r32, EAX``
 
 ``o32 90+rd``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-XCHG_R64_RAX: Code = 304 # type: ignore
+XCHG_R64_RAX: int = 304
 """
 ``XCHG r64, RAX``
 
 ``o64 90+ro``
 
 ``X64``
 
 ``64-bit``
 """
-PAUSE: Code = 305 # type: ignore
+PAUSE: int = 305
 """
 ``PAUSE``
 
 ``F3 90``
 
 ``Pentium 4 or later``
 
 ``16/32/64-bit``
 """
-CBW: Code = 306 # type: ignore
+CBW: int = 306
 """
 ``CBW``
 
 ``o16 98``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CWDE: Code = 307 # type: ignore
+CWDE: int = 307
 """
 ``CWDE``
 
 ``o32 98``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CDQE: Code = 308 # type: ignore
+CDQE: int = 308
 """
 ``CDQE``
 
 ``o64 98``
 
 ``X64``
 
 ``64-bit``
 """
-CWD: Code = 309 # type: ignore
+CWD: int = 309
 """
 ``CWD``
 
 ``o16 99``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CDQ: Code = 310 # type: ignore
+CDQ: int = 310
 """
 ``CDQ``
 
 ``o32 99``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CQO: Code = 311 # type: ignore
+CQO: int = 311
 """
 ``CQO``
 
 ``o64 99``
 
 ``X64``
 
 ``64-bit``
 """
-CALL_PTR1616: Code = 312 # type: ignore
+CALL_PTR1616: int = 312
 """
 ``CALL ptr16:16``
 
 ``o16 9A cd``
 
 ``8086+``
 
 ``16/32-bit``
 """
-CALL_PTR1632: Code = 313 # type: ignore
+CALL_PTR1632: int = 313
 """
 ``CALL ptr16:32``
 
 ``o32 9A cp``
 
 ``386+``
 
 ``16/32-bit``
 """
-WAIT: Code = 314 # type: ignore
+WAIT: int = 314
 """
 ``WAIT``
 
 ``9B``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-PUSHFW: Code = 315 # type: ignore
+PUSHFW: int = 315
 """
 ``PUSHF``
 
 ``o16 9C``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-PUSHFD: Code = 316 # type: ignore
+PUSHFD: int = 316
 """
 ``PUSHFD``
 
 ``o32 9C``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSHFQ: Code = 317 # type: ignore
+PUSHFQ: int = 317
 """
 ``PUSHFQ``
 
 ``o64 9C``
 
 ``X64``
 
 ``64-bit``
 """
-POPFW: Code = 318 # type: ignore
+POPFW: int = 318
 """
 ``POPF``
 
 ``o16 9D``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-POPFD: Code = 319 # type: ignore
+POPFD: int = 319
 """
 ``POPFD``
 
 ``o32 9D``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPFQ: Code = 320 # type: ignore
+POPFQ: int = 320
 """
 ``POPFQ``
 
 ``o64 9D``
 
 ``X64``
 
 ``64-bit``
 """
-SAHF: Code = 321 # type: ignore
+SAHF: int = 321
 """
 ``SAHF``
 
 ``9E``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-LAHF: Code = 322 # type: ignore
+LAHF: int = 322
 """
 ``LAHF``
 
 ``9F``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_AL_MOFFS8: Code = 323 # type: ignore
+MOV_AL_MOFFS8: int = 323
 """
 ``MOV AL, moffs8``
 
 ``A0 mo``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_AX_MOFFS16: Code = 324 # type: ignore
+MOV_AX_MOFFS16: int = 324
 """
 ``MOV AX, moffs16``
 
 ``o16 A1 mo``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_EAX_MOFFS32: Code = 325 # type: ignore
+MOV_EAX_MOFFS32: int = 325
 """
 ``MOV EAX, moffs32``
 
 ``o32 A1 mo``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_RAX_MOFFS64: Code = 326 # type: ignore
+MOV_RAX_MOFFS64: int = 326
 """
 ``MOV RAX, moffs64``
 
 ``o64 A1 mo``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_MOFFS8_AL: Code = 327 # type: ignore
+MOV_MOFFS8_AL: int = 327
 """
 ``MOV moffs8, AL``
 
 ``A2 mo``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_MOFFS16_AX: Code = 328 # type: ignore
+MOV_MOFFS16_AX: int = 328
 """
 ``MOV moffs16, AX``
 
 ``o16 A3 mo``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_MOFFS32_EAX: Code = 329 # type: ignore
+MOV_MOFFS32_EAX: int = 329
 """
 ``MOV moffs32, EAX``
 
 ``o32 A3 mo``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_MOFFS64_RAX: Code = 330 # type: ignore
+MOV_MOFFS64_RAX: int = 330
 """
 ``MOV moffs64, RAX``
 
 ``o64 A3 mo``
 
 ``X64``
 
 ``64-bit``
 """
-MOVSB_M8_M8: Code = 331 # type: ignore
+MOVSB_M8_M8: int = 331
 """
 ``MOVSB``
 
 ``A4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOVSW_M16_M16: Code = 332 # type: ignore
+MOVSW_M16_M16: int = 332
 """
 ``MOVSW``
 
 ``o16 A5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOVSD_M32_M32: Code = 333 # type: ignore
+MOVSD_M32_M32: int = 333
 """
 ``MOVSD``
 
 ``o32 A5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVSQ_M64_M64: Code = 334 # type: ignore
+MOVSQ_M64_M64: int = 334
 """
 ``MOVSQ``
 
 ``o64 A5``
 
 ``X64``
 
 ``64-bit``
 """
-CMPSB_M8_M8: Code = 335 # type: ignore
+CMPSB_M8_M8: int = 335
 """
 ``CMPSB``
 
 ``A6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMPSW_M16_M16: Code = 336 # type: ignore
+CMPSW_M16_M16: int = 336
 """
 ``CMPSW``
 
 ``o16 A7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMPSD_M32_M32: Code = 337 # type: ignore
+CMPSD_M32_M32: int = 337
 """
 ``CMPSD``
 
 ``o32 A7``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CMPSQ_M64_M64: Code = 338 # type: ignore
+CMPSQ_M64_M64: int = 338
 """
 ``CMPSQ``
 
 ``o64 A7``
 
 ``X64``
 
 ``64-bit``
 """
-TEST_AL_IMM8: Code = 339 # type: ignore
+TEST_AL_IMM8: int = 339
 """
 ``TEST AL, imm8``
 
 ``A8 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_AX_IMM16: Code = 340 # type: ignore
+TEST_AX_IMM16: int = 340
 """
 ``TEST AX, imm16``
 
 ``o16 A9 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_EAX_IMM32: Code = 341 # type: ignore
+TEST_EAX_IMM32: int = 341
 """
 ``TEST EAX, imm32``
 
 ``o32 A9 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-TEST_RAX_IMM32: Code = 342 # type: ignore
+TEST_RAX_IMM32: int = 342
 """
 ``TEST RAX, imm32``
 
 ``o64 A9 id``
 
 ``X64``
 
 ``64-bit``
 """
-STOSB_M8_AL: Code = 343 # type: ignore
+STOSB_M8_AL: int = 343
 """
 ``STOSB``
 
 ``AA``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-STOSW_M16_AX: Code = 344 # type: ignore
+STOSW_M16_AX: int = 344
 """
 ``STOSW``
 
 ``o16 AB``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-STOSD_M32_EAX: Code = 345 # type: ignore
+STOSD_M32_EAX: int = 345
 """
 ``STOSD``
 
 ``o32 AB``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-STOSQ_M64_RAX: Code = 346 # type: ignore
+STOSQ_M64_RAX: int = 346
 """
 ``STOSQ``
 
 ``o64 AB``
 
 ``X64``
 
 ``64-bit``
 """
-LODSB_AL_M8: Code = 347 # type: ignore
+LODSB_AL_M8: int = 347
 """
 ``LODSB``
 
 ``AC``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-LODSW_AX_M16: Code = 348 # type: ignore
+LODSW_AX_M16: int = 348
 """
 ``LODSW``
 
 ``o16 AD``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-LODSD_EAX_M32: Code = 349 # type: ignore
+LODSD_EAX_M32: int = 349
 """
 ``LODSD``
 
 ``o32 AD``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LODSQ_RAX_M64: Code = 350 # type: ignore
+LODSQ_RAX_M64: int = 350
 """
 ``LODSQ``
 
 ``o64 AD``
 
 ``X64``
 
 ``64-bit``
 """
-SCASB_AL_M8: Code = 351 # type: ignore
+SCASB_AL_M8: int = 351
 """
 ``SCASB``
 
 ``AE``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SCASW_AX_M16: Code = 352 # type: ignore
+SCASW_AX_M16: int = 352
 """
 ``SCASW``
 
 ``o16 AF``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SCASD_EAX_M32: Code = 353 # type: ignore
+SCASD_EAX_M32: int = 353
 """
 ``SCASD``
 
 ``o32 AF``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SCASQ_RAX_M64: Code = 354 # type: ignore
+SCASQ_RAX_M64: int = 354
 """
 ``SCASQ``
 
 ``o64 AF``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_R8_IMM8: Code = 355 # type: ignore
+MOV_R8_IMM8: int = 355
 """
 ``MOV r8, imm8``
 
 ``B0+rb ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_R16_IMM16: Code = 356 # type: ignore
+MOV_R16_IMM16: int = 356
 """
 ``MOV r16, imm16``
 
 ``o16 B8+rw iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_R32_IMM32: Code = 357 # type: ignore
+MOV_R32_IMM32: int = 357
 """
 ``MOV r32, imm32``
 
 ``o32 B8+rd id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_R64_IMM64: Code = 358 # type: ignore
+MOV_R64_IMM64: int = 358
 """
 ``MOV r64, imm64``
 
 ``o64 B8+ro io``
 
 ``X64``
 
 ``64-bit``
 """
-ROL_RM8_IMM8: Code = 359 # type: ignore
+ROL_RM8_IMM8: int = 359
 """
 ``ROL r/m8, imm8``
 
 ``C0 /0 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-ROR_RM8_IMM8: Code = 360 # type: ignore
+ROR_RM8_IMM8: int = 360
 """
 ``ROR r/m8, imm8``
 
 ``C0 /1 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-RCL_RM8_IMM8: Code = 361 # type: ignore
+RCL_RM8_IMM8: int = 361
 """
 ``RCL r/m8, imm8``
 
 ``C0 /2 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-RCR_RM8_IMM8: Code = 362 # type: ignore
+RCR_RM8_IMM8: int = 362
 """
 ``RCR r/m8, imm8``
 
 ``C0 /3 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SHL_RM8_IMM8: Code = 363 # type: ignore
+SHL_RM8_IMM8: int = 363
 """
 ``SHL r/m8, imm8``
 
 ``C0 /4 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SHR_RM8_IMM8: Code = 364 # type: ignore
+SHR_RM8_IMM8: int = 364
 """
 ``SHR r/m8, imm8``
 
 ``C0 /5 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SAL_RM8_IMM8: Code = 365 # type: ignore
+SAL_RM8_IMM8: int = 365
 """
 ``SAL r/m8, imm8``
 
 ``C0 /6 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SAR_RM8_IMM8: Code = 366 # type: ignore
+SAR_RM8_IMM8: int = 366
 """
 ``SAR r/m8, imm8``
 
 ``C0 /7 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-ROL_RM16_IMM8: Code = 367 # type: ignore
+ROL_RM16_IMM8: int = 367
 """
 ``ROL r/m16, imm8``
 
 ``o16 C1 /0 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-ROL_RM32_IMM8: Code = 368 # type: ignore
+ROL_RM32_IMM8: int = 368
 """
 ``ROL r/m32, imm8``
 
 ``o32 C1 /0 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROL_RM64_IMM8: Code = 369 # type: ignore
+ROL_RM64_IMM8: int = 369
 """
 ``ROL r/m64, imm8``
 
 ``o64 C1 /0 ib``
 
 ``X64``
 
 ``64-bit``
 """
-ROR_RM16_IMM8: Code = 370 # type: ignore
+ROR_RM16_IMM8: int = 370
 """
 ``ROR r/m16, imm8``
 
 ``o16 C1 /1 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-ROR_RM32_IMM8: Code = 371 # type: ignore
+ROR_RM32_IMM8: int = 371
 """
 ``ROR r/m32, imm8``
 
 ``o32 C1 /1 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROR_RM64_IMM8: Code = 372 # type: ignore
+ROR_RM64_IMM8: int = 372
 """
 ``ROR r/m64, imm8``
 
 ``o64 C1 /1 ib``
 
 ``X64``
 
 ``64-bit``
 """
-RCL_RM16_IMM8: Code = 373 # type: ignore
+RCL_RM16_IMM8: int = 373
 """
 ``RCL r/m16, imm8``
 
 ``o16 C1 /2 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-RCL_RM32_IMM8: Code = 374 # type: ignore
+RCL_RM32_IMM8: int = 374
 """
 ``RCL r/m32, imm8``
 
 ``o32 C1 /2 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCL_RM64_IMM8: Code = 375 # type: ignore
+RCL_RM64_IMM8: int = 375
 """
 ``RCL r/m64, imm8``
 
 ``o64 C1 /2 ib``
 
 ``X64``
 
 ``64-bit``
 """
-RCR_RM16_IMM8: Code = 376 # type: ignore
+RCR_RM16_IMM8: int = 376
 """
 ``RCR r/m16, imm8``
 
 ``o16 C1 /3 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-RCR_RM32_IMM8: Code = 377 # type: ignore
+RCR_RM32_IMM8: int = 377
 """
 ``RCR r/m32, imm8``
 
 ``o32 C1 /3 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCR_RM64_IMM8: Code = 378 # type: ignore
+RCR_RM64_IMM8: int = 378
 """
 ``RCR r/m64, imm8``
 
 ``o64 C1 /3 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SHL_RM16_IMM8: Code = 379 # type: ignore
+SHL_RM16_IMM8: int = 379
 """
 ``SHL r/m16, imm8``
 
 ``o16 C1 /4 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SHL_RM32_IMM8: Code = 380 # type: ignore
+SHL_RM32_IMM8: int = 380
 """
 ``SHL r/m32, imm8``
 
 ``o32 C1 /4 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHL_RM64_IMM8: Code = 381 # type: ignore
+SHL_RM64_IMM8: int = 381
 """
 ``SHL r/m64, imm8``
 
 ``o64 C1 /4 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SHR_RM16_IMM8: Code = 382 # type: ignore
+SHR_RM16_IMM8: int = 382
 """
 ``SHR r/m16, imm8``
 
 ``o16 C1 /5 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SHR_RM32_IMM8: Code = 383 # type: ignore
+SHR_RM32_IMM8: int = 383
 """
 ``SHR r/m32, imm8``
 
 ``o32 C1 /5 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHR_RM64_IMM8: Code = 384 # type: ignore
+SHR_RM64_IMM8: int = 384
 """
 ``SHR r/m64, imm8``
 
 ``o64 C1 /5 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SAL_RM16_IMM8: Code = 385 # type: ignore
+SAL_RM16_IMM8: int = 385
 """
 ``SAL r/m16, imm8``
 
 ``o16 C1 /6 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SAL_RM32_IMM8: Code = 386 # type: ignore
+SAL_RM32_IMM8: int = 386
 """
 ``SAL r/m32, imm8``
 
 ``o32 C1 /6 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAL_RM64_IMM8: Code = 387 # type: ignore
+SAL_RM64_IMM8: int = 387
 """
 ``SAL r/m64, imm8``
 
 ``o64 C1 /6 ib``
 
 ``X64``
 
 ``64-bit``
 """
-SAR_RM16_IMM8: Code = 388 # type: ignore
+SAR_RM16_IMM8: int = 388
 """
 ``SAR r/m16, imm8``
 
 ``o16 C1 /7 ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-SAR_RM32_IMM8: Code = 389 # type: ignore
+SAR_RM32_IMM8: int = 389
 """
 ``SAR r/m32, imm8``
 
 ``o32 C1 /7 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAR_RM64_IMM8: Code = 390 # type: ignore
+SAR_RM64_IMM8: int = 390
 """
 ``SAR r/m64, imm8``
 
 ``o64 C1 /7 ib``
 
 ``X64``
 
 ``64-bit``
 """
-RETNW_IMM16: Code = 391 # type: ignore
+RETNW_IMM16: int = 391
 """
 ``RET imm16``
 
 ``o16 C2 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RETND_IMM16: Code = 392 # type: ignore
+RETND_IMM16: int = 392
 """
 ``RET imm16``
 
 ``o32 C2 iw``
 
 ``386+``
 
 ``16/32-bit``
 """
-RETNQ_IMM16: Code = 393 # type: ignore
+RETNQ_IMM16: int = 393
 """
 ``RET imm16``
 
 ``o64 C2 iw``
 
 ``X64``
 
 ``64-bit``
 """
-RETNW: Code = 394 # type: ignore
+RETNW: int = 394
 """
 ``RET``
 
 ``o16 C3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RETND: Code = 395 # type: ignore
+RETND: int = 395
 """
 ``RET``
 
 ``o32 C3``
 
 ``386+``
 
 ``16/32-bit``
 """
-RETNQ: Code = 396 # type: ignore
+RETNQ: int = 396
 """
 ``RET``
 
 ``o64 C3``
 
 ``X64``
 
 ``64-bit``
 """
-LES_R16_M1616: Code = 397 # type: ignore
+LES_R16_M1616: int = 397
 """
 ``LES r16, m16:16``
 
 ``o16 C4 /r``
 
 ``8086+``
 
 ``16/32-bit``
 """
-LES_R32_M1632: Code = 398 # type: ignore
+LES_R32_M1632: int = 398
 """
 ``LES r32, m16:32``
 
 ``o32 C4 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-LDS_R16_M1616: Code = 399 # type: ignore
+LDS_R16_M1616: int = 399
 """
 ``LDS r16, m16:16``
 
 ``o16 C5 /r``
 
 ``8086+``
 
 ``16/32-bit``
 """
-LDS_R32_M1632: Code = 400 # type: ignore
+LDS_R32_M1632: int = 400
 """
 ``LDS r32, m16:32``
 
 ``o32 C5 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOV_RM8_IMM8: Code = 401 # type: ignore
+MOV_RM8_IMM8: int = 401
 """
 ``MOV r/m8, imm8``
 
 ``C6 /0 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-XABORT_IMM8: Code = 402 # type: ignore
+XABORT_IMM8: int = 402
 """
 ``XABORT imm8``
 
 ``C6 F8 ib``
 
 ``RTM``
 
 ``16/32/64-bit``
 """
-MOV_RM16_IMM16: Code = 403 # type: ignore
+MOV_RM16_IMM16: int = 403
 """
 ``MOV r/m16, imm16``
 
 ``o16 C7 /0 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MOV_RM32_IMM32: Code = 404 # type: ignore
+MOV_RM32_IMM32: int = 404
 """
 ``MOV r/m32, imm32``
 
 ``o32 C7 /0 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOV_RM64_IMM32: Code = 405 # type: ignore
+MOV_RM64_IMM32: int = 405
 """
 ``MOV r/m64, imm32``
 
 ``o64 C7 /0 id``
 
 ``X64``
 
 ``64-bit``
 """
-XBEGIN_REL16: Code = 406 # type: ignore
+XBEGIN_REL16: int = 406
 """
 ``XBEGIN rel16``
 
 ``o16 C7 F8 cw``
 
 ``RTM``
 
 ``16/32/64-bit``
 """
-XBEGIN_REL32: Code = 407 # type: ignore
+XBEGIN_REL32: int = 407
 """
 ``XBEGIN rel32``
 
 ``o32 C7 F8 cd``
 
 ``RTM``
 
 ``16/32/64-bit``
 """
-ENTERW_IMM16_IMM8: Code = 408 # type: ignore
+ENTERW_IMM16_IMM8: int = 408
 """
 ``ENTER imm16, imm8``
 
 ``o16 C8 iw ib``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-ENTERD_IMM16_IMM8: Code = 409 # type: ignore
+ENTERD_IMM16_IMM8: int = 409
 """
 ``ENTER imm16, imm8``
 
 ``o32 C8 iw ib``
 
 ``386+``
 
 ``16/32-bit``
 """
-ENTERQ_IMM16_IMM8: Code = 410 # type: ignore
+ENTERQ_IMM16_IMM8: int = 410
 """
 ``ENTER imm16, imm8``
 
 ``o64 C8 iw ib``
 
 ``X64``
 
 ``64-bit``
 """
-LEAVEW: Code = 411 # type: ignore
+LEAVEW: int = 411
 """
 ``LEAVE``
 
 ``o16 C9``
 
 ``186+``
 
 ``16/32/64-bit``
 """
-LEAVED: Code = 412 # type: ignore
+LEAVED: int = 412
 """
 ``LEAVE``
 
 ``o32 C9``
 
 ``386+``
 
 ``16/32-bit``
 """
-LEAVEQ: Code = 413 # type: ignore
+LEAVEQ: int = 413
 """
 ``LEAVE``
 
 ``o64 C9``
 
 ``X64``
 
 ``64-bit``
 """
-RETFW_IMM16: Code = 414 # type: ignore
+RETFW_IMM16: int = 414
 """
 ``RETF imm16``
 
 ``o16 CA iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RETFD_IMM16: Code = 415 # type: ignore
+RETFD_IMM16: int = 415
 """
 ``RETF imm16``
 
 ``o32 CA iw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RETFQ_IMM16: Code = 416 # type: ignore
+RETFQ_IMM16: int = 416
 """
 ``RETF imm16``
 
 ``o64 CA iw``
 
 ``X64``
 
 ``64-bit``
 """
-RETFW: Code = 417 # type: ignore
+RETFW: int = 417
 """
 ``RETF``
 
 ``o16 CB``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RETFD: Code = 418 # type: ignore
+RETFD: int = 418
 """
 ``RETF``
 
 ``o32 CB``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RETFQ: Code = 419 # type: ignore
+RETFQ: int = 419
 """
 ``RETF``
 
 ``o64 CB``
 
 ``X64``
 
 ``64-bit``
 """
-INT3: Code = 420 # type: ignore
+INT3: int = 420
 """
 ``INT3``
 
 ``CC``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-INT_IMM8: Code = 421 # type: ignore
+INT_IMM8: int = 421
 """
 ``INT imm8``
 
 ``CD ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-INTO: Code = 422 # type: ignore
+INTO: int = 422
 """
 ``INTO``
 
 ``CE``
 
 ``8086+``
 
 ``16/32-bit``
 """
-IRETW: Code = 423 # type: ignore
+IRETW: int = 423
 """
 ``IRET``
 
 ``o16 CF``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IRETD: Code = 424 # type: ignore
+IRETD: int = 424
 """
 ``IRETD``
 
 ``o32 CF``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IRETQ: Code = 425 # type: ignore
+IRETQ: int = 425
 """
 ``IRETQ``
 
 ``o64 CF``
 
 ``X64``
 
 ``64-bit``
 """
-ROL_RM8_1: Code = 426 # type: ignore
+ROL_RM8_1: int = 426
 """
 ``ROL r/m8, 1``
 
 ``D0 /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROR_RM8_1: Code = 427 # type: ignore
+ROR_RM8_1: int = 427
 """
 ``ROR r/m8, 1``
 
 ``D0 /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCL_RM8_1: Code = 428 # type: ignore
+RCL_RM8_1: int = 428
 """
 ``RCL r/m8, 1``
 
 ``D0 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCR_RM8_1: Code = 429 # type: ignore
+RCR_RM8_1: int = 429
 """
 ``RCR r/m8, 1``
 
 ``D0 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHL_RM8_1: Code = 430 # type: ignore
+SHL_RM8_1: int = 430
 """
 ``SHL r/m8, 1``
 
 ``D0 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHR_RM8_1: Code = 431 # type: ignore
+SHR_RM8_1: int = 431
 """
 ``SHR r/m8, 1``
 
 ``D0 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAL_RM8_1: Code = 432 # type: ignore
+SAL_RM8_1: int = 432
 """
 ``SAL r/m8, 1``
 
 ``D0 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAR_RM8_1: Code = 433 # type: ignore
+SAR_RM8_1: int = 433
 """
 ``SAR r/m8, 1``
 
 ``D0 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROL_RM16_1: Code = 434 # type: ignore
+ROL_RM16_1: int = 434
 """
 ``ROL r/m16, 1``
 
 ``o16 D1 /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROL_RM32_1: Code = 435 # type: ignore
+ROL_RM32_1: int = 435
 """
 ``ROL r/m32, 1``
 
 ``o32 D1 /0``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROL_RM64_1: Code = 436 # type: ignore
+ROL_RM64_1: int = 436
 """
 ``ROL r/m64, 1``
 
 ``o64 D1 /0``
 
 ``X64``
 
 ``64-bit``
 """
-ROR_RM16_1: Code = 437 # type: ignore
+ROR_RM16_1: int = 437
 """
 ``ROR r/m16, 1``
 
 ``o16 D1 /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROR_RM32_1: Code = 438 # type: ignore
+ROR_RM32_1: int = 438
 """
 ``ROR r/m32, 1``
 
 ``o32 D1 /1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROR_RM64_1: Code = 439 # type: ignore
+ROR_RM64_1: int = 439
 """
 ``ROR r/m64, 1``
 
 ``o64 D1 /1``
 
 ``X64``
 
 ``64-bit``
 """
-RCL_RM16_1: Code = 440 # type: ignore
+RCL_RM16_1: int = 440
 """
 ``RCL r/m16, 1``
 
 ``o16 D1 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCL_RM32_1: Code = 441 # type: ignore
+RCL_RM32_1: int = 441
 """
 ``RCL r/m32, 1``
 
 ``o32 D1 /2``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCL_RM64_1: Code = 442 # type: ignore
+RCL_RM64_1: int = 442
 """
 ``RCL r/m64, 1``
 
 ``o64 D1 /2``
 
 ``X64``
 
 ``64-bit``
 """
-RCR_RM16_1: Code = 443 # type: ignore
+RCR_RM16_1: int = 443
 """
 ``RCR r/m16, 1``
 
 ``o16 D1 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCR_RM32_1: Code = 444 # type: ignore
+RCR_RM32_1: int = 444
 """
 ``RCR r/m32, 1``
 
 ``o32 D1 /3``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCR_RM64_1: Code = 445 # type: ignore
+RCR_RM64_1: int = 445
 """
 ``RCR r/m64, 1``
 
 ``o64 D1 /3``
 
 ``X64``
 
 ``64-bit``
 """
-SHL_RM16_1: Code = 446 # type: ignore
+SHL_RM16_1: int = 446
 """
 ``SHL r/m16, 1``
 
 ``o16 D1 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHL_RM32_1: Code = 447 # type: ignore
+SHL_RM32_1: int = 447
 """
 ``SHL r/m32, 1``
 
 ``o32 D1 /4``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHL_RM64_1: Code = 448 # type: ignore
+SHL_RM64_1: int = 448
 """
 ``SHL r/m64, 1``
 
 ``o64 D1 /4``
 
 ``X64``
 
 ``64-bit``
 """
-SHR_RM16_1: Code = 449 # type: ignore
+SHR_RM16_1: int = 449
 """
 ``SHR r/m16, 1``
 
 ``o16 D1 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHR_RM32_1: Code = 450 # type: ignore
+SHR_RM32_1: int = 450
 """
 ``SHR r/m32, 1``
 
 ``o32 D1 /5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHR_RM64_1: Code = 451 # type: ignore
+SHR_RM64_1: int = 451
 """
 ``SHR r/m64, 1``
 
 ``o64 D1 /5``
 
 ``X64``
 
 ``64-bit``
 """
-SAL_RM16_1: Code = 452 # type: ignore
+SAL_RM16_1: int = 452
 """
 ``SAL r/m16, 1``
 
 ``o16 D1 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAL_RM32_1: Code = 453 # type: ignore
+SAL_RM32_1: int = 453
 """
 ``SAL r/m32, 1``
 
 ``o32 D1 /6``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAL_RM64_1: Code = 454 # type: ignore
+SAL_RM64_1: int = 454
 """
 ``SAL r/m64, 1``
 
 ``o64 D1 /6``
 
 ``X64``
 
 ``64-bit``
 """
-SAR_RM16_1: Code = 455 # type: ignore
+SAR_RM16_1: int = 455
 """
 ``SAR r/m16, 1``
 
 ``o16 D1 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAR_RM32_1: Code = 456 # type: ignore
+SAR_RM32_1: int = 456
 """
 ``SAR r/m32, 1``
 
 ``o32 D1 /7``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAR_RM64_1: Code = 457 # type: ignore
+SAR_RM64_1: int = 457
 """
 ``SAR r/m64, 1``
 
 ``o64 D1 /7``
 
 ``X64``
 
 ``64-bit``
 """
-ROL_RM8_CL: Code = 458 # type: ignore
+ROL_RM8_CL: int = 458
 """
 ``ROL r/m8, CL``
 
 ``D2 /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROR_RM8_CL: Code = 459 # type: ignore
+ROR_RM8_CL: int = 459
 """
 ``ROR r/m8, CL``
 
 ``D2 /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCL_RM8_CL: Code = 460 # type: ignore
+RCL_RM8_CL: int = 460
 """
 ``RCL r/m8, CL``
 
 ``D2 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCR_RM8_CL: Code = 461 # type: ignore
+RCR_RM8_CL: int = 461
 """
 ``RCR r/m8, CL``
 
 ``D2 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHL_RM8_CL: Code = 462 # type: ignore
+SHL_RM8_CL: int = 462
 """
 ``SHL r/m8, CL``
 
 ``D2 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHR_RM8_CL: Code = 463 # type: ignore
+SHR_RM8_CL: int = 463
 """
 ``SHR r/m8, CL``
 
 ``D2 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAL_RM8_CL: Code = 464 # type: ignore
+SAL_RM8_CL: int = 464
 """
 ``SAL r/m8, CL``
 
 ``D2 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAR_RM8_CL: Code = 465 # type: ignore
+SAR_RM8_CL: int = 465
 """
 ``SAR r/m8, CL``
 
 ``D2 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROL_RM16_CL: Code = 466 # type: ignore
+ROL_RM16_CL: int = 466
 """
 ``ROL r/m16, CL``
 
 ``o16 D3 /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROL_RM32_CL: Code = 467 # type: ignore
+ROL_RM32_CL: int = 467
 """
 ``ROL r/m32, CL``
 
 ``o32 D3 /0``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROL_RM64_CL: Code = 468 # type: ignore
+ROL_RM64_CL: int = 468
 """
 ``ROL r/m64, CL``
 
 ``o64 D3 /0``
 
 ``X64``
 
 ``64-bit``
 """
-ROR_RM16_CL: Code = 469 # type: ignore
+ROR_RM16_CL: int = 469
 """
 ``ROR r/m16, CL``
 
 ``o16 D3 /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-ROR_RM32_CL: Code = 470 # type: ignore
+ROR_RM32_CL: int = 470
 """
 ``ROR r/m32, CL``
 
 ``o32 D3 /1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-ROR_RM64_CL: Code = 471 # type: ignore
+ROR_RM64_CL: int = 471
 """
 ``ROR r/m64, CL``
 
 ``o64 D3 /1``
 
 ``X64``
 
 ``64-bit``
 """
-RCL_RM16_CL: Code = 472 # type: ignore
+RCL_RM16_CL: int = 472
 """
 ``RCL r/m16, CL``
 
 ``o16 D3 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCL_RM32_CL: Code = 473 # type: ignore
+RCL_RM32_CL: int = 473
 """
 ``RCL r/m32, CL``
 
 ``o32 D3 /2``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCL_RM64_CL: Code = 474 # type: ignore
+RCL_RM64_CL: int = 474
 """
 ``RCL r/m64, CL``
 
 ``o64 D3 /2``
 
 ``X64``
 
 ``64-bit``
 """
-RCR_RM16_CL: Code = 475 # type: ignore
+RCR_RM16_CL: int = 475
 """
 ``RCR r/m16, CL``
 
 ``o16 D3 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-RCR_RM32_CL: Code = 476 # type: ignore
+RCR_RM32_CL: int = 476
 """
 ``RCR r/m32, CL``
 
 ``o32 D3 /3``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-RCR_RM64_CL: Code = 477 # type: ignore
+RCR_RM64_CL: int = 477
 """
 ``RCR r/m64, CL``
 
 ``o64 D3 /3``
 
 ``X64``
 
 ``64-bit``
 """
-SHL_RM16_CL: Code = 478 # type: ignore
+SHL_RM16_CL: int = 478
 """
 ``SHL r/m16, CL``
 
 ``o16 D3 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHL_RM32_CL: Code = 479 # type: ignore
+SHL_RM32_CL: int = 479
 """
 ``SHL r/m32, CL``
 
 ``o32 D3 /4``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHL_RM64_CL: Code = 480 # type: ignore
+SHL_RM64_CL: int = 480
 """
 ``SHL r/m64, CL``
 
 ``o64 D3 /4``
 
 ``X64``
 
 ``64-bit``
 """
-SHR_RM16_CL: Code = 481 # type: ignore
+SHR_RM16_CL: int = 481
 """
 ``SHR r/m16, CL``
 
 ``o16 D3 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SHR_RM32_CL: Code = 482 # type: ignore
+SHR_RM32_CL: int = 482
 """
 ``SHR r/m32, CL``
 
 ``o32 D3 /5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHR_RM64_CL: Code = 483 # type: ignore
+SHR_RM64_CL: int = 483
 """
 ``SHR r/m64, CL``
 
 ``o64 D3 /5``
 
 ``X64``
 
 ``64-bit``
 """
-SAL_RM16_CL: Code = 484 # type: ignore
+SAL_RM16_CL: int = 484
 """
 ``SAL r/m16, CL``
 
 ``o16 D3 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAL_RM32_CL: Code = 485 # type: ignore
+SAL_RM32_CL: int = 485
 """
 ``SAL r/m32, CL``
 
 ``o32 D3 /6``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAL_RM64_CL: Code = 486 # type: ignore
+SAL_RM64_CL: int = 486
 """
 ``SAL r/m64, CL``
 
 ``o64 D3 /6``
 
 ``X64``
 
 ``64-bit``
 """
-SAR_RM16_CL: Code = 487 # type: ignore
+SAR_RM16_CL: int = 487
 """
 ``SAR r/m16, CL``
 
 ``o16 D3 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-SAR_RM32_CL: Code = 488 # type: ignore
+SAR_RM32_CL: int = 488
 """
 ``SAR r/m32, CL``
 
 ``o32 D3 /7``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SAR_RM64_CL: Code = 489 # type: ignore
+SAR_RM64_CL: int = 489
 """
 ``SAR r/m64, CL``
 
 ``o64 D3 /7``
 
 ``X64``
 
 ``64-bit``
 """
-AAM_IMM8: Code = 490 # type: ignore
+AAM_IMM8: int = 490
 """
 ``AAM imm8``
 
 ``D4 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-AAD_IMM8: Code = 491 # type: ignore
+AAD_IMM8: int = 491
 """
 ``AAD imm8``
 
 ``D5 ib``
 
 ``8086+``
 
 ``16/32-bit``
 """
-SALC: Code = 492 # type: ignore
+SALC: int = 492
 """
 ``SALC``
 
 ``D6``
 
 ``8086+``
 
 ``16/32-bit``
 """
-XLAT_M8: Code = 493 # type: ignore
+XLAT_M8: int = 493
 """
 ``XLATB``
 
 ``D7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-FADD_M32FP: Code = 494 # type: ignore
+FADD_M32FP: int = 494
 """
 ``FADD m32fp``
 
 ``D8 /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FMUL_M32FP: Code = 495 # type: ignore
+FMUL_M32FP: int = 495
 """
 ``FMUL m32fp``
 
 ``D8 /1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOM_M32FP: Code = 496 # type: ignore
+FCOM_M32FP: int = 496
 """
 ``FCOM m32fp``
 
 ``D8 /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMP_M32FP: Code = 497 # type: ignore
+FCOMP_M32FP: int = 497
 """
 ``FCOMP m32fp``
 
 ``D8 /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUB_M32FP: Code = 498 # type: ignore
+FSUB_M32FP: int = 498
 """
 ``FSUB m32fp``
 
 ``D8 /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBR_M32FP: Code = 499 # type: ignore
+FSUBR_M32FP: int = 499
 """
 ``FSUBR m32fp``
 
 ``D8 /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIV_M32FP: Code = 500 # type: ignore
+FDIV_M32FP: int = 500
 """
 ``FDIV m32fp``
 
 ``D8 /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVR_M32FP: Code = 501 # type: ignore
+FDIVR_M32FP: int = 501
 """
 ``FDIVR m32fp``
 
 ``D8 /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FADD_ST0_STI: Code = 502 # type: ignore
+FADD_ST0_STI: int = 502
 """
 ``FADD ST(0), ST(i)``
 
 ``D8 C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FMUL_ST0_STI: Code = 503 # type: ignore
+FMUL_ST0_STI: int = 503
 """
 ``FMUL ST(0), ST(i)``
 
 ``D8 C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOM_ST0_STI: Code = 504 # type: ignore
+FCOM_ST0_STI: int = 504
 """
 ``FCOM ST(i)``
 
 ``D8 D0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMP_ST0_STI: Code = 505 # type: ignore
+FCOMP_ST0_STI: int = 505
 """
 ``FCOMP ST(i)``
 
 ``D8 D8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUB_ST0_STI: Code = 506 # type: ignore
+FSUB_ST0_STI: int = 506
 """
 ``FSUB ST(0), ST(i)``
 
 ``D8 E0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBR_ST0_STI: Code = 507 # type: ignore
+FSUBR_ST0_STI: int = 507
 """
 ``FSUBR ST(0), ST(i)``
 
 ``D8 E8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIV_ST0_STI: Code = 508 # type: ignore
+FDIV_ST0_STI: int = 508
 """
 ``FDIV ST(0), ST(i)``
 
 ``D8 F0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVR_ST0_STI: Code = 509 # type: ignore
+FDIVR_ST0_STI: int = 509
 """
 ``FDIVR ST(0), ST(i)``
 
 ``D8 F8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLD_M32FP: Code = 510 # type: ignore
+FLD_M32FP: int = 510
 """
 ``FLD m32fp``
 
 ``D9 /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FST_M32FP: Code = 511 # type: ignore
+FST_M32FP: int = 511
 """
 ``FST m32fp``
 
 ``D9 /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_M32FP: Code = 512 # type: ignore
+FSTP_M32FP: int = 512
 """
 ``FSTP m32fp``
 
 ``D9 /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDENV_M14BYTE: Code = 513 # type: ignore
+FLDENV_M14BYTE: int = 513
 """
 ``FLDENV m14byte``
 
 ``o16 D9 /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDENV_M28BYTE: Code = 514 # type: ignore
+FLDENV_M28BYTE: int = 514
 """
 ``FLDENV m28byte``
 
 ``o32 D9 /4``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FLDCW_M2BYTE: Code = 515 # type: ignore
+FLDCW_M2BYTE: int = 515
 """
 ``FLDCW m2byte``
 
 ``D9 /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNSTENV_M14BYTE: Code = 516 # type: ignore
+FNSTENV_M14BYTE: int = 516
 """
 ``FNSTENV m14byte``
 
 ``o16 D9 /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTENV_M14BYTE: Code = 517 # type: ignore
+FSTENV_M14BYTE: int = 517
 """
 ``FSTENV m14byte``
 
 ``9B o16 D9 /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNSTENV_M28BYTE: Code = 518 # type: ignore
+FNSTENV_M28BYTE: int = 518
 """
 ``FNSTENV m28byte``
 
 ``o32 D9 /6``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FSTENV_M28BYTE: Code = 519 # type: ignore
+FSTENV_M28BYTE: int = 519
 """
 ``FSTENV m28byte``
 
 ``9B o32 D9 /6``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FNSTCW_M2BYTE: Code = 520 # type: ignore
+FNSTCW_M2BYTE: int = 520
 """
 ``FNSTCW m2byte``
 
 ``D9 /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTCW_M2BYTE: Code = 521 # type: ignore
+FSTCW_M2BYTE: int = 521
 """
 ``FSTCW m2byte``
 
 ``9B D9 /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLD_STI: Code = 522 # type: ignore
+FLD_STI: int = 522
 """
 ``FLD ST(i)``
 
 ``D9 C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FXCH_ST0_STI: Code = 523 # type: ignore
+FXCH_ST0_STI: int = 523
 """
 ``FXCH ST(i)``
 
 ``D9 C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNOP: Code = 524 # type: ignore
+FNOP: int = 524
 """
 ``FNOP``
 
 ``D9 D0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTPNCE_STI: Code = 525 # type: ignore
+FSTPNCE_STI: int = 525
 """
 ``FSTPNCE ST(i)``
 
 ``D9 D8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCHS: Code = 526 # type: ignore
+FCHS: int = 526
 """
 ``FCHS``
 
 ``D9 E0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FABS: Code = 527 # type: ignore
+FABS: int = 527
 """
 ``FABS``
 
 ``D9 E1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FTST: Code = 528 # type: ignore
+FTST: int = 528
 """
 ``FTST``
 
 ``D9 E4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FXAM: Code = 529 # type: ignore
+FXAM: int = 529
 """
 ``FXAM``
 
 ``D9 E5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLD1: Code = 530 # type: ignore
+FLD1: int = 530
 """
 ``FLD1``
 
 ``D9 E8``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDL2T: Code = 531 # type: ignore
+FLDL2T: int = 531
 """
 ``FLDL2T``
 
 ``D9 E9``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDL2E: Code = 532 # type: ignore
+FLDL2E: int = 532
 """
 ``FLDL2E``
 
 ``D9 EA``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDPI: Code = 533 # type: ignore
+FLDPI: int = 533
 """
 ``FLDPI``
 
 ``D9 EB``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDLG2: Code = 534 # type: ignore
+FLDLG2: int = 534
 """
 ``FLDLG2``
 
 ``D9 EC``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDLN2: Code = 535 # type: ignore
+FLDLN2: int = 535
 """
 ``FLDLN2``
 
 ``D9 ED``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLDZ: Code = 536 # type: ignore
+FLDZ: int = 536
 """
 ``FLDZ``
 
 ``D9 EE``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-F2XM1: Code = 537 # type: ignore
+F2XM1: int = 537
 """
 ``F2XM1``
 
 ``D9 F0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FYL2X: Code = 538 # type: ignore
+FYL2X: int = 538
 """
 ``FYL2X``
 
 ``D9 F1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FPTAN: Code = 539 # type: ignore
+FPTAN: int = 539
 """
 ``FPTAN``
 
 ``D9 F2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FPATAN: Code = 540 # type: ignore
+FPATAN: int = 540
 """
 ``FPATAN``
 
 ``D9 F3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FXTRACT: Code = 541 # type: ignore
+FXTRACT: int = 541
 """
 ``FXTRACT``
 
 ``D9 F4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FPREM1: Code = 542 # type: ignore
+FPREM1: int = 542
 """
 ``FPREM1``
 
 ``D9 F5``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FDECSTP: Code = 543 # type: ignore
+FDECSTP: int = 543
 """
 ``FDECSTP``
 
 ``D9 F6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FINCSTP: Code = 544 # type: ignore
+FINCSTP: int = 544
 """
 ``FINCSTP``
 
 ``D9 F7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FPREM: Code = 545 # type: ignore
+FPREM: int = 545
 """
 ``FPREM``
 
 ``D9 F8``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FYL2XP1: Code = 546 # type: ignore
+FYL2XP1: int = 546
 """
 ``FYL2XP1``
 
 ``D9 F9``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSQRT: Code = 547 # type: ignore
+FSQRT: int = 547
 """
 ``FSQRT``
 
 ``D9 FA``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSINCOS: Code = 548 # type: ignore
+FSINCOS: int = 548
 """
 ``FSINCOS``
 
 ``D9 FB``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FRNDINT: Code = 549 # type: ignore
+FRNDINT: int = 549
 """
 ``FRNDINT``
 
 ``D9 FC``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSCALE: Code = 550 # type: ignore
+FSCALE: int = 550
 """
 ``FSCALE``
 
 ``D9 FD``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSIN: Code = 551 # type: ignore
+FSIN: int = 551
 """
 ``FSIN``
 
 ``D9 FE``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FCOS: Code = 552 # type: ignore
+FCOS: int = 552
 """
 ``FCOS``
 
 ``D9 FF``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FIADD_M32INT: Code = 553 # type: ignore
+FIADD_M32INT: int = 553
 """
 ``FIADD m32int``
 
 ``DA /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIMUL_M32INT: Code = 554 # type: ignore
+FIMUL_M32INT: int = 554
 """
 ``FIMUL m32int``
 
 ``DA /1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FICOM_M32INT: Code = 555 # type: ignore
+FICOM_M32INT: int = 555
 """
 ``FICOM m32int``
 
 ``DA /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FICOMP_M32INT: Code = 556 # type: ignore
+FICOMP_M32INT: int = 556
 """
 ``FICOMP m32int``
 
 ``DA /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISUB_M32INT: Code = 557 # type: ignore
+FISUB_M32INT: int = 557
 """
 ``FISUB m32int``
 
 ``DA /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISUBR_M32INT: Code = 558 # type: ignore
+FISUBR_M32INT: int = 558
 """
 ``FISUBR m32int``
 
 ``DA /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIDIV_M32INT: Code = 559 # type: ignore
+FIDIV_M32INT: int = 559
 """
 ``FIDIV m32int``
 
 ``DA /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIDIVR_M32INT: Code = 560 # type: ignore
+FIDIVR_M32INT: int = 560
 """
 ``FIDIVR m32int``
 
 ``DA /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCMOVB_ST0_STI: Code = 561 # type: ignore
+FCMOVB_ST0_STI: int = 561
 """
 ``FCMOVB ST(0), ST(i)``
 
 ``DA C0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVE_ST0_STI: Code = 562 # type: ignore
+FCMOVE_ST0_STI: int = 562
 """
 ``FCMOVE ST(0), ST(i)``
 
 ``DA C8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVBE_ST0_STI: Code = 563 # type: ignore
+FCMOVBE_ST0_STI: int = 563
 """
 ``FCMOVBE ST(0), ST(i)``
 
 ``DA D0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVU_ST0_STI: Code = 564 # type: ignore
+FCMOVU_ST0_STI: int = 564
 """
 ``FCMOVU ST(0), ST(i)``
 
 ``DA D8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FUCOMPP: Code = 565 # type: ignore
+FUCOMPP: int = 565
 """
 ``FUCOMPP``
 
 ``DA E9``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FILD_M32INT: Code = 566 # type: ignore
+FILD_M32INT: int = 566
 """
 ``FILD m32int``
 
 ``DB /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTTP_M32INT: Code = 567 # type: ignore
+FISTTP_M32INT: int = 567
 """
 ``FISTTP m32int``
 
 ``DB /1``
 
 ``8087+ and SSE3``
 
 ``16/32/64-bit``
 """
-FIST_M32INT: Code = 568 # type: ignore
+FIST_M32INT: int = 568
 """
 ``FIST m32int``
 
 ``DB /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTP_M32INT: Code = 569 # type: ignore
+FISTP_M32INT: int = 569
 """
 ``FISTP m32int``
 
 ``DB /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLD_M80FP: Code = 570 # type: ignore
+FLD_M80FP: int = 570
 """
 ``FLD m80fp``
 
 ``DB /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_M80FP: Code = 571 # type: ignore
+FSTP_M80FP: int = 571
 """
 ``FSTP m80fp``
 
 ``DB /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCMOVNB_ST0_STI: Code = 572 # type: ignore
+FCMOVNB_ST0_STI: int = 572
 """
 ``FCMOVNB ST(0), ST(i)``
 
 ``DB C0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVNE_ST0_STI: Code = 573 # type: ignore
+FCMOVNE_ST0_STI: int = 573
 """
 ``FCMOVNE ST(0), ST(i)``
 
 ``DB C8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVNBE_ST0_STI: Code = 574 # type: ignore
+FCMOVNBE_ST0_STI: int = 574
 """
 ``FCMOVNBE ST(0), ST(i)``
 
 ``DB D0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCMOVNU_ST0_STI: Code = 575 # type: ignore
+FCMOVNU_ST0_STI: int = 575
 """
 ``FCMOVNU ST(0), ST(i)``
 
 ``DB D8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FNENI: Code = 576 # type: ignore
+FNENI: int = 576
 """
 ``FNENI``
 
 ``DB E0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FENI: Code = 577 # type: ignore
+FENI: int = 577
 """
 ``FENI``
 
 ``9B DB E0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNDISI: Code = 578 # type: ignore
+FNDISI: int = 578
 """
 ``FNDISI``
 
 ``DB E1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDISI: Code = 579 # type: ignore
+FDISI: int = 579
 """
 ``FDISI``
 
 ``9B DB E1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNCLEX: Code = 580 # type: ignore
+FNCLEX: int = 580
 """
 ``FNCLEX``
 
 ``DB E2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCLEX: Code = 581 # type: ignore
+FCLEX: int = 581
 """
 ``FCLEX``
 
 ``9B DB E2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNINIT: Code = 582 # type: ignore
+FNINIT: int = 582
 """
 ``FNINIT``
 
 ``DB E3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FINIT: Code = 583 # type: ignore
+FINIT: int = 583
 """
 ``FINIT``
 
 ``9B DB E3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNSETPM: Code = 584 # type: ignore
+FNSETPM: int = 584
 """
 ``FNSETPM``
 
 ``DB E4``
 
 ``287+``
 
 ``16/32/64-bit``
 """
-FSETPM: Code = 585 # type: ignore
+FSETPM: int = 585
 """
 ``FSETPM``
 
 ``9B DB E4``
 
 ``287+``
 
 ``16/32/64-bit``
 """
-FRSTPM: Code = 586 # type: ignore
+FRSTPM: int = 586
 """
 ``FRSTPM``
 
 ``DB E5``
 
 ``287 XL``
 
 ``16/32-bit``
 """
-FUCOMI_ST0_STI: Code = 587 # type: ignore
+FUCOMI_ST0_STI: int = 587
 """
 ``FUCOMI ST, ST(i)``
 
 ``DB E8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCOMI_ST0_STI: Code = 588 # type: ignore
+FCOMI_ST0_STI: int = 588
 """
 ``FCOMI ST, ST(i)``
 
 ``DB F0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FADD_M64FP: Code = 589 # type: ignore
+FADD_M64FP: int = 589
 """
 ``FADD m64fp``
 
 ``DC /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FMUL_M64FP: Code = 590 # type: ignore
+FMUL_M64FP: int = 590
 """
 ``FMUL m64fp``
 
 ``DC /1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOM_M64FP: Code = 591 # type: ignore
+FCOM_M64FP: int = 591
 """
 ``FCOM m64fp``
 
 ``DC /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMP_M64FP: Code = 592 # type: ignore
+FCOMP_M64FP: int = 592
 """
 ``FCOMP m64fp``
 
 ``DC /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUB_M64FP: Code = 593 # type: ignore
+FSUB_M64FP: int = 593
 """
 ``FSUB m64fp``
 
 ``DC /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBR_M64FP: Code = 594 # type: ignore
+FSUBR_M64FP: int = 594
 """
 ``FSUBR m64fp``
 
 ``DC /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIV_M64FP: Code = 595 # type: ignore
+FDIV_M64FP: int = 595
 """
 ``FDIV m64fp``
 
 ``DC /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVR_M64FP: Code = 596 # type: ignore
+FDIVR_M64FP: int = 596
 """
 ``FDIVR m64fp``
 
 ``DC /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FADD_STI_ST0: Code = 597 # type: ignore
+FADD_STI_ST0: int = 597
 """
 ``FADD ST(i), ST(0)``
 
 ``DC C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FMUL_STI_ST0: Code = 598 # type: ignore
+FMUL_STI_ST0: int = 598
 """
 ``FMUL ST(i), ST(0)``
 
 ``DC C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOM_ST0_STI_DCD0: Code = 599 # type: ignore
+FCOM_ST0_STI_DCD0: int = 599
 """
 ``FCOM ST(i)``
 
 ``DC D0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMP_ST0_STI_DCD8: Code = 600 # type: ignore
+FCOMP_ST0_STI_DCD8: int = 600
 """
 ``FCOMP ST(i)``
 
 ``DC D8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBR_STI_ST0: Code = 601 # type: ignore
+FSUBR_STI_ST0: int = 601
 """
 ``FSUBR ST(i), ST(0)``
 
 ``DC E0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUB_STI_ST0: Code = 602 # type: ignore
+FSUB_STI_ST0: int = 602
 """
 ``FSUB ST(i), ST(0)``
 
 ``DC E8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVR_STI_ST0: Code = 603 # type: ignore
+FDIVR_STI_ST0: int = 603
 """
 ``FDIVR ST(i), ST(0)``
 
 ``DC F0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIV_STI_ST0: Code = 604 # type: ignore
+FDIV_STI_ST0: int = 604
 """
 ``FDIV ST(i), ST(0)``
 
 ``DC F8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FLD_M64FP: Code = 605 # type: ignore
+FLD_M64FP: int = 605
 """
 ``FLD m64fp``
 
 ``DD /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTTP_M64INT: Code = 606 # type: ignore
+FISTTP_M64INT: int = 606
 """
 ``FISTTP m64int``
 
 ``DD /1``
 
 ``8087+ and SSE3``
 
 ``16/32/64-bit``
 """
-FST_M64FP: Code = 607 # type: ignore
+FST_M64FP: int = 607
 """
 ``FST m64fp``
 
 ``DD /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_M64FP: Code = 608 # type: ignore
+FSTP_M64FP: int = 608
 """
 ``FSTP m64fp``
 
 ``DD /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FRSTOR_M94BYTE: Code = 609 # type: ignore
+FRSTOR_M94BYTE: int = 609
 """
 ``FRSTOR m94byte``
 
 ``o16 DD /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FRSTOR_M108BYTE: Code = 610 # type: ignore
+FRSTOR_M108BYTE: int = 610
 """
 ``FRSTOR m108byte``
 
 ``o32 DD /4``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FNSAVE_M94BYTE: Code = 611 # type: ignore
+FNSAVE_M94BYTE: int = 611
 """
 ``FNSAVE m94byte``
 
 ``o16 DD /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSAVE_M94BYTE: Code = 612 # type: ignore
+FSAVE_M94BYTE: int = 612
 """
 ``FSAVE m94byte``
 
 ``9B o16 DD /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNSAVE_M108BYTE: Code = 613 # type: ignore
+FNSAVE_M108BYTE: int = 613
 """
 ``FNSAVE m108byte``
 
 ``o32 DD /6``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FSAVE_M108BYTE: Code = 614 # type: ignore
+FSAVE_M108BYTE: int = 614
 """
 ``FSAVE m108byte``
 
 ``9B o32 DD /6``
 
 ``387+``
 
 ``16/32/64-bit``
 """
-FNSTSW_M2BYTE: Code = 615 # type: ignore
+FNSTSW_M2BYTE: int = 615
 """
 ``FNSTSW m2byte``
 
 ``DD /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTSW_M2BYTE: Code = 616 # type: ignore
+FSTSW_M2BYTE: int = 616
 """
 ``FSTSW m2byte``
 
 ``9B DD /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FFREE_STI: Code = 617 # type: ignore
+FFREE_STI: int = 617
 """
 ``FFREE ST(i)``
 
 ``DD C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FXCH_ST0_STI_DDC8: Code = 618 # type: ignore
+FXCH_ST0_STI_DDC8: int = 618
 """
 ``FXCH ST(i)``
 
 ``DD C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FST_STI: Code = 619 # type: ignore
+FST_STI: int = 619
 """
 ``FST ST(i)``
 
 ``DD D0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_STI: Code = 620 # type: ignore
+FSTP_STI: int = 620
 """
 ``FSTP ST(i)``
 
 ``DD D8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FUCOM_ST0_STI: Code = 621 # type: ignore
+FUCOM_ST0_STI: int = 621
 """
 ``FUCOM ST(i)``
 
 ``DD E0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FUCOMP_ST0_STI: Code = 622 # type: ignore
+FUCOMP_ST0_STI: int = 622
 """
 ``FUCOMP ST(i)``
 
 ``DD E8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIADD_M16INT: Code = 623 # type: ignore
+FIADD_M16INT: int = 623
 """
 ``FIADD m16int``
 
 ``DE /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIMUL_M16INT: Code = 624 # type: ignore
+FIMUL_M16INT: int = 624
 """
 ``FIMUL m16int``
 
 ``DE /1``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FICOM_M16INT: Code = 625 # type: ignore
+FICOM_M16INT: int = 625
 """
 ``FICOM m16int``
 
 ``DE /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FICOMP_M16INT: Code = 626 # type: ignore
+FICOMP_M16INT: int = 626
 """
 ``FICOMP m16int``
 
 ``DE /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISUB_M16INT: Code = 627 # type: ignore
+FISUB_M16INT: int = 627
 """
 ``FISUB m16int``
 
 ``DE /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISUBR_M16INT: Code = 628 # type: ignore
+FISUBR_M16INT: int = 628
 """
 ``FISUBR m16int``
 
 ``DE /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIDIV_M16INT: Code = 629 # type: ignore
+FIDIV_M16INT: int = 629
 """
 ``FIDIV m16int``
 
 ``DE /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FIDIVR_M16INT: Code = 630 # type: ignore
+FIDIVR_M16INT: int = 630
 """
 ``FIDIVR m16int``
 
 ``DE /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FADDP_STI_ST0: Code = 631 # type: ignore
+FADDP_STI_ST0: int = 631
 """
 ``FADDP ST(i), ST(0)``
 
 ``DE C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FMULP_STI_ST0: Code = 632 # type: ignore
+FMULP_STI_ST0: int = 632
 """
 ``FMULP ST(i), ST(0)``
 
 ``DE C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMP_ST0_STI_DED0: Code = 633 # type: ignore
+FCOMP_ST0_STI_DED0: int = 633
 """
 ``FCOMP ST(i)``
 
 ``DE D0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FCOMPP: Code = 634 # type: ignore
+FCOMPP: int = 634
 """
 ``FCOMPP``
 
 ``DE D9``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBRP_STI_ST0: Code = 635 # type: ignore
+FSUBRP_STI_ST0: int = 635
 """
 ``FSUBRP ST(i), ST(0)``
 
 ``DE E0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSUBP_STI_ST0: Code = 636 # type: ignore
+FSUBP_STI_ST0: int = 636
 """
 ``FSUBP ST(i), ST(0)``
 
 ``DE E8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVRP_STI_ST0: Code = 637 # type: ignore
+FDIVRP_STI_ST0: int = 637
 """
 ``FDIVRP ST(i), ST(0)``
 
 ``DE F0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FDIVP_STI_ST0: Code = 638 # type: ignore
+FDIVP_STI_ST0: int = 638
 """
 ``FDIVP ST(i), ST(0)``
 
 ``DE F8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FILD_M16INT: Code = 639 # type: ignore
+FILD_M16INT: int = 639
 """
 ``FILD m16int``
 
 ``DF /0``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTTP_M16INT: Code = 640 # type: ignore
+FISTTP_M16INT: int = 640
 """
 ``FISTTP m16int``
 
 ``DF /1``
 
 ``8087+ and SSE3``
 
 ``16/32/64-bit``
 """
-FIST_M16INT: Code = 641 # type: ignore
+FIST_M16INT: int = 641
 """
 ``FIST m16int``
 
 ``DF /2``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTP_M16INT: Code = 642 # type: ignore
+FISTP_M16INT: int = 642
 """
 ``FISTP m16int``
 
 ``DF /3``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FBLD_M80BCD: Code = 643 # type: ignore
+FBLD_M80BCD: int = 643
 """
 ``FBLD m80bcd``
 
 ``DF /4``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FILD_M64INT: Code = 644 # type: ignore
+FILD_M64INT: int = 644
 """
 ``FILD m64int``
 
 ``DF /5``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FBSTP_M80BCD: Code = 645 # type: ignore
+FBSTP_M80BCD: int = 645
 """
 ``FBSTP m80bcd``
 
 ``DF /6``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FISTP_M64INT: Code = 646 # type: ignore
+FISTP_M64INT: int = 646
 """
 ``FISTP m64int``
 
 ``DF /7``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FFREEP_STI: Code = 647 # type: ignore
+FFREEP_STI: int = 647
 """
 ``FFREEP ST(i)``
 
 ``DF C0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FXCH_ST0_STI_DFC8: Code = 648 # type: ignore
+FXCH_ST0_STI_DFC8: int = 648
 """
 ``FXCH ST(i)``
 
 ``DF C8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_STI_DFD0: Code = 649 # type: ignore
+FSTP_STI_DFD0: int = 649
 """
 ``FSTP ST(i)``
 
 ``DF D0+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FSTP_STI_DFD8: Code = 650 # type: ignore
+FSTP_STI_DFD8: int = 650
 """
 ``FSTP ST(i)``
 
 ``DF D8+i``
 
 ``8087+``
 
 ``16/32/64-bit``
 """
-FNSTSW_AX: Code = 651 # type: ignore
+FNSTSW_AX: int = 651
 """
 ``FNSTSW AX``
 
 ``DF E0``
 
 ``287+``
 
 ``16/32/64-bit``
 """
-FSTSW_AX: Code = 652 # type: ignore
+FSTSW_AX: int = 652
 """
 ``FSTSW AX``
 
 ``9B DF E0``
 
 ``287+``
 
 ``16/32/64-bit``
 """
-FSTDW_AX: Code = 653 # type: ignore
+FSTDW_AX: int = 653
 """
 ``FSTDW AX``
 
 ``9B DF E1``
 
 ``387 SL``
 
 ``16/32-bit``
 """
-FSTSG_AX: Code = 654 # type: ignore
+FSTSG_AX: int = 654
 """
 ``FSTSG AX``
 
 ``9B DF E2``
 
 ``387 SL``
 
 ``16/32-bit``
 """
-FUCOMIP_ST0_STI: Code = 655 # type: ignore
+FUCOMIP_ST0_STI: int = 655
 """
 ``FUCOMIP ST, ST(i)``
 
 ``DF E8+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-FCOMIP_ST0_STI: Code = 656 # type: ignore
+FCOMIP_ST0_STI: int = 656
 """
 ``FCOMIP ST, ST(i)``
 
 ``DF F0+i``
 
 ``8087+ and CMOV``
 
 ``16/32/64-bit``
 """
-LOOPNE_REL8_16_CX: Code = 657 # type: ignore
+LOOPNE_REL8_16_CX: int = 657
 """
 ``LOOPNE rel8``
 
 ``a16 o16 E0 cb``
 
 ``8086+``
 
 ``16/32-bit``
 """
-LOOPNE_REL8_32_CX: Code = 658 # type: ignore
+LOOPNE_REL8_32_CX: int = 658
 """
 ``LOOPNE rel8``
 
 ``a16 o32 E0 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOPNE_REL8_16_ECX: Code = 659 # type: ignore
+LOOPNE_REL8_16_ECX: int = 659
 """
 ``LOOPNE rel8``
 
 ``a32 o16 E0 cb``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LOOPNE_REL8_32_ECX: Code = 660 # type: ignore
+LOOPNE_REL8_32_ECX: int = 660
 """
 ``LOOPNE rel8``
 
 ``a32 o32 E0 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOPNE_REL8_64_ECX: Code = 661 # type: ignore
+LOOPNE_REL8_64_ECX: int = 661
 """
 ``LOOPNE rel8``
 
 ``a32 o64 E0 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOPNE_REL8_16_RCX: Code = 662 # type: ignore
+LOOPNE_REL8_16_RCX: int = 662
 """
 ``LOOPNE rel8``
 
 ``a64 o16 E0 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOPNE_REL8_64_RCX: Code = 663 # type: ignore
+LOOPNE_REL8_64_RCX: int = 663
 """
 ``LOOPNE rel8``
 
 ``a64 o64 E0 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOPE_REL8_16_CX: Code = 664 # type: ignore
+LOOPE_REL8_16_CX: int = 664
 """
 ``LOOPE rel8``
 
 ``a16 o16 E1 cb``
 
 ``8086+``
 
 ``16/32-bit``
 """
-LOOPE_REL8_32_CX: Code = 665 # type: ignore
+LOOPE_REL8_32_CX: int = 665
 """
 ``LOOPE rel8``
 
 ``a16 o32 E1 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOPE_REL8_16_ECX: Code = 666 # type: ignore
+LOOPE_REL8_16_ECX: int = 666
 """
 ``LOOPE rel8``
 
 ``a32 o16 E1 cb``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LOOPE_REL8_32_ECX: Code = 667 # type: ignore
+LOOPE_REL8_32_ECX: int = 667
 """
 ``LOOPE rel8``
 
 ``a32 o32 E1 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOPE_REL8_64_ECX: Code = 668 # type: ignore
+LOOPE_REL8_64_ECX: int = 668
 """
 ``LOOPE rel8``
 
 ``a32 o64 E1 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOPE_REL8_16_RCX: Code = 669 # type: ignore
+LOOPE_REL8_16_RCX: int = 669
 """
 ``LOOPE rel8``
 
 ``a64 o16 E1 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOPE_REL8_64_RCX: Code = 670 # type: ignore
+LOOPE_REL8_64_RCX: int = 670
 """
 ``LOOPE rel8``
 
 ``a64 o64 E1 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOP_REL8_16_CX: Code = 671 # type: ignore
+LOOP_REL8_16_CX: int = 671
 """
 ``LOOP rel8``
 
 ``a16 o16 E2 cb``
 
 ``8086+``
 
 ``16/32-bit``
 """
-LOOP_REL8_32_CX: Code = 672 # type: ignore
+LOOP_REL8_32_CX: int = 672
 """
 ``LOOP rel8``
 
 ``a16 o32 E2 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOP_REL8_16_ECX: Code = 673 # type: ignore
+LOOP_REL8_16_ECX: int = 673
 """
 ``LOOP rel8``
 
 ``a32 o16 E2 cb``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LOOP_REL8_32_ECX: Code = 674 # type: ignore
+LOOP_REL8_32_ECX: int = 674
 """
 ``LOOP rel8``
 
 ``a32 o32 E2 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-LOOP_REL8_64_ECX: Code = 675 # type: ignore
+LOOP_REL8_64_ECX: int = 675
 """
 ``LOOP rel8``
 
 ``a32 o64 E2 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOP_REL8_16_RCX: Code = 676 # type: ignore
+LOOP_REL8_16_RCX: int = 676
 """
 ``LOOP rel8``
 
 ``a64 o16 E2 cb``
 
 ``X64``
 
 ``64-bit``
 """
-LOOP_REL8_64_RCX: Code = 677 # type: ignore
+LOOP_REL8_64_RCX: int = 677
 """
 ``LOOP rel8``
 
 ``a64 o64 E2 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JCXZ_REL8_16: Code = 678 # type: ignore
+JCXZ_REL8_16: int = 678
 """
 ``JCXZ rel8``
 
 ``a16 o16 E3 cb``
 
 ``8086+``
 
 ``16/32-bit``
 """
-JCXZ_REL8_32: Code = 679 # type: ignore
+JCXZ_REL8_32: int = 679
 """
 ``JCXZ rel8``
 
 ``a16 o32 E3 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JECXZ_REL8_16: Code = 680 # type: ignore
+JECXZ_REL8_16: int = 680
 """
 ``JECXZ rel8``
 
 ``a32 o16 E3 cb``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JECXZ_REL8_32: Code = 681 # type: ignore
+JECXZ_REL8_32: int = 681
 """
 ``JECXZ rel8``
 
 ``a32 o32 E3 cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JECXZ_REL8_64: Code = 682 # type: ignore
+JECXZ_REL8_64: int = 682
 """
 ``JECXZ rel8``
 
 ``a32 o64 E3 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JRCXZ_REL8_16: Code = 683 # type: ignore
+JRCXZ_REL8_16: int = 683
 """
 ``JRCXZ rel8``
 
 ``a64 o16 E3 cb``
 
 ``X64``
 
 ``64-bit``
 """
-JRCXZ_REL8_64: Code = 684 # type: ignore
+JRCXZ_REL8_64: int = 684
 """
 ``JRCXZ rel8``
 
 ``a64 o64 E3 cb``
 
 ``X64``
 
 ``64-bit``
 """
-IN_AL_IMM8: Code = 685 # type: ignore
+IN_AL_IMM8: int = 685
 """
 ``IN AL, imm8``
 
 ``E4 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IN_AX_IMM8: Code = 686 # type: ignore
+IN_AX_IMM8: int = 686
 """
 ``IN AX, imm8``
 
 ``o16 E5 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IN_EAX_IMM8: Code = 687 # type: ignore
+IN_EAX_IMM8: int = 687
 """
 ``IN EAX, imm8``
 
 ``o32 E5 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OUT_IMM8_AL: Code = 688 # type: ignore
+OUT_IMM8_AL: int = 688
 """
 ``OUT imm8, AL``
 
 ``E6 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OUT_IMM8_AX: Code = 689 # type: ignore
+OUT_IMM8_AX: int = 689
 """
 ``OUT imm8, AX``
 
 ``o16 E7 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OUT_IMM8_EAX: Code = 690 # type: ignore
+OUT_IMM8_EAX: int = 690
 """
 ``OUT imm8, EAX``
 
 ``o32 E7 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CALL_REL16: Code = 691 # type: ignore
+CALL_REL16: int = 691
 """
 ``CALL rel16``
 
 ``o16 E8 cw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CALL_REL32_32: Code = 692 # type: ignore
+CALL_REL32_32: int = 692
 """
 ``CALL rel32``
 
 ``o32 E8 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-CALL_REL32_64: Code = 693 # type: ignore
+CALL_REL32_64: int = 693
 """
 ``CALL rel32``
 
 ``o64 E8 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JMP_REL16: Code = 694 # type: ignore
+JMP_REL16: int = 694
 """
 ``JMP rel16``
 
 ``o16 E9 cw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JMP_REL32_32: Code = 695 # type: ignore
+JMP_REL32_32: int = 695
 """
 ``JMP rel32``
 
 ``o32 E9 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JMP_REL32_64: Code = 696 # type: ignore
+JMP_REL32_64: int = 696
 """
 ``JMP rel32``
 
 ``o64 E9 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JMP_PTR1616: Code = 697 # type: ignore
+JMP_PTR1616: int = 697
 """
 ``JMP ptr16:16``
 
 ``o16 EA cd``
 
 ``8086+``
 
 ``16/32-bit``
 """
-JMP_PTR1632: Code = 698 # type: ignore
+JMP_PTR1632: int = 698
 """
 ``JMP ptr16:32``
 
 ``o32 EA cp``
 
 ``386+``
 
 ``16/32-bit``
 """
-JMP_REL8_16: Code = 699 # type: ignore
+JMP_REL8_16: int = 699
 """
 ``JMP rel8``
 
 ``o16 EB cb``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JMP_REL8_32: Code = 700 # type: ignore
+JMP_REL8_32: int = 700
 """
 ``JMP rel8``
 
 ``o32 EB cb``
 
 ``386+``
 
 ``16/32-bit``
 """
-JMP_REL8_64: Code = 701 # type: ignore
+JMP_REL8_64: int = 701
 """
 ``JMP rel8``
 
 ``o64 EB cb``
 
 ``X64``
 
 ``64-bit``
 """
-IN_AL_DX: Code = 702 # type: ignore
+IN_AL_DX: int = 702
 """
 ``IN AL, DX``
 
 ``EC``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IN_AX_DX: Code = 703 # type: ignore
+IN_AX_DX: int = 703
 """
 ``IN AX, DX``
 
 ``o16 ED``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IN_EAX_DX: Code = 704 # type: ignore
+IN_EAX_DX: int = 704
 """
 ``IN EAX, DX``
 
 ``o32 ED``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-OUT_DX_AL: Code = 705 # type: ignore
+OUT_DX_AL: int = 705
 """
 ``OUT DX, AL``
 
 ``EE``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OUT_DX_AX: Code = 706 # type: ignore
+OUT_DX_AX: int = 706
 """
 ``OUT DX, AX``
 
 ``o16 EF``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-OUT_DX_EAX: Code = 707 # type: ignore
+OUT_DX_EAX: int = 707
 """
 ``OUT DX, EAX``
 
 ``o32 EF``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-INT1: Code = 708 # type: ignore
+INT1: int = 708
 """
 ``INT1``
 
 ``F1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-HLT: Code = 709 # type: ignore
+HLT: int = 709
 """
 ``HLT``
 
 ``F4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CMC: Code = 710 # type: ignore
+CMC: int = 710
 """
 ``CMC``
 
 ``F5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM8_IMM8: Code = 711 # type: ignore
+TEST_RM8_IMM8: int = 711
 """
 ``TEST r/m8, imm8``
 
 ``F6 /0 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM8_IMM8_F6R1: Code = 712 # type: ignore
+TEST_RM8_IMM8_F6R1: int = 712
 """
 ``TEST r/m8, imm8``
 
 ``F6 /1 ib``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NOT_RM8: Code = 713 # type: ignore
+NOT_RM8: int = 713
 """
 ``NOT r/m8``
 
 ``F6 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NEG_RM8: Code = 714 # type: ignore
+NEG_RM8: int = 714
 """
 ``NEG r/m8``
 
 ``F6 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MUL_RM8: Code = 715 # type: ignore
+MUL_RM8: int = 715
 """
 ``MUL r/m8``
 
 ``F6 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IMUL_RM8: Code = 716 # type: ignore
+IMUL_RM8: int = 716
 """
 ``IMUL r/m8``
 
 ``F6 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-DIV_RM8: Code = 717 # type: ignore
+DIV_RM8: int = 717
 """
 ``DIV r/m8``
 
 ``F6 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IDIV_RM8: Code = 718 # type: ignore
+IDIV_RM8: int = 718
 """
 ``IDIV r/m8``
 
 ``F6 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM16_IMM16: Code = 719 # type: ignore
+TEST_RM16_IMM16: int = 719
 """
 ``TEST r/m16, imm16``
 
 ``o16 F7 /0 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM32_IMM32: Code = 720 # type: ignore
+TEST_RM32_IMM32: int = 720
 """
 ``TEST r/m32, imm32``
 
 ``o32 F7 /0 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-TEST_RM64_IMM32: Code = 721 # type: ignore
+TEST_RM64_IMM32: int = 721
 """
 ``TEST r/m64, imm32``
 
 ``o64 F7 /0 id``
 
 ``X64``
 
 ``64-bit``
 """
-TEST_RM16_IMM16_F7R1: Code = 722 # type: ignore
+TEST_RM16_IMM16_F7R1: int = 722
 """
 ``TEST r/m16, imm16``
 
 ``o16 F7 /1 iw``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-TEST_RM32_IMM32_F7R1: Code = 723 # type: ignore
+TEST_RM32_IMM32_F7R1: int = 723
 """
 ``TEST r/m32, imm32``
 
 ``o32 F7 /1 id``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-TEST_RM64_IMM32_F7R1: Code = 724 # type: ignore
+TEST_RM64_IMM32_F7R1: int = 724
 """
 ``TEST r/m64, imm32``
 
 ``o64 F7 /1 id``
 
 ``X64``
 
 ``64-bit``
 """
-NOT_RM16: Code = 725 # type: ignore
+NOT_RM16: int = 725
 """
 ``NOT r/m16``
 
 ``o16 F7 /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NOT_RM32: Code = 726 # type: ignore
+NOT_RM32: int = 726
 """
 ``NOT r/m32``
 
 ``o32 F7 /2``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-NOT_RM64: Code = 727 # type: ignore
+NOT_RM64: int = 727
 """
 ``NOT r/m64``
 
 ``o64 F7 /2``
 
 ``X64``
 
 ``64-bit``
 """
-NEG_RM16: Code = 728 # type: ignore
+NEG_RM16: int = 728
 """
 ``NEG r/m16``
 
 ``o16 F7 /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-NEG_RM32: Code = 729 # type: ignore
+NEG_RM32: int = 729
 """
 ``NEG r/m32``
 
 ``o32 F7 /3``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-NEG_RM64: Code = 730 # type: ignore
+NEG_RM64: int = 730
 """
 ``NEG r/m64``
 
 ``o64 F7 /3``
 
 ``X64``
 
 ``64-bit``
 """
-MUL_RM16: Code = 731 # type: ignore
+MUL_RM16: int = 731
 """
 ``MUL r/m16``
 
 ``o16 F7 /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-MUL_RM32: Code = 732 # type: ignore
+MUL_RM32: int = 732
 """
 ``MUL r/m32``
 
 ``o32 F7 /4``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MUL_RM64: Code = 733 # type: ignore
+MUL_RM64: int = 733
 """
 ``MUL r/m64``
 
 ``o64 F7 /4``
 
 ``X64``
 
 ``64-bit``
 """
-IMUL_RM16: Code = 734 # type: ignore
+IMUL_RM16: int = 734
 """
 ``IMUL r/m16``
 
 ``o16 F7 /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IMUL_RM32: Code = 735 # type: ignore
+IMUL_RM32: int = 735
 """
 ``IMUL r/m32``
 
 ``o32 F7 /5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IMUL_RM64: Code = 736 # type: ignore
+IMUL_RM64: int = 736
 """
 ``IMUL r/m64``
 
 ``o64 F7 /5``
 
 ``X64``
 
 ``64-bit``
 """
-DIV_RM16: Code = 737 # type: ignore
+DIV_RM16: int = 737
 """
 ``DIV r/m16``
 
 ``o16 F7 /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-DIV_RM32: Code = 738 # type: ignore
+DIV_RM32: int = 738
 """
 ``DIV r/m32``
 
 ``o32 F7 /6``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-DIV_RM64: Code = 739 # type: ignore
+DIV_RM64: int = 739
 """
 ``DIV r/m64``
 
 ``o64 F7 /6``
 
 ``X64``
 
 ``64-bit``
 """
-IDIV_RM16: Code = 740 # type: ignore
+IDIV_RM16: int = 740
 """
 ``IDIV r/m16``
 
 ``o16 F7 /7``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-IDIV_RM32: Code = 741 # type: ignore
+IDIV_RM32: int = 741
 """
 ``IDIV r/m32``
 
 ``o32 F7 /7``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IDIV_RM64: Code = 742 # type: ignore
+IDIV_RM64: int = 742
 """
 ``IDIV r/m64``
 
 ``o64 F7 /7``
 
 ``X64``
 
 ``64-bit``
 """
-CLC: Code = 743 # type: ignore
+CLC: int = 743
 """
 ``CLC``
 
 ``F8``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-STC: Code = 744 # type: ignore
+STC: int = 744
 """
 ``STC``
 
 ``F9``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CLI: Code = 745 # type: ignore
+CLI: int = 745
 """
 ``CLI``
 
 ``FA``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-STI: Code = 746 # type: ignore
+STI: int = 746
 """
 ``STI``
 
 ``FB``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CLD: Code = 747 # type: ignore
+CLD: int = 747
 """
 ``CLD``
 
 ``FC``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-STD: Code = 748 # type: ignore
+STD: int = 748
 """
 ``STD``
 
 ``FD``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-INC_RM8: Code = 749 # type: ignore
+INC_RM8: int = 749
 """
 ``INC r/m8``
 
 ``FE /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-DEC_RM8: Code = 750 # type: ignore
+DEC_RM8: int = 750
 """
 ``DEC r/m8``
 
 ``FE /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-INC_RM16: Code = 751 # type: ignore
+INC_RM16: int = 751
 """
 ``INC r/m16``
 
 ``o16 FF /0``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-INC_RM32: Code = 752 # type: ignore
+INC_RM32: int = 752
 """
 ``INC r/m32``
 
 ``o32 FF /0``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-INC_RM64: Code = 753 # type: ignore
+INC_RM64: int = 753
 """
 ``INC r/m64``
 
 ``o64 FF /0``
 
 ``X64``
 
 ``64-bit``
 """
-DEC_RM16: Code = 754 # type: ignore
+DEC_RM16: int = 754
 """
 ``DEC r/m16``
 
 ``o16 FF /1``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-DEC_RM32: Code = 755 # type: ignore
+DEC_RM32: int = 755
 """
 ``DEC r/m32``
 
 ``o32 FF /1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-DEC_RM64: Code = 756 # type: ignore
+DEC_RM64: int = 756
 """
 ``DEC r/m64``
 
 ``o64 FF /1``
 
 ``X64``
 
 ``64-bit``
 """
-CALL_RM16: Code = 757 # type: ignore
+CALL_RM16: int = 757
 """
 ``CALL r/m16``
 
 ``o16 FF /2``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CALL_RM32: Code = 758 # type: ignore
+CALL_RM32: int = 758
 """
 ``CALL r/m32``
 
 ``o32 FF /2``
 
 ``386+``
 
 ``16/32-bit``
 """
-CALL_RM64: Code = 759 # type: ignore
+CALL_RM64: int = 759
 """
 ``CALL r/m64``
 
 ``o64 FF /2``
 
 ``X64``
 
 ``64-bit``
 """
-CALL_M1616: Code = 760 # type: ignore
+CALL_M1616: int = 760
 """
 ``CALL m16:16``
 
 ``o16 FF /3``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-CALL_M1632: Code = 761 # type: ignore
+CALL_M1632: int = 761
 """
 ``CALL m16:32``
 
 ``o32 FF /3``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-CALL_M1664: Code = 762 # type: ignore
+CALL_M1664: int = 762
 """
 ``CALL m16:64``
 
 ``o64 FF /3``
 
 ``X64``
 
 ``64-bit``
 """
-JMP_RM16: Code = 763 # type: ignore
+JMP_RM16: int = 763
 """
 ``JMP r/m16``
 
 ``o16 FF /4``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JMP_RM32: Code = 764 # type: ignore
+JMP_RM32: int = 764
 """
 ``JMP r/m32``
 
 ``o32 FF /4``
 
 ``386+``
 
 ``16/32-bit``
 """
-JMP_RM64: Code = 765 # type: ignore
+JMP_RM64: int = 765
 """
 ``JMP r/m64``
 
 ``o64 FF /4``
 
 ``X64``
 
 ``64-bit``
 """
-JMP_M1616: Code = 766 # type: ignore
+JMP_M1616: int = 766
 """
 ``JMP m16:16``
 
 ``o16 FF /5``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-JMP_M1632: Code = 767 # type: ignore
+JMP_M1632: int = 767
 """
 ``JMP m16:32``
 
 ``o32 FF /5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JMP_M1664: Code = 768 # type: ignore
+JMP_M1664: int = 768
 """
 ``JMP m16:64``
 
 ``o64 FF /5``
 
 ``X64``
 
 ``64-bit``
 """
-PUSH_RM16: Code = 769 # type: ignore
+PUSH_RM16: int = 769
 """
 ``PUSH r/m16``
 
 ``o16 FF /6``
 
 ``8086+``
 
 ``16/32/64-bit``
 """
-PUSH_RM32: Code = 770 # type: ignore
+PUSH_RM32: int = 770
 """
 ``PUSH r/m32``
 
 ``o32 FF /6``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSH_RM64: Code = 771 # type: ignore
+PUSH_RM64: int = 771
 """
 ``PUSH r/m64``
 
 ``o64 FF /6``
 
 ``X64``
 
 ``64-bit``
 """
-SLDT_RM16: Code = 772 # type: ignore
+SLDT_RM16: int = 772
 """
 ``SLDT r/m16``
 
 ``o16 0F 00 /0``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-SLDT_R32M16: Code = 773 # type: ignore
+SLDT_R32M16: int = 773
 """
 ``SLDT r32/m16``
 
 ``o32 0F 00 /0``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SLDT_R64M16: Code = 774 # type: ignore
+SLDT_R64M16: int = 774
 """
 ``SLDT r64/m16``
 
 ``o64 0F 00 /0``
 
 ``X64``
 
 ``64-bit``
 """
-STR_RM16: Code = 775 # type: ignore
+STR_RM16: int = 775
 """
 ``STR r/m16``
 
 ``o16 0F 00 /1``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-STR_R32M16: Code = 776 # type: ignore
+STR_R32M16: int = 776
 """
 ``STR r32/m16``
 
 ``o32 0F 00 /1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-STR_R64M16: Code = 777 # type: ignore
+STR_R64M16: int = 777
 """
 ``STR r64/m16``
 
 ``o64 0F 00 /1``
 
 ``X64``
 
 ``64-bit``
 """
-LLDT_RM16: Code = 778 # type: ignore
+LLDT_RM16: int = 778
 """
 ``LLDT r/m16``
 
 ``o16 0F 00 /2``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LLDT_R32M16: Code = 779 # type: ignore
+LLDT_R32M16: int = 779
 """
 ``LLDT r32/m16``
 
 ``o32 0F 00 /2``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LLDT_R64M16: Code = 780 # type: ignore
+LLDT_R64M16: int = 780
 """
 ``LLDT r64/m16``
 
 ``o64 0F 00 /2``
 
 ``X64``
 
 ``64-bit``
 """
-LTR_RM16: Code = 781 # type: ignore
+LTR_RM16: int = 781
 """
 ``LTR r/m16``
 
 ``o16 0F 00 /3``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LTR_R32M16: Code = 782 # type: ignore
+LTR_R32M16: int = 782
 """
 ``LTR r32/m16``
 
 ``o32 0F 00 /3``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LTR_R64M16: Code = 783 # type: ignore
+LTR_R64M16: int = 783
 """
 ``LTR r64/m16``
 
 ``o64 0F 00 /3``
 
 ``X64``
 
 ``64-bit``
 """
-VERR_RM16: Code = 784 # type: ignore
+VERR_RM16: int = 784
 """
 ``VERR r/m16``
 
 ``o16 0F 00 /4``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-VERR_R32M16: Code = 785 # type: ignore
+VERR_R32M16: int = 785
 """
 ``VERR r32/m16``
 
 ``o32 0F 00 /4``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-VERR_R64M16: Code = 786 # type: ignore
+VERR_R64M16: int = 786
 """
 ``VERR r64/m16``
 
 ``o64 0F 00 /4``
 
 ``X64``
 
 ``64-bit``
 """
-VERW_RM16: Code = 787 # type: ignore
+VERW_RM16: int = 787
 """
 ``VERW r/m16``
 
 ``o16 0F 00 /5``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-VERW_R32M16: Code = 788 # type: ignore
+VERW_R32M16: int = 788
 """
 ``VERW r32/m16``
 
 ``o32 0F 00 /5``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-VERW_R64M16: Code = 789 # type: ignore
+VERW_R64M16: int = 789
 """
 ``VERW r64/m16``
 
 ``o64 0F 00 /5``
 
 ``X64``
 
 ``64-bit``
 """
-JMPE_RM16: Code = 790 # type: ignore
+JMPE_RM16: int = 790
 """
 ``JMPE r/m16``
 
 ``o16 0F 00 /6``
 
 ``IA-64``
 
 ``16/32-bit``
 """
-JMPE_RM32: Code = 791 # type: ignore
+JMPE_RM32: int = 791
 """
 ``JMPE r/m32``
 
 ``o32 0F 00 /6``
 
 ``IA-64``
 
 ``16/32-bit``
 """
-SGDT_M1632_16: Code = 792 # type: ignore
+SGDT_M1632_16: int = 792
 """
 ``SGDT m``
 
 ``o16 0F 01 /0``
 
 ``286+``
 
 ``16/32-bit``
 """
-SGDT_M1632: Code = 793 # type: ignore
+SGDT_M1632: int = 793
 """
 ``SGDT m``
 
 ``o32 0F 01 /0``
 
 ``386+``
 
 ``16/32-bit``
 """
-SGDT_M1664: Code = 794 # type: ignore
+SGDT_M1664: int = 794
 """
 ``SGDT m``
 
 ``0F 01 /0``
 
 ``X64``
 
 ``64-bit``
 """
-SIDT_M1632_16: Code = 795 # type: ignore
+SIDT_M1632_16: int = 795
 """
 ``SIDT m``
 
 ``o16 0F 01 /1``
 
 ``286+``
 
 ``16/32-bit``
 """
-SIDT_M1632: Code = 796 # type: ignore
+SIDT_M1632: int = 796
 """
 ``SIDT m``
 
 ``o32 0F 01 /1``
 
 ``386+``
 
 ``16/32-bit``
 """
-SIDT_M1664: Code = 797 # type: ignore
+SIDT_M1664: int = 797
 """
 ``SIDT m``
 
 ``0F 01 /1``
 
 ``X64``
 
 ``64-bit``
 """
-LGDT_M1632_16: Code = 798 # type: ignore
+LGDT_M1632_16: int = 798
 """
 ``LGDT m16&32``
 
 ``o16 0F 01 /2``
 
 ``286+``
 
 ``16/32-bit``
 """
-LGDT_M1632: Code = 799 # type: ignore
+LGDT_M1632: int = 799
 """
 ``LGDT m16&32``
 
 ``o32 0F 01 /2``
 
 ``386+``
 
 ``16/32-bit``
 """
-LGDT_M1664: Code = 800 # type: ignore
+LGDT_M1664: int = 800
 """
 ``LGDT m16&64``
 
 ``0F 01 /2``
 
 ``X64``
 
 ``64-bit``
 """
-LIDT_M1632_16: Code = 801 # type: ignore
+LIDT_M1632_16: int = 801
 """
 ``LIDT m16&32``
 
 ``o16 0F 01 /3``
 
 ``286+``
 
 ``16/32-bit``
 """
-LIDT_M1632: Code = 802 # type: ignore
+LIDT_M1632: int = 802
 """
 ``LIDT m16&32``
 
 ``o32 0F 01 /3``
 
 ``386+``
 
 ``16/32-bit``
 """
-LIDT_M1664: Code = 803 # type: ignore
+LIDT_M1664: int = 803
 """
 ``LIDT m16&64``
 
 ``0F 01 /3``
 
 ``X64``
 
 ``64-bit``
 """
-SMSW_RM16: Code = 804 # type: ignore
+SMSW_RM16: int = 804
 """
 ``SMSW r/m16``
 
 ``o16 0F 01 /4``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-SMSW_R32M16: Code = 805 # type: ignore
+SMSW_R32M16: int = 805
 """
 ``SMSW r32/m16``
 
 ``o32 0F 01 /4``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SMSW_R64M16: Code = 806 # type: ignore
+SMSW_R64M16: int = 806
 """
 ``SMSW r64/m16``
 
 ``o64 0F 01 /4``
 
 ``X64``
 
 ``64-bit``
 """
-RSTORSSP_M64: Code = 807 # type: ignore
+RSTORSSP_M64: int = 807
 """
 ``RSTORSSP m64``
 
 ``F3 0F 01 /5``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-LMSW_RM16: Code = 808 # type: ignore
+LMSW_RM16: int = 808
 """
 ``LMSW r/m16``
 
 ``o16 0F 01 /6``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LMSW_R32M16: Code = 809 # type: ignore
+LMSW_R32M16: int = 809
 """
 ``LMSW r32/m16``
 
 ``o32 0F 01 /6``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LMSW_R64M16: Code = 810 # type: ignore
+LMSW_R64M16: int = 810
 """
 ``LMSW r64/m16``
 
 ``o64 0F 01 /6``
 
 ``X64``
 
 ``64-bit``
 """
-INVLPG_M: Code = 811 # type: ignore
+INVLPG_M: int = 811
 """
 ``INVLPG m``
 
 ``0F 01 /7``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-ENCLV: Code = 812 # type: ignore
+ENCLV: int = 812
 """
 ``ENCLV``
 
 ``NP 0F 01 C0``
 
 ``OSS``
 
 ``16/32/64-bit``
 """
-VMCALL: Code = 813 # type: ignore
+VMCALL: int = 813
 """
 ``VMCALL``
 
 ``NP 0F 01 C1``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-VMLAUNCH: Code = 814 # type: ignore
+VMLAUNCH: int = 814
 """
 ``VMLAUNCH``
 
 ``NP 0F 01 C2``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-VMRESUME: Code = 815 # type: ignore
+VMRESUME: int = 815
 """
 ``VMRESUME``
 
 ``NP 0F 01 C3``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-VMXOFF: Code = 816 # type: ignore
+VMXOFF: int = 816
 """
 ``VMXOFF``
 
 ``NP 0F 01 C4``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-PCONFIG: Code = 817 # type: ignore
+PCONFIG: int = 817
 """
 ``PCONFIG``
 
 ``NP 0F 01 C5``
 
 ``PCONFIG``
 
 ``16/32/64-bit``
 """
-MONITORW: Code = 818 # type: ignore
+MONITORW: int = 818
 """
 ``MONITOR``
 
 ``a16 NP 0F 01 C8``
 
 ``MONITOR``
 
 ``16/32-bit``
 """
-MONITORD: Code = 819 # type: ignore
+MONITORD: int = 819
 """
 ``MONITOR``
 
 ``a32 NP 0F 01 C8``
 
 ``MONITOR``
 
 ``16/32/64-bit``
 """
-MONITORQ: Code = 820 # type: ignore
+MONITORQ: int = 820
 """
 ``MONITOR``
 
 ``a64 NP 0F 01 C8``
 
 ``MONITOR``
 
 ``64-bit``
 """
-MWAIT: Code = 821 # type: ignore
+MWAIT: int = 821
 """
 ``MWAIT``
 
 ``NP 0F 01 C9``
 
 ``MONITOR``
 
 ``16/32/64-bit``
 """
-CLAC: Code = 822 # type: ignore
+CLAC: int = 822
 """
 ``CLAC``
 
 ``NP 0F 01 CA``
 
 ``SMAP``
 
 ``16/32/64-bit``
 """
-STAC: Code = 823 # type: ignore
+STAC: int = 823
 """
 ``STAC``
 
 ``NP 0F 01 CB``
 
 ``SMAP``
 
 ``16/32/64-bit``
 """
-ENCLS: Code = 824 # type: ignore
+ENCLS: int = 824
 """
 ``ENCLS``
 
 ``NP 0F 01 CF``
 
 ``SGX1``
 
 ``16/32/64-bit``
 """
-XGETBV: Code = 825 # type: ignore
+XGETBV: int = 825
 """
 ``XGETBV``
 
 ``NP 0F 01 D0``
 
 ``XSAVE``
 
 ``16/32/64-bit``
 """
-XSETBV: Code = 826 # type: ignore
+XSETBV: int = 826
 """
 ``XSETBV``
 
 ``NP 0F 01 D1``
 
 ``XSAVE``
 
 ``16/32/64-bit``
 """
-VMFUNC: Code = 827 # type: ignore
+VMFUNC: int = 827
 """
 ``VMFUNC``
 
 ``NP 0F 01 D4``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-XEND: Code = 828 # type: ignore
+XEND: int = 828
 """
 ``XEND``
 
 ``NP 0F 01 D5``
 
 ``RTM``
 
 ``16/32/64-bit``
 """
-XTEST: Code = 829 # type: ignore
+XTEST: int = 829
 """
 ``XTEST``
 
 ``NP 0F 01 D6``
 
 ``HLE or RTM``
 
 ``16/32/64-bit``
 """
-ENCLU: Code = 830 # type: ignore
+ENCLU: int = 830
 """
 ``ENCLU``
 
 ``NP 0F 01 D7``
 
 ``SGX1``
 
 ``16/32/64-bit``
 """
-VMRUNW: Code = 831 # type: ignore
+VMRUNW: int = 831
 """
 ``VMRUN``
 
 ``a16 0F 01 D8``
 
 ``SVM``
 
 ``16/32-bit``
 """
-VMRUND: Code = 832 # type: ignore
+VMRUND: int = 832
 """
 ``VMRUN``
 
 ``a32 0F 01 D8``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-VMRUNQ: Code = 833 # type: ignore
+VMRUNQ: int = 833
 """
 ``VMRUN``
 
 ``a64 0F 01 D8``
 
 ``SVM``
 
 ``64-bit``
 """
-VMMCALL: Code = 834 # type: ignore
+VMMCALL: int = 834
 """
 ``VMMCALL``
 
 ``0F 01 D9``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-VMLOADW: Code = 835 # type: ignore
+VMLOADW: int = 835
 """
 ``VMLOAD``
 
 ``a16 0F 01 DA``
 
 ``SVM``
 
 ``16/32-bit``
 """
-VMLOADD: Code = 836 # type: ignore
+VMLOADD: int = 836
 """
 ``VMLOAD``
 
 ``a32 0F 01 DA``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-VMLOADQ: Code = 837 # type: ignore
+VMLOADQ: int = 837
 """
 ``VMLOAD``
 
 ``a64 0F 01 DA``
 
 ``SVM``
 
 ``64-bit``
 """
-VMSAVEW: Code = 838 # type: ignore
+VMSAVEW: int = 838
 """
 ``VMSAVE``
 
 ``a16 0F 01 DB``
 
 ``SVM``
 
 ``16/32-bit``
 """
-VMSAVED: Code = 839 # type: ignore
+VMSAVED: int = 839
 """
 ``VMSAVE``
 
 ``a32 0F 01 DB``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-VMSAVEQ: Code = 840 # type: ignore
+VMSAVEQ: int = 840
 """
 ``VMSAVE``
 
 ``a64 0F 01 DB``
 
 ``SVM``
 
 ``64-bit``
 """
-STGI: Code = 841 # type: ignore
+STGI: int = 841
 """
 ``STGI``
 
 ``0F 01 DC``
 
 ``SKINIT or SVM``
 
 ``16/32/64-bit``
 """
-CLGI: Code = 842 # type: ignore
+CLGI: int = 842
 """
 ``CLGI``
 
 ``0F 01 DD``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-SKINIT: Code = 843 # type: ignore
+SKINIT: int = 843
 """
 ``SKINIT``
 
 ``0F 01 DE``
 
 ``SKINIT or SVM``
 
 ``16/32/64-bit``
 """
-INVLPGAW: Code = 844 # type: ignore
+INVLPGAW: int = 844
 """
 ``INVLPGA``
 
 ``a16 0F 01 DF``
 
 ``SVM``
 
 ``16/32-bit``
 """
-INVLPGAD: Code = 845 # type: ignore
+INVLPGAD: int = 845
 """
 ``INVLPGA``
 
 ``a32 0F 01 DF``
 
 ``SVM``
 
 ``16/32/64-bit``
 """
-INVLPGAQ: Code = 846 # type: ignore
+INVLPGAQ: int = 846
 """
 ``INVLPGA``
 
 ``a64 0F 01 DF``
 
 ``SVM``
 
 ``64-bit``
 """
-SETSSBSY: Code = 847 # type: ignore
+SETSSBSY: int = 847
 """
 ``SETSSBSY``
 
 ``F3 0F 01 E8``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-SAVEPREVSSP: Code = 848 # type: ignore
+SAVEPREVSSP: int = 848
 """
 ``SAVEPREVSSP``
 
 ``F3 0F 01 EA``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-RDPKRU: Code = 849 # type: ignore
+RDPKRU: int = 849
 """
 ``RDPKRU``
 
 ``NP 0F 01 EE``
 
 ``PKU``
 
 ``16/32/64-bit``
 """
-WRPKRU: Code = 850 # type: ignore
+WRPKRU: int = 850
 """
 ``WRPKRU``
 
 ``NP 0F 01 EF``
 
 ``PKU``
 
 ``16/32/64-bit``
 """
-SWAPGS: Code = 851 # type: ignore
+SWAPGS: int = 851
 """
 ``SWAPGS``
 
 ``0F 01 F8``
 
 ``X64``
 
 ``64-bit``
 """
-RDTSCP: Code = 852 # type: ignore
+RDTSCP: int = 852
 """
 ``RDTSCP``
 
 ``0F 01 F9``
 
 ``RDTSCP``
 
 ``16/32/64-bit``
 """
-MONITORXW: Code = 853 # type: ignore
+MONITORXW: int = 853
 """
 ``MONITORX``
 
 ``a16 NP 0F 01 FA``
 
 ``MONITORX``
 
 ``16/32-bit``
 """
-MONITORXD: Code = 854 # type: ignore
+MONITORXD: int = 854
 """
 ``MONITORX``
 
 ``a32 NP 0F 01 FA``
 
 ``MONITORX``
 
 ``16/32/64-bit``
 """
-MONITORXQ: Code = 855 # type: ignore
+MONITORXQ: int = 855
 """
 ``MONITORX``
 
 ``a64 NP 0F 01 FA``
 
 ``MONITORX``
 
 ``64-bit``
 """
-MCOMMIT: Code = 856 # type: ignore
+MCOMMIT: int = 856
 """
 ``MCOMMIT``
 
 ``F3 0F 01 FA``
 
 ``MCOMMIT``
 
 ``16/32/64-bit``
 """
-MWAITX: Code = 857 # type: ignore
+MWAITX: int = 857
 """
 ``MWAITX``
 
 ``NP 0F 01 FB``
 
 ``MONITORX``
 
 ``16/32/64-bit``
 """
-CLZEROW: Code = 858 # type: ignore
+CLZEROW: int = 858
 """
 ``CLZERO``
 
 ``a16 0F 01 FC``
 
 ``CLZERO``
 
 ``16/32-bit``
 """
-CLZEROD: Code = 859 # type: ignore
+CLZEROD: int = 859
 """
 ``CLZERO``
 
 ``a32 0F 01 FC``
 
 ``CLZERO``
 
 ``16/32/64-bit``
 """
-CLZEROQ: Code = 860 # type: ignore
+CLZEROQ: int = 860
 """
 ``CLZERO``
 
 ``a64 0F 01 FC``
 
 ``CLZERO``
 
 ``64-bit``
 """
-RDPRU: Code = 861 # type: ignore
+RDPRU: int = 861
 """
 ``RDPRU``
 
-``NP 0F 01 FD``
+``0F 01 FD``
 
 ``RDPRU``
 
 ``16/32/64-bit``
 """
-LAR_R16_RM16: Code = 862 # type: ignore
+LAR_R16_RM16: int = 862
 """
 ``LAR r16, r/m16``
 
 ``o16 0F 02 /r``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LAR_R32_R32M16: Code = 863 # type: ignore
+LAR_R32_R32M16: int = 863
 """
 ``LAR r32, r32/m16``
 
 ``o32 0F 02 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LAR_R64_R64M16: Code = 864 # type: ignore
+LAR_R64_R64M16: int = 864
 """
 ``LAR r64, r64/m16``
 
 ``o64 0F 02 /r``
 
 ``X64``
 
 ``64-bit``
 """
-LSL_R16_RM16: Code = 865 # type: ignore
+LSL_R16_RM16: int = 865
 """
 ``LSL r16, r/m16``
 
 ``o16 0F 03 /r``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LSL_R32_R32M16: Code = 866 # type: ignore
+LSL_R32_R32M16: int = 866
 """
 ``LSL r32, r32/m16``
 
 ``o32 0F 03 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LSL_R64_R64M16: Code = 867 # type: ignore
+LSL_R64_R64M16: int = 867
 """
 ``LSL r64, r64/m16``
 
 ``o64 0F 03 /r``
 
 ``X64``
 
 ``64-bit``
 """
-STOREALL: Code = 868 # type: ignore
+LOADALLRESET286: int = 868
 """
-``STOREALL``
+``LOADALL``
 
 ``0F 04``
 
 ``286``
 
 ``16/32-bit``
 """
-LOADALL286: Code = 869 # type: ignore
+LOADALL286: int = 869
 """
 ``LOADALL``
 
 ``0F 05``
 
 ``286``
 
 ``16/32-bit``
 """
-SYSCALL: Code = 870 # type: ignore
+SYSCALL: int = 870
 """
 ``SYSCALL``
 
 ``0F 05``
 
 ``SYSCALL``
 
 ``16/32/64-bit``
 """
-CLTS: Code = 871 # type: ignore
+CLTS: int = 871
 """
 ``CLTS``
 
 ``0F 06``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-LOADALL386: Code = 872 # type: ignore
+LOADALL386: int = 872
 """
 ``LOADALL``
 
 ``0F 07``
 
 ``386``
 
 ``16/32-bit``
 """
-SYSRETD: Code = 873 # type: ignore
+SYSRETD: int = 873
 """
 ``SYSRET``
 
 ``0F 07``
 
 ``SYSCALL``
 
 ``16/32/64-bit``
 """
-SYSRETQ: Code = 874 # type: ignore
+SYSRETQ: int = 874
 """
 ``SYSRETQ``
 
 ``o64 0F 07``
 
 ``SYSCALL``
 
 ``64-bit``
 """
-INVD: Code = 875 # type: ignore
+INVD: int = 875
 """
 ``INVD``
 
 ``0F 08``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-WBINVD: Code = 876 # type: ignore
+WBINVD: int = 876
 """
 ``WBINVD``
 
 ``0F 09``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-WBNOINVD: Code = 877 # type: ignore
+WBNOINVD: int = 877
 """
 ``WBNOINVD``
 
 ``F3 0F 09``
 
 ``WBNOINVD``
 
 ``16/32/64-bit``
 """
-CL1INVMB: Code = 878 # type: ignore
+CL1INVMB: int = 878
 """
 ``CL1INVMB``
 
 ``0F 0A``
 
 ``CL1INVMB``
 
 ``16/32-bit``
 """
-UD2: Code = 879 # type: ignore
+UD2: int = 879
 """
 ``UD2``
 
 ``0F 0B``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM16_R16_0F0D: Code = 880 # type: ignore
+RESERVEDNOP_RM16_R16_0F0D: int = 880
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 0D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F0D: Code = 881 # type: ignore
+RESERVEDNOP_RM32_R32_0F0D: int = 881
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 0D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F0D: Code = 882 # type: ignore
+RESERVEDNOP_RM64_R64_0F0D: int = 882
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 0D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-PREFETCH_M8: Code = 883 # type: ignore
+PREFETCH_M8: int = 883
 """
 ``PREFETCH m8``
 
 ``0F 0D /0``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHW_M8: Code = 884 # type: ignore
+PREFETCHW_M8: int = 884
 """
 ``PREFETCHW m8``
 
 ``0F 0D /1``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHWT1_M8: Code = 885 # type: ignore
+PREFETCHWT1_M8: int = 885
 """
 ``PREFETCHWT1 m8``
 
 ``0F 0D /2``
 
 ``PREFETCHWT1``
 
 ``16/32/64-bit``
 """
-FEMMS: Code = 886 # type: ignore
+FEMMS: int = 886
 """
 ``FEMMS``
 
 ``0F 0E``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-UMOV_RM8_R8: Code = 887 # type: ignore
+UMOV_RM8_R8: int = 887
 """
 ``UMOV r/m8, r8``
 
 ``0F 10 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-UMOV_RM16_R16: Code = 888 # type: ignore
+UMOV_RM16_R16: int = 888
 """
 ``UMOV r/m16, r16``
 
 ``o16 0F 11 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-UMOV_RM32_R32: Code = 889 # type: ignore
+UMOV_RM32_R32: int = 889
 """
 ``UMOV r/m32, r32``
 
 ``o32 0F 11 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-UMOV_R8_RM8: Code = 890 # type: ignore
+UMOV_R8_RM8: int = 890
 """
 ``UMOV r8, r/m8``
 
 ``0F 12 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-UMOV_R16_RM16: Code = 891 # type: ignore
+UMOV_R16_RM16: int = 891
 """
 ``UMOV r16, r/m16``
 
 ``o16 0F 13 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-UMOV_R32_RM32: Code = 892 # type: ignore
+UMOV_R32_RM32: int = 892
 """
 ``UMOV r32, r/m32``
 
 ``o32 0F 13 /r``
 
 ``386/486``
 
 ``16/32-bit``
 """
-MOVUPS_XMM_XMMM128: Code = 893 # type: ignore
+MOVUPS_XMM_XMMM128: int = 893
 """
 ``MOVUPS xmm1, xmm2/m128``
 
 ``NP 0F 10 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPS_XMM_XMMM128: Code = 894 # type: ignore
+VEX_VMOVUPS_XMM_XMMM128: int = 894
 """
 ``VMOVUPS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPS_YMM_YMMM256: Code = 895 # type: ignore
+VEX_VMOVUPS_YMM_YMMM256: int = 895
 """
 ``VMOVUPS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_XMM_K1Z_XMMM128: Code = 896 # type: ignore
+EVEX_VMOVUPS_XMM_K1Z_XMMM128: int = 896
 """
 ``VMOVUPS xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.0F.W0 10 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_YMM_K1Z_YMMM256: Code = 897 # type: ignore
+EVEX_VMOVUPS_YMM_K1Z_YMMM256: int = 897
 """
 ``VMOVUPS ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.0F.W0 10 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_ZMM_K1Z_ZMMM512: Code = 898 # type: ignore
+EVEX_VMOVUPS_ZMM_K1Z_ZMMM512: int = 898
 """
 ``VMOVUPS zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.0F.W0 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVUPD_XMM_XMMM128: Code = 899 # type: ignore
+MOVUPD_XMM_XMMM128: int = 899
 """
 ``MOVUPD xmm1, xmm2/m128``
 
 ``66 0F 10 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPD_XMM_XMMM128: Code = 900 # type: ignore
+VEX_VMOVUPD_XMM_XMMM128: int = 900
 """
 ``VMOVUPD xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPD_YMM_YMMM256: Code = 901 # type: ignore
+VEX_VMOVUPD_YMM_YMMM256: int = 901
 """
 ``VMOVUPD ymm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_XMM_K1Z_XMMM128: Code = 902 # type: ignore
+EVEX_VMOVUPD_XMM_K1Z_XMMM128: int = 902
 """
 ``VMOVUPD xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F.W1 10 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_YMM_K1Z_YMMM256: Code = 903 # type: ignore
+EVEX_VMOVUPD_YMM_K1Z_YMMM256: int = 903
 """
 ``VMOVUPD ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F.W1 10 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_ZMM_K1Z_ZMMM512: Code = 904 # type: ignore
+EVEX_VMOVUPD_ZMM_K1Z_ZMMM512: int = 904
 """
 ``VMOVUPD zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F.W1 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSS_XMM_XMMM32: Code = 905 # type: ignore
+MOVSS_XMM_XMMM32: int = 905
 """
 ``MOVSS xmm1, xmm2/m32``
 
 ``F3 0F 10 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSS_XMM_XMM_XMM: Code = 906 # type: ignore
+VEX_VMOVSS_XMM_XMM_XMM: int = 906
 """
 ``VMOVSS xmm1, xmm2, xmm3``
 
 ``VEX.LIG.F3.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSS_XMM_M32: Code = 907 # type: ignore
+VEX_VMOVSS_XMM_M32: int = 907
 """
 ``VMOVSS xmm1, m32``
 
 ``VEX.LIG.F3.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSS_XMM_K1Z_XMM_XMM: Code = 908 # type: ignore
+EVEX_VMOVSS_XMM_K1Z_XMM_XMM: int = 908
 """
 ``VMOVSS xmm1 {k1}{z}, xmm2, xmm3``
 
 ``EVEX.LIG.F3.0F.W0 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSS_XMM_K1Z_M32: Code = 909 # type: ignore
+EVEX_VMOVSS_XMM_K1Z_M32: int = 909
 """
 ``VMOVSS xmm1 {k1}{z}, m32``
 
 ``EVEX.LIG.F3.0F.W0 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSD_XMM_XMMM64: Code = 910 # type: ignore
+MOVSD_XMM_XMMM64: int = 910
 """
 ``MOVSD xmm1, xmm2/m64``
 
 ``F2 0F 10 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSD_XMM_XMM_XMM: Code = 911 # type: ignore
+VEX_VMOVSD_XMM_XMM_XMM: int = 911
 """
 ``VMOVSD xmm1, xmm2, xmm3``
 
 ``VEX.LIG.F2.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSD_XMM_M64: Code = 912 # type: ignore
+VEX_VMOVSD_XMM_M64: int = 912
 """
 ``VMOVSD xmm1, m64``
 
 ``VEX.LIG.F2.0F.WIG 10 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSD_XMM_K1Z_XMM_XMM: Code = 913 # type: ignore
+EVEX_VMOVSD_XMM_K1Z_XMM_XMM: int = 913
 """
 ``VMOVSD xmm1 {k1}{z}, xmm2, xmm3``
 
 ``EVEX.LIG.F2.0F.W1 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSD_XMM_K1Z_M64: Code = 914 # type: ignore
+EVEX_VMOVSD_XMM_K1Z_M64: int = 914
 """
 ``VMOVSD xmm1 {k1}{z}, m64``
 
 ``EVEX.LIG.F2.0F.W1 10 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVUPS_XMMM128_XMM: Code = 915 # type: ignore
+MOVUPS_XMMM128_XMM: int = 915
 """
 ``MOVUPS xmm2/m128, xmm1``
 
 ``NP 0F 11 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPS_XMMM128_XMM: Code = 916 # type: ignore
+VEX_VMOVUPS_XMMM128_XMM: int = 916
 """
 ``VMOVUPS xmm2/m128, xmm1``
 
 ``VEX.128.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPS_YMMM256_YMM: Code = 917 # type: ignore
+VEX_VMOVUPS_YMMM256_YMM: int = 917
 """
 ``VMOVUPS ymm2/m256, ymm1``
 
 ``VEX.256.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_XMMM128_K1Z_XMM: Code = 918 # type: ignore
+EVEX_VMOVUPS_XMMM128_K1Z_XMM: int = 918
 """
 ``VMOVUPS xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.0F.W0 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_YMMM256_K1Z_YMM: Code = 919 # type: ignore
+EVEX_VMOVUPS_YMMM256_K1Z_YMM: int = 919
 """
 ``VMOVUPS ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.0F.W0 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPS_ZMMM512_K1Z_ZMM: Code = 920 # type: ignore
+EVEX_VMOVUPS_ZMMM512_K1Z_ZMM: int = 920
 """
 ``VMOVUPS zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.0F.W0 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVUPD_XMMM128_XMM: Code = 921 # type: ignore
+MOVUPD_XMMM128_XMM: int = 921
 """
 ``MOVUPD xmm2/m128, xmm1``
 
 ``66 0F 11 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPD_XMMM128_XMM: Code = 922 # type: ignore
+VEX_VMOVUPD_XMMM128_XMM: int = 922
 """
 ``VMOVUPD xmm2/m128, xmm1``
 
 ``VEX.128.66.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVUPD_YMMM256_YMM: Code = 923 # type: ignore
+VEX_VMOVUPD_YMMM256_YMM: int = 923
 """
 ``VMOVUPD ymm2/m256, ymm1``
 
 ``VEX.256.66.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_XMMM128_K1Z_XMM: Code = 924 # type: ignore
+EVEX_VMOVUPD_XMMM128_K1Z_XMM: int = 924
 """
 ``VMOVUPD xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.66.0F.W1 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_YMMM256_K1Z_YMM: Code = 925 # type: ignore
+EVEX_VMOVUPD_YMMM256_K1Z_YMM: int = 925
 """
 ``VMOVUPD ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.66.0F.W1 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVUPD_ZMMM512_K1Z_ZMM: Code = 926 # type: ignore
+EVEX_VMOVUPD_ZMMM512_K1Z_ZMM: int = 926
 """
 ``VMOVUPD zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.66.0F.W1 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSS_XMMM32_XMM: Code = 927 # type: ignore
+MOVSS_XMMM32_XMM: int = 927
 """
 ``MOVSS xmm2/m32, xmm1``
 
 ``F3 0F 11 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSS_XMM_XMM_XMM_0F11: Code = 928 # type: ignore
+VEX_VMOVSS_XMM_XMM_XMM_0F11: int = 928
 """
 ``VMOVSS xmm1, xmm2, xmm3``
 
 ``VEX.LIG.F3.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSS_M32_XMM: Code = 929 # type: ignore
+VEX_VMOVSS_M32_XMM: int = 929
 """
 ``VMOVSS m32, xmm1``
 
 ``VEX.LIG.F3.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSS_XMM_K1Z_XMM_XMM_0F11: Code = 930 # type: ignore
+EVEX_VMOVSS_XMM_K1Z_XMM_XMM_0F11: int = 930
 """
 ``VMOVSS xmm1 {k1}{z}, xmm2, xmm3``
 
 ``EVEX.LIG.F3.0F.W0 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSS_M32_K1_XMM: Code = 931 # type: ignore
+EVEX_VMOVSS_M32_K1_XMM: int = 931
 """
 ``VMOVSS m32 {k1}, xmm1``
 
 ``EVEX.LIG.F3.0F.W0 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSD_XMMM64_XMM: Code = 932 # type: ignore
+MOVSD_XMMM64_XMM: int = 932
 """
 ``MOVSD xmm1/m64, xmm2``
 
 ``F2 0F 11 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSD_XMM_XMM_XMM_0F11: Code = 933 # type: ignore
+VEX_VMOVSD_XMM_XMM_XMM_0F11: int = 933
 """
 ``VMOVSD xmm1, xmm2, xmm3``
 
 ``VEX.LIG.F2.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSD_M64_XMM: Code = 934 # type: ignore
+VEX_VMOVSD_M64_XMM: int = 934
 """
 ``VMOVSD m64, xmm1``
 
 ``VEX.LIG.F2.0F.WIG 11 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSD_XMM_K1Z_XMM_XMM_0F11: Code = 935 # type: ignore
+EVEX_VMOVSD_XMM_K1Z_XMM_XMM_0F11: int = 935
 """
 ``VMOVSD xmm1 {k1}{z}, xmm2, xmm3``
 
 ``EVEX.LIG.F2.0F.W1 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSD_M64_K1_XMM: Code = 936 # type: ignore
+EVEX_VMOVSD_M64_K1_XMM: int = 936
 """
 ``VMOVSD m64 {k1}, xmm1``
 
 ``EVEX.LIG.F2.0F.W1 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVHLPS_XMM_XMM: Code = 937 # type: ignore
+MOVHLPS_XMM_XMM: int = 937
 """
 ``MOVHLPS xmm1, xmm2``
 
 ``NP 0F 12 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-MOVLPS_XMM_M64: Code = 938 # type: ignore
+MOVLPS_XMM_M64: int = 938
 """
 ``MOVLPS xmm1, m64``
 
 ``NP 0F 12 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVHLPS_XMM_XMM_XMM: Code = 939 # type: ignore
+VEX_VMOVHLPS_XMM_XMM_XMM: int = 939
 """
 ``VMOVHLPS xmm1, xmm2, xmm3``
 
 ``VEX.128.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVLPS_XMM_XMM_M64: Code = 940 # type: ignore
+VEX_VMOVLPS_XMM_XMM_M64: int = 940
 """
 ``VMOVLPS xmm2, xmm1, m64``
 
 ``VEX.128.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVHLPS_XMM_XMM_XMM: Code = 941 # type: ignore
+EVEX_VMOVHLPS_XMM_XMM_XMM: int = 941
 """
 ``VMOVHLPS xmm1, xmm2, xmm3``
 
 ``EVEX.128.0F.W0 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVLPS_XMM_XMM_M64: Code = 942 # type: ignore
+EVEX_VMOVLPS_XMM_XMM_M64: int = 942
 """
 ``VMOVLPS xmm2, xmm1, m64``
 
 ``EVEX.128.0F.W0 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVLPD_XMM_M64: Code = 943 # type: ignore
+MOVLPD_XMM_M64: int = 943
 """
 ``MOVLPD xmm1, m64``
 
 ``66 0F 12 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVLPD_XMM_XMM_M64: Code = 944 # type: ignore
+VEX_VMOVLPD_XMM_XMM_M64: int = 944
 """
 ``VMOVLPD xmm2, xmm1, m64``
 
 ``VEX.128.66.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVLPD_XMM_XMM_M64: Code = 945 # type: ignore
+EVEX_VMOVLPD_XMM_XMM_M64: int = 945
 """
 ``VMOVLPD xmm2, xmm1, m64``
 
 ``EVEX.128.66.0F.W1 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSLDUP_XMM_XMMM128: Code = 946 # type: ignore
+MOVSLDUP_XMM_XMMM128: int = 946
 """
 ``MOVSLDUP xmm1, xmm2/m128``
 
 ``F3 0F 12 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSLDUP_XMM_XMMM128: Code = 947 # type: ignore
+VEX_VMOVSLDUP_XMM_XMMM128: int = 947
 """
 ``VMOVSLDUP xmm1, xmm2/m128``
 
 ``VEX.128.F3.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSLDUP_YMM_YMMM256: Code = 948 # type: ignore
+VEX_VMOVSLDUP_YMM_YMMM256: int = 948
 """
 ``VMOVSLDUP ymm1, ymm2/m256``
 
 ``VEX.256.F3.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSLDUP_XMM_K1Z_XMMM128: Code = 949 # type: ignore
+EVEX_VMOVSLDUP_XMM_K1Z_XMMM128: int = 949
 """
 ``VMOVSLDUP xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F3.0F.W0 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSLDUP_YMM_K1Z_YMMM256: Code = 950 # type: ignore
+EVEX_VMOVSLDUP_YMM_K1Z_YMMM256: int = 950
 """
 ``VMOVSLDUP ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F3.0F.W0 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSLDUP_ZMM_K1Z_ZMMM512: Code = 951 # type: ignore
+EVEX_VMOVSLDUP_ZMM_K1Z_ZMMM512: int = 951
 """
 ``VMOVSLDUP zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F3.0F.W0 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVDDUP_XMM_XMMM64: Code = 952 # type: ignore
+MOVDDUP_XMM_XMMM64: int = 952
 """
 ``MOVDDUP xmm1, xmm2/m64``
 
 ``F2 0F 12 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDDUP_XMM_XMMM64: Code = 953 # type: ignore
+VEX_VMOVDDUP_XMM_XMMM64: int = 953
 """
 ``VMOVDDUP xmm1, xmm2/m64``
 
 ``VEX.128.F2.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDDUP_YMM_YMMM256: Code = 954 # type: ignore
+VEX_VMOVDDUP_YMM_YMMM256: int = 954
 """
 ``VMOVDDUP ymm1, ymm2/m256``
 
 ``VEX.256.F2.0F.WIG 12 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDDUP_XMM_K1Z_XMMM64: Code = 955 # type: ignore
+EVEX_VMOVDDUP_XMM_K1Z_XMMM64: int = 955
 """
 ``VMOVDDUP xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.F2.0F.W1 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDDUP_YMM_K1Z_YMMM256: Code = 956 # type: ignore
+EVEX_VMOVDDUP_YMM_K1Z_YMMM256: int = 956
 """
 ``VMOVDDUP ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F2.0F.W1 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDDUP_ZMM_K1Z_ZMMM512: Code = 957 # type: ignore
+EVEX_VMOVDDUP_ZMM_K1Z_ZMMM512: int = 957
 """
 ``VMOVDDUP zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F2.0F.W1 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVLPS_M64_XMM: Code = 958 # type: ignore
+MOVLPS_M64_XMM: int = 958
 """
 ``MOVLPS m64, xmm1``
 
 ``NP 0F 13 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVLPS_M64_XMM: Code = 959 # type: ignore
+VEX_VMOVLPS_M64_XMM: int = 959
 """
 ``VMOVLPS m64, xmm1``
 
 ``VEX.128.0F.WIG 13 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVLPS_M64_XMM: Code = 960 # type: ignore
+EVEX_VMOVLPS_M64_XMM: int = 960
 """
 ``VMOVLPS m64, xmm1``
 
 ``EVEX.128.0F.W0 13 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVLPD_M64_XMM: Code = 961 # type: ignore
+MOVLPD_M64_XMM: int = 961
 """
 ``MOVLPD m64, xmm1``
 
 ``66 0F 13 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVLPD_M64_XMM: Code = 962 # type: ignore
+VEX_VMOVLPD_M64_XMM: int = 962
 """
 ``VMOVLPD m64, xmm1``
 
 ``VEX.128.66.0F.WIG 13 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVLPD_M64_XMM: Code = 963 # type: ignore
+EVEX_VMOVLPD_M64_XMM: int = 963
 """
 ``VMOVLPD m64, xmm1``
 
 ``EVEX.128.66.0F.W1 13 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UNPCKLPS_XMM_XMMM128: Code = 964 # type: ignore
+UNPCKLPS_XMM_XMMM128: int = 964
 """
 ``UNPCKLPS xmm1, xmm2/m128``
 
 ``NP 0F 14 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKLPS_XMM_XMM_XMMM128: Code = 965 # type: ignore
+VEX_VUNPCKLPS_XMM_XMM_XMMM128: int = 965
 """
 ``VUNPCKLPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 14 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKLPS_YMM_YMM_YMMM256: Code = 966 # type: ignore
+VEX_VUNPCKLPS_YMM_YMM_YMMM256: int = 966
 """
 ``VUNPCKLPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 14 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPS_XMM_K1Z_XMM_XMMM128B32: Code = 967 # type: ignore
+EVEX_VUNPCKLPS_XMM_K1Z_XMM_XMMM128B32: int = 967
 """
 ``VUNPCKLPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPS_YMM_K1Z_YMM_YMMM256B32: Code = 968 # type: ignore
+EVEX_VUNPCKLPS_YMM_K1Z_YMM_YMMM256B32: int = 968
 """
 ``VUNPCKLPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 969 # type: ignore
+EVEX_VUNPCKLPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 969
 """
 ``VUNPCKLPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 14 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UNPCKLPD_XMM_XMMM128: Code = 970 # type: ignore
+UNPCKLPD_XMM_XMMM128: int = 970
 """
 ``UNPCKLPD xmm1, xmm2/m128``
 
 ``66 0F 14 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKLPD_XMM_XMM_XMMM128: Code = 971 # type: ignore
+VEX_VUNPCKLPD_XMM_XMM_XMMM128: int = 971
 """
 ``VUNPCKLPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 14 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKLPD_YMM_YMM_YMMM256: Code = 972 # type: ignore
+VEX_VUNPCKLPD_YMM_YMM_YMMM256: int = 972
 """
 ``VUNPCKLPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 14 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPD_XMM_K1Z_XMM_XMMM128B64: Code = 973 # type: ignore
+EVEX_VUNPCKLPD_XMM_K1Z_XMM_XMMM128B64: int = 973
 """
 ``VUNPCKLPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPD_YMM_K1Z_YMM_YMMM256B64: Code = 974 # type: ignore
+EVEX_VUNPCKLPD_YMM_K1Z_YMM_YMMM256B64: int = 974
 """
 ``VUNPCKLPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKLPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 975 # type: ignore
+EVEX_VUNPCKLPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 975
 """
 ``VUNPCKLPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 14 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UNPCKHPS_XMM_XMMM128: Code = 976 # type: ignore
+UNPCKHPS_XMM_XMMM128: int = 976
 """
 ``UNPCKHPS xmm1, xmm2/m128``
 
 ``NP 0F 15 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKHPS_XMM_XMM_XMMM128: Code = 977 # type: ignore
+VEX_VUNPCKHPS_XMM_XMM_XMMM128: int = 977
 """
 ``VUNPCKHPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 15 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKHPS_YMM_YMM_YMMM256: Code = 978 # type: ignore
+VEX_VUNPCKHPS_YMM_YMM_YMMM256: int = 978
 """
 ``VUNPCKHPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 15 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPS_XMM_K1Z_XMM_XMMM128B32: Code = 979 # type: ignore
+EVEX_VUNPCKHPS_XMM_K1Z_XMM_XMMM128B32: int = 979
 """
 ``VUNPCKHPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPS_YMM_K1Z_YMM_YMMM256B32: Code = 980 # type: ignore
+EVEX_VUNPCKHPS_YMM_K1Z_YMM_YMMM256B32: int = 980
 """
 ``VUNPCKHPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 981 # type: ignore
+EVEX_VUNPCKHPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 981
 """
 ``VUNPCKHPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 15 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UNPCKHPD_XMM_XMMM128: Code = 982 # type: ignore
+UNPCKHPD_XMM_XMMM128: int = 982
 """
 ``UNPCKHPD xmm1, xmm2/m128``
 
 ``66 0F 15 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKHPD_XMM_XMM_XMMM128: Code = 983 # type: ignore
+VEX_VUNPCKHPD_XMM_XMM_XMMM128: int = 983
 """
 ``VUNPCKHPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 15 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VUNPCKHPD_YMM_YMM_YMMM256: Code = 984 # type: ignore
+VEX_VUNPCKHPD_YMM_YMM_YMMM256: int = 984
 """
 ``VUNPCKHPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 15 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPD_XMM_K1Z_XMM_XMMM128B64: Code = 985 # type: ignore
+EVEX_VUNPCKHPD_XMM_K1Z_XMM_XMMM128B64: int = 985
 """
 ``VUNPCKHPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPD_YMM_K1Z_YMM_YMMM256B64: Code = 986 # type: ignore
+EVEX_VUNPCKHPD_YMM_K1Z_YMM_YMMM256B64: int = 986
 """
 ``VUNPCKHPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VUNPCKHPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 987 # type: ignore
+EVEX_VUNPCKHPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 987
 """
 ``VUNPCKHPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 15 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVLHPS_XMM_XMM: Code = 988 # type: ignore
+MOVLHPS_XMM_XMM: int = 988
 """
 ``MOVLHPS xmm1, xmm2``
 
 ``NP 0F 16 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVLHPS_XMM_XMM_XMM: Code = 989 # type: ignore
+VEX_VMOVLHPS_XMM_XMM_XMM: int = 989
 """
 ``VMOVLHPS xmm1, xmm2, xmm3``
 
 ``VEX.128.0F.WIG 16 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVLHPS_XMM_XMM_XMM: Code = 990 # type: ignore
+EVEX_VMOVLHPS_XMM_XMM_XMM: int = 990
 """
 ``VMOVLHPS xmm1, xmm2, xmm3``
 
 ``EVEX.128.0F.W0 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVHPS_XMM_M64: Code = 991 # type: ignore
+MOVHPS_XMM_M64: int = 991
 """
 ``MOVHPS xmm1, m64``
 
 ``NP 0F 16 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVHPS_XMM_XMM_M64: Code = 992 # type: ignore
+VEX_VMOVHPS_XMM_XMM_M64: int = 992
 """
 ``VMOVHPS xmm2, xmm1, m64``
 
 ``VEX.128.0F.WIG 16 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVHPS_XMM_XMM_M64: Code = 993 # type: ignore
+EVEX_VMOVHPS_XMM_XMM_M64: int = 993
 """
 ``VMOVHPS xmm2, xmm1, m64``
 
 ``EVEX.128.0F.W0 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVHPD_XMM_M64: Code = 994 # type: ignore
+MOVHPD_XMM_M64: int = 994
 """
 ``MOVHPD xmm1, m64``
 
 ``66 0F 16 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVHPD_XMM_XMM_M64: Code = 995 # type: ignore
+VEX_VMOVHPD_XMM_XMM_M64: int = 995
 """
 ``VMOVHPD xmm2, xmm1, m64``
 
 ``VEX.128.66.0F.WIG 16 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVHPD_XMM_XMM_M64: Code = 996 # type: ignore
+EVEX_VMOVHPD_XMM_XMM_M64: int = 996
 """
 ``VMOVHPD xmm2, xmm1, m64``
 
 ``EVEX.128.66.0F.W1 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVSHDUP_XMM_XMMM128: Code = 997 # type: ignore
+MOVSHDUP_XMM_XMMM128: int = 997
 """
 ``MOVSHDUP xmm1, xmm2/m128``
 
 ``F3 0F 16 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSHDUP_XMM_XMMM128: Code = 998 # type: ignore
+VEX_VMOVSHDUP_XMM_XMMM128: int = 998
 """
 ``VMOVSHDUP xmm1, xmm2/m128``
 
 ``VEX.128.F3.0F.WIG 16 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVSHDUP_YMM_YMMM256: Code = 999 # type: ignore
+VEX_VMOVSHDUP_YMM_YMMM256: int = 999
 """
 ``VMOVSHDUP ymm1, ymm2/m256``
 
 ``VEX.256.F3.0F.WIG 16 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSHDUP_XMM_K1Z_XMMM128: Code = 1000 # type: ignore
+EVEX_VMOVSHDUP_XMM_K1Z_XMMM128: int = 1000
 """
 ``VMOVSHDUP xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F3.0F.W0 16 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSHDUP_YMM_K1Z_YMMM256: Code = 1001 # type: ignore
+EVEX_VMOVSHDUP_YMM_K1Z_YMMM256: int = 1001
 """
 ``VMOVSHDUP ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F3.0F.W0 16 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVSHDUP_ZMM_K1Z_ZMMM512: Code = 1002 # type: ignore
+EVEX_VMOVSHDUP_ZMM_K1Z_ZMMM512: int = 1002
 """
 ``VMOVSHDUP zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F3.0F.W0 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVHPS_M64_XMM: Code = 1003 # type: ignore
+MOVHPS_M64_XMM: int = 1003
 """
 ``MOVHPS m64, xmm1``
 
 ``NP 0F 17 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVHPS_M64_XMM: Code = 1004 # type: ignore
+VEX_VMOVHPS_M64_XMM: int = 1004
 """
 ``VMOVHPS m64, xmm1``
 
 ``VEX.128.0F.WIG 17 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVHPS_M64_XMM: Code = 1005 # type: ignore
+EVEX_VMOVHPS_M64_XMM: int = 1005
 """
 ``VMOVHPS m64, xmm1``
 
 ``EVEX.128.0F.W0 17 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVHPD_M64_XMM: Code = 1006 # type: ignore
+MOVHPD_M64_XMM: int = 1006
 """
 ``MOVHPD m64, xmm1``
 
 ``66 0F 17 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVHPD_M64_XMM: Code = 1007 # type: ignore
+VEX_VMOVHPD_M64_XMM: int = 1007
 """
 ``VMOVHPD m64, xmm1``
 
 ``VEX.128.66.0F.WIG 17 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVHPD_M64_XMM: Code = 1008 # type: ignore
+EVEX_VMOVHPD_M64_XMM: int = 1008
 """
 ``VMOVHPD m64, xmm1``
 
 ``EVEX.128.66.0F.W1 17 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM16_R16_0F18: Code = 1009 # type: ignore
+RESERVEDNOP_RM16_R16_0F18: int = 1009
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 18 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F18: Code = 1010 # type: ignore
+RESERVEDNOP_RM32_R32_0F18: int = 1010
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 18 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F18: Code = 1011 # type: ignore
+RESERVEDNOP_RM64_R64_0F18: int = 1011
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 18 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F19: Code = 1012 # type: ignore
+RESERVEDNOP_RM16_R16_0F19: int = 1012
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 19 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F19: Code = 1013 # type: ignore
+RESERVEDNOP_RM32_R32_0F19: int = 1013
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 19 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F19: Code = 1014 # type: ignore
+RESERVEDNOP_RM64_R64_0F19: int = 1014
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 19 /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1A: Code = 1015 # type: ignore
+RESERVEDNOP_RM16_R16_0F1A: int = 1015
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1A /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1A: Code = 1016 # type: ignore
+RESERVEDNOP_RM32_R32_0F1A: int = 1016
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1A /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1A: Code = 1017 # type: ignore
+RESERVEDNOP_RM64_R64_0F1A: int = 1017
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1A /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1B: Code = 1018 # type: ignore
+RESERVEDNOP_RM16_R16_0F1B: int = 1018
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1B /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1B: Code = 1019 # type: ignore
+RESERVEDNOP_RM32_R32_0F1B: int = 1019
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1B /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1B: Code = 1020 # type: ignore
+RESERVEDNOP_RM64_R64_0F1B: int = 1020
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1B /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1C: Code = 1021 # type: ignore
+RESERVEDNOP_RM16_R16_0F1C: int = 1021
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1C /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1C: Code = 1022 # type: ignore
+RESERVEDNOP_RM32_R32_0F1C: int = 1022
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1C /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1C: Code = 1023 # type: ignore
+RESERVEDNOP_RM64_R64_0F1C: int = 1023
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1C /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1D: Code = 1024 # type: ignore
+RESERVEDNOP_RM16_R16_0F1D: int = 1024
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1D: Code = 1025 # type: ignore
+RESERVEDNOP_RM32_R32_0F1D: int = 1025
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1D: Code = 1026 # type: ignore
+RESERVEDNOP_RM64_R64_0F1D: int = 1026
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1D /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1E: Code = 1027 # type: ignore
+RESERVEDNOP_RM16_R16_0F1E: int = 1027
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1E /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1E: Code = 1028 # type: ignore
+RESERVEDNOP_RM32_R32_0F1E: int = 1028
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1E /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1E: Code = 1029 # type: ignore
+RESERVEDNOP_RM64_R64_0F1E: int = 1029
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1E /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-RESERVEDNOP_RM16_R16_0F1F: Code = 1030 # type: ignore
+RESERVEDNOP_RM16_R16_0F1F: int = 1030
 """
 ``RESERVEDNOP r/m16, r16``
 
 ``o16 0F 1F /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM32_R32_0F1F: Code = 1031 # type: ignore
+RESERVEDNOP_RM32_R32_0F1F: int = 1031
 """
 ``RESERVEDNOP r/m32, r32``
 
 ``o32 0F 1F /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-RESERVEDNOP_RM64_R64_0F1F: Code = 1032 # type: ignore
+RESERVEDNOP_RM64_R64_0F1F: int = 1032
 """
 ``RESERVEDNOP r/m64, r64``
 
 ``o64 0F 1F /r``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-PREFETCHNTA_M8: Code = 1033 # type: ignore
+PREFETCHNTA_M8: int = 1033
 """
 ``PREFETCHNTA m8``
 
 ``0F 18 /0``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PREFETCHT0_M8: Code = 1034 # type: ignore
+PREFETCHT0_M8: int = 1034
 """
 ``PREFETCHT0 m8``
 
 ``0F 18 /1``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PREFETCHT1_M8: Code = 1035 # type: ignore
+PREFETCHT1_M8: int = 1035
 """
 ``PREFETCHT1 m8``
 
 ``0F 18 /2``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PREFETCHT2_M8: Code = 1036 # type: ignore
+PREFETCHT2_M8: int = 1036
 """
 ``PREFETCHT2 m8``
 
 ``0F 18 /3``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-BNDLDX_BND_MIB: Code = 1037 # type: ignore
+BNDLDX_BND_MIB: int = 1037
 """
 ``BNDLDX bnd, mib``
 
 ``NP 0F 1A /r``
 
 ``MPX``
 
 ``16/32/64-bit``
 """
-BNDMOV_BND_BNDM64: Code = 1038 # type: ignore
+BNDMOV_BND_BNDM64: int = 1038
 """
 ``BNDMOV bnd1, bnd2/m64``
 
 ``66 0F 1A /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDMOV_BND_BNDM128: Code = 1039 # type: ignore
+BNDMOV_BND_BNDM128: int = 1039
 """
 ``BNDMOV bnd1, bnd2/m128``
 
 ``66 0F 1A /r``
 
 ``MPX``
 
 ``64-bit``
 """
-BNDCL_BND_RM32: Code = 1040 # type: ignore
+BNDCL_BND_RM32: int = 1040
 """
 ``BNDCL bnd, r/m32``
 
 ``F3 0F 1A /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDCL_BND_RM64: Code = 1041 # type: ignore
+BNDCL_BND_RM64: int = 1041
 """
 ``BNDCL bnd, r/m64``
 
 ``F3 0F 1A /r``
 
 ``MPX``
 
 ``64-bit``
 """
-BNDCU_BND_RM32: Code = 1042 # type: ignore
+BNDCU_BND_RM32: int = 1042
 """
 ``BNDCU bnd, r/m32``
 
 ``F2 0F 1A /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDCU_BND_RM64: Code = 1043 # type: ignore
+BNDCU_BND_RM64: int = 1043
 """
 ``BNDCU bnd, r/m64``
 
 ``F2 0F 1A /r``
 
 ``MPX``
 
 ``64-bit``
 """
-BNDSTX_MIB_BND: Code = 1044 # type: ignore
+BNDSTX_MIB_BND: int = 1044
 """
 ``BNDSTX mib, bnd``
 
 ``NP 0F 1B /r``
 
 ``MPX``
 
 ``16/32/64-bit``
 """
-BNDMOV_BNDM64_BND: Code = 1045 # type: ignore
+BNDMOV_BNDM64_BND: int = 1045
 """
 ``BNDMOV bnd1/m64, bnd2``
 
 ``66 0F 1B /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDMOV_BNDM128_BND: Code = 1046 # type: ignore
+BNDMOV_BNDM128_BND: int = 1046
 """
 ``BNDMOV bnd1/m128, bnd2``
 
 ``66 0F 1B /r``
 
 ``MPX``
 
 ``64-bit``
 """
-BNDMK_BND_M32: Code = 1047 # type: ignore
+BNDMK_BND_M32: int = 1047
 """
 ``BNDMK bnd, m32``
 
 ``F3 0F 1B /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDMK_BND_M64: Code = 1048 # type: ignore
+BNDMK_BND_M64: int = 1048
 """
 ``BNDMK bnd, m64``
 
 ``F3 0F 1B /r``
 
 ``MPX``
 
 ``64-bit``
 """
-BNDCN_BND_RM32: Code = 1049 # type: ignore
+BNDCN_BND_RM32: int = 1049
 """
 ``BNDCN bnd, r/m32``
 
 ``F2 0F 1B /r``
 
 ``MPX``
 
 ``16/32-bit``
 """
-BNDCN_BND_RM64: Code = 1050 # type: ignore
+BNDCN_BND_RM64: int = 1050
 """
 ``BNDCN bnd, r/m64``
 
 ``F2 0F 1B /r``
 
 ``MPX``
 
 ``64-bit``
 """
-CLDEMOTE_M8: Code = 1051 # type: ignore
+CLDEMOTE_M8: int = 1051
 """
 ``CLDEMOTE m8``
 
 ``NP 0F 1C /0``
 
 ``CLDEMOTE``
 
 ``16/32/64-bit``
 """
-RDSSPD_R32: Code = 1052 # type: ignore
+RDSSPD_R32: int = 1052
 """
 ``RDSSPD r32``
 
 ``F3 0F 1E /1``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-RDSSPQ_R64: Code = 1053 # type: ignore
+RDSSPQ_R64: int = 1053
 """
 ``RDSSPQ r64``
 
 ``F3 o64 0F 1E /1``
 
 ``CET_SS``
 
 ``64-bit``
 """
-ENDBR64: Code = 1054 # type: ignore
+ENDBR64: int = 1054
 """
 ``ENDBR64``
 
 ``F3 0F 1E FA``
 
 ``CET_IBT``
 
 ``16/32/64-bit``
 """
-ENDBR32: Code = 1055 # type: ignore
+ENDBR32: int = 1055
 """
 ``ENDBR32``
 
 ``F3 0F 1E FB``
 
 ``CET_IBT``
 
 ``16/32/64-bit``
 """
-NOP_RM16: Code = 1056 # type: ignore
+NOP_RM16: int = 1056
 """
 ``NOP r/m16``
 
 ``o16 0F 1F /0``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-NOP_RM32: Code = 1057 # type: ignore
+NOP_RM32: int = 1057
 """
 ``NOP r/m32``
 
 ``o32 0F 1F /0``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``16/32/64-bit``
 """
-NOP_RM64: Code = 1058 # type: ignore
+NOP_RM64: int = 1058
 """
 ``NOP r/m64``
 
 ``o64 0F 1F /0``
 
 ``CPUID.01H.EAX[Bits 11:8] = 0110B or 1111B``
 
 ``64-bit``
 """
-MOV_R32_CR: Code = 1059 # type: ignore
+MOV_R32_CR: int = 1059
 """
 ``MOV r32, cr``
 
 ``0F 20 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOV_R64_CR: Code = 1060 # type: ignore
+MOV_R64_CR: int = 1060
 """
 ``MOV r64, cr``
 
 ``0F 20 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_R32_DR: Code = 1061 # type: ignore
+MOV_R32_DR: int = 1061
 """
 ``MOV r32, dr``
 
 ``0F 21 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOV_R64_DR: Code = 1062 # type: ignore
+MOV_R64_DR: int = 1062
 """
 ``MOV r64, dr``
 
 ``0F 21 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_CR_R32: Code = 1063 # type: ignore
+MOV_CR_R32: int = 1063
 """
 ``MOV cr, r32``
 
 ``0F 22 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOV_CR_R64: Code = 1064 # type: ignore
+MOV_CR_R64: int = 1064
 """
 ``MOV cr, r64``
 
 ``0F 22 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_DR_R32: Code = 1065 # type: ignore
+MOV_DR_R32: int = 1065
 """
 ``MOV dr, r32``
 
 ``0F 23 /r``
 
 ``386+``
 
 ``16/32-bit``
 """
-MOV_DR_R64: Code = 1066 # type: ignore
+MOV_DR_R64: int = 1066
 """
 ``MOV dr, r64``
 
 ``0F 23 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOV_R32_TR: Code = 1067 # type: ignore
+MOV_R32_TR: int = 1067
 """
 ``MOV r32, tr``
 
 ``0F 24 /r``
 
 ``386/486/Cyrix/Geode``
 
 ``16/32-bit``
 """
-MOV_TR_R32: Code = 1068 # type: ignore
+MOV_TR_R32: int = 1068
 """
 ``MOV tr, r32``
 
 ``0F 26 /r``
 
 ``386/486/Cyrix/Geode``
 
 ``16/32-bit``
 """
-MOVAPS_XMM_XMMM128: Code = 1069 # type: ignore
+MOVAPS_XMM_XMMM128: int = 1069
 """
 ``MOVAPS xmm1, xmm2/m128``
 
 ``NP 0F 28 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPS_XMM_XMMM128: Code = 1070 # type: ignore
+VEX_VMOVAPS_XMM_XMMM128: int = 1070
 """
 ``VMOVAPS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 28 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPS_YMM_YMMM256: Code = 1071 # type: ignore
+VEX_VMOVAPS_YMM_YMMM256: int = 1071
 """
 ``VMOVAPS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 28 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_XMM_K1Z_XMMM128: Code = 1072 # type: ignore
+EVEX_VMOVAPS_XMM_K1Z_XMMM128: int = 1072
 """
 ``VMOVAPS xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.0F.W0 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_YMM_K1Z_YMMM256: Code = 1073 # type: ignore
+EVEX_VMOVAPS_YMM_K1Z_YMMM256: int = 1073
 """
 ``VMOVAPS ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.0F.W0 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_ZMM_K1Z_ZMMM512: Code = 1074 # type: ignore
+EVEX_VMOVAPS_ZMM_K1Z_ZMMM512: int = 1074
 """
 ``VMOVAPS zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.0F.W0 28 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVAPD_XMM_XMMM128: Code = 1075 # type: ignore
+MOVAPD_XMM_XMMM128: int = 1075
 """
 ``MOVAPD xmm1, xmm2/m128``
 
 ``66 0F 28 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPD_XMM_XMMM128: Code = 1076 # type: ignore
+VEX_VMOVAPD_XMM_XMMM128: int = 1076
 """
 ``VMOVAPD xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 28 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPD_YMM_YMMM256: Code = 1077 # type: ignore
+VEX_VMOVAPD_YMM_YMMM256: int = 1077
 """
 ``VMOVAPD ymm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 28 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_XMM_K1Z_XMMM128: Code = 1078 # type: ignore
+EVEX_VMOVAPD_XMM_K1Z_XMMM128: int = 1078
 """
 ``VMOVAPD xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F.W1 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_YMM_K1Z_YMMM256: Code = 1079 # type: ignore
+EVEX_VMOVAPD_YMM_K1Z_YMMM256: int = 1079
 """
 ``VMOVAPD ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F.W1 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_ZMM_K1Z_ZMMM512: Code = 1080 # type: ignore
+EVEX_VMOVAPD_ZMM_K1Z_ZMMM512: int = 1080
 """
 ``VMOVAPD zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F.W1 28 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVAPS_XMMM128_XMM: Code = 1081 # type: ignore
+MOVAPS_XMMM128_XMM: int = 1081
 """
 ``MOVAPS xmm2/m128, xmm1``
 
 ``NP 0F 29 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPS_XMMM128_XMM: Code = 1082 # type: ignore
+VEX_VMOVAPS_XMMM128_XMM: int = 1082
 """
 ``VMOVAPS xmm2/m128, xmm1``
 
 ``VEX.128.0F.WIG 29 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPS_YMMM256_YMM: Code = 1083 # type: ignore
+VEX_VMOVAPS_YMMM256_YMM: int = 1083
 """
 ``VMOVAPS ymm2/m256, ymm1``
 
 ``VEX.256.0F.WIG 29 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_XMMM128_K1Z_XMM: Code = 1084 # type: ignore
+EVEX_VMOVAPS_XMMM128_K1Z_XMM: int = 1084
 """
 ``VMOVAPS xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.0F.W0 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_YMMM256_K1Z_YMM: Code = 1085 # type: ignore
+EVEX_VMOVAPS_YMMM256_K1Z_YMM: int = 1085
 """
 ``VMOVAPS ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.0F.W0 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPS_ZMMM512_K1Z_ZMM: Code = 1086 # type: ignore
+EVEX_VMOVAPS_ZMMM512_K1Z_ZMM: int = 1086
 """
 ``VMOVAPS zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.0F.W0 29 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVAPD_XMMM128_XMM: Code = 1087 # type: ignore
+MOVAPD_XMMM128_XMM: int = 1087
 """
 ``MOVAPD xmm2/m128, xmm1``
 
 ``66 0F 29 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPD_XMMM128_XMM: Code = 1088 # type: ignore
+VEX_VMOVAPD_XMMM128_XMM: int = 1088
 """
 ``VMOVAPD xmm2/m128, xmm1``
 
 ``VEX.128.66.0F.WIG 29 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVAPD_YMMM256_YMM: Code = 1089 # type: ignore
+VEX_VMOVAPD_YMMM256_YMM: int = 1089
 """
 ``VMOVAPD ymm2/m256, ymm1``
 
 ``VEX.256.66.0F.WIG 29 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_XMMM128_K1Z_XMM: Code = 1090 # type: ignore
+EVEX_VMOVAPD_XMMM128_K1Z_XMM: int = 1090
 """
 ``VMOVAPD xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.66.0F.W1 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_YMMM256_K1Z_YMM: Code = 1091 # type: ignore
+EVEX_VMOVAPD_YMMM256_K1Z_YMM: int = 1091
 """
 ``VMOVAPD ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.66.0F.W1 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVAPD_ZMMM512_K1Z_ZMM: Code = 1092 # type: ignore
+EVEX_VMOVAPD_ZMMM512_K1Z_ZMM: int = 1092
 """
 ``VMOVAPD zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.66.0F.W1 29 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTPI2PS_XMM_MMM64: Code = 1093 # type: ignore
+CVTPI2PS_XMM_MMM64: int = 1093
 """
 ``CVTPI2PS xmm, mm/m64``
 
 ``NP 0F 2A /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTPI2PD_XMM_MMM64: Code = 1094 # type: ignore
+CVTPI2PD_XMM_MMM64: int = 1094
 """
 ``CVTPI2PD xmm, mm/m64``
 
 ``66 0F 2A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTSI2SS_XMM_RM32: Code = 1095 # type: ignore
+CVTSI2SS_XMM_RM32: int = 1095
 """
 ``CVTSI2SS xmm1, r/m32``
 
 ``F3 0F 2A /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTSI2SS_XMM_RM64: Code = 1096 # type: ignore
+CVTSI2SS_XMM_RM64: int = 1096
 """
 ``CVTSI2SS xmm1, r/m64``
 
 ``F3 o64 0F 2A /r``
 
 ``SSE``
 
 ``64-bit``
 """
-VEX_VCVTSI2SS_XMM_XMM_RM32: Code = 1097 # type: ignore
+VEX_VCVTSI2SS_XMM_XMM_RM32: int = 1097
 """
 ``VCVTSI2SS xmm1, xmm2, r/m32``
 
 ``VEX.LIG.F3.0F.W0 2A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSI2SS_XMM_XMM_RM64: Code = 1098 # type: ignore
+VEX_VCVTSI2SS_XMM_XMM_RM64: int = 1098
 """
 ``VCVTSI2SS xmm1, xmm2, r/m64``
 
 ``VEX.LIG.F3.0F.W1 2A /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTSI2SS_XMM_XMM_RM32_ER: Code = 1099 # type: ignore
+EVEX_VCVTSI2SS_XMM_XMM_RM32_ER: int = 1099
 """
 ``VCVTSI2SS xmm1, xmm2, r/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 2A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSI2SS_XMM_XMM_RM64_ER: Code = 1100 # type: ignore
+EVEX_VCVTSI2SS_XMM_XMM_RM64_ER: int = 1100
 """
 ``VCVTSI2SS xmm1, xmm2, r/m64{er}``
 
 ``EVEX.LIG.F3.0F.W1 2A /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-CVTSI2SD_XMM_RM32: Code = 1101 # type: ignore
+CVTSI2SD_XMM_RM32: int = 1101
 """
 ``CVTSI2SD xmm1, r/m32``
 
 ``F2 0F 2A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTSI2SD_XMM_RM64: Code = 1102 # type: ignore
+CVTSI2SD_XMM_RM64: int = 1102
 """
 ``CVTSI2SD xmm1, r/m64``
 
 ``F2 o64 0F 2A /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VCVTSI2SD_XMM_XMM_RM32: Code = 1103 # type: ignore
+VEX_VCVTSI2SD_XMM_XMM_RM32: int = 1103
 """
 ``VCVTSI2SD xmm1, xmm2, r/m32``
 
 ``VEX.LIG.F2.0F.W0 2A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSI2SD_XMM_XMM_RM64: Code = 1104 # type: ignore
+VEX_VCVTSI2SD_XMM_XMM_RM64: int = 1104
 """
 ``VCVTSI2SD xmm1, xmm2, r/m64``
 
 ``VEX.LIG.F2.0F.W1 2A /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTSI2SD_XMM_XMM_RM32_ER: Code = 1105 # type: ignore
+EVEX_VCVTSI2SD_XMM_XMM_RM32_ER: int = 1105
 """
 ``VCVTSI2SD xmm1, xmm2, r/m32{er}``
 
 ``EVEX.LIG.F2.0F.W0 2A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSI2SD_XMM_XMM_RM64_ER: Code = 1106 # type: ignore
+EVEX_VCVTSI2SD_XMM_XMM_RM64_ER: int = 1106
 """
 ``VCVTSI2SD xmm1, xmm2, r/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 2A /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-MOVNTPS_M128_XMM: Code = 1107 # type: ignore
+MOVNTPS_M128_XMM: int = 1107
 """
 ``MOVNTPS m128, xmm1``
 
 ``NP 0F 2B /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTPS_M128_XMM: Code = 1108 # type: ignore
+VEX_VMOVNTPS_M128_XMM: int = 1108
 """
 ``VMOVNTPS m128, xmm1``
 
 ``VEX.128.0F.WIG 2B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTPS_M256_YMM: Code = 1109 # type: ignore
+VEX_VMOVNTPS_M256_YMM: int = 1109
 """
 ``VMOVNTPS m256, ymm1``
 
 ``VEX.256.0F.WIG 2B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPS_M128_XMM: Code = 1110 # type: ignore
+EVEX_VMOVNTPS_M128_XMM: int = 1110
 """
 ``VMOVNTPS m128, xmm1``
 
 ``EVEX.128.0F.W0 2B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPS_M256_YMM: Code = 1111 # type: ignore
+EVEX_VMOVNTPS_M256_YMM: int = 1111
 """
 ``VMOVNTPS m256, ymm1``
 
 ``EVEX.256.0F.W0 2B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPS_M512_ZMM: Code = 1112 # type: ignore
+EVEX_VMOVNTPS_M512_ZMM: int = 1112
 """
 ``VMOVNTPS m512, zmm1``
 
 ``EVEX.512.0F.W0 2B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVNTPD_M128_XMM: Code = 1113 # type: ignore
+MOVNTPD_M128_XMM: int = 1113
 """
 ``MOVNTPD m128, xmm1``
 
 ``66 0F 2B /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTPD_M128_XMM: Code = 1114 # type: ignore
+VEX_VMOVNTPD_M128_XMM: int = 1114
 """
 ``VMOVNTPD m128, xmm1``
 
 ``VEX.128.66.0F.WIG 2B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTPD_M256_YMM: Code = 1115 # type: ignore
+VEX_VMOVNTPD_M256_YMM: int = 1115
 """
 ``VMOVNTPD m256, ymm1``
 
 ``VEX.256.66.0F.WIG 2B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPD_M128_XMM: Code = 1116 # type: ignore
+EVEX_VMOVNTPD_M128_XMM: int = 1116
 """
 ``VMOVNTPD m128, xmm1``
 
 ``EVEX.128.66.0F.W1 2B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPD_M256_YMM: Code = 1117 # type: ignore
+EVEX_VMOVNTPD_M256_YMM: int = 1117
 """
 ``VMOVNTPD m256, ymm1``
 
 ``EVEX.256.66.0F.W1 2B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTPD_M512_ZMM: Code = 1118 # type: ignore
+EVEX_VMOVNTPD_M512_ZMM: int = 1118
 """
 ``VMOVNTPD m512, zmm1``
 
 ``EVEX.512.66.0F.W1 2B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVNTSS_M32_XMM: Code = 1119 # type: ignore
+MOVNTSS_M32_XMM: int = 1119
 """
 ``MOVNTSS m32, xmm1``
 
 ``F3 0F 2B /r``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-MOVNTSD_M64_XMM: Code = 1120 # type: ignore
+MOVNTSD_M64_XMM: int = 1120
 """
 ``MOVNTSD m64, xmm1``
 
 ``F2 0F 2B /r``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-CVTTPS2PI_MM_XMMM64: Code = 1121 # type: ignore
+CVTTPS2PI_MM_XMMM64: int = 1121
 """
 ``CVTTPS2PI mm, xmm/m64``
 
 ``NP 0F 2C /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTTPD2PI_MM_XMMM128: Code = 1122 # type: ignore
+CVTTPD2PI_MM_XMMM128: int = 1122
 """
 ``CVTTPD2PI mm, xmm/m128``
 
 ``66 0F 2C /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTTSS2SI_R32_XMMM32: Code = 1123 # type: ignore
+CVTTSS2SI_R32_XMMM32: int = 1123
 """
 ``CVTTSS2SI r32, xmm1/m32``
 
 ``F3 0F 2C /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTTSS2SI_R64_XMMM32: Code = 1124 # type: ignore
+CVTTSS2SI_R64_XMMM32: int = 1124
 """
 ``CVTTSS2SI r64, xmm1/m32``
 
 ``F3 o64 0F 2C /r``
 
 ``SSE``
 
 ``64-bit``
 """
-VEX_VCVTTSS2SI_R32_XMMM32: Code = 1125 # type: ignore
+VEX_VCVTTSS2SI_R32_XMMM32: int = 1125
 """
 ``VCVTTSS2SI r32, xmm1/m32``
 
 ``VEX.LIG.F3.0F.W0 2C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTSS2SI_R64_XMMM32: Code = 1126 # type: ignore
+VEX_VCVTTSS2SI_R64_XMMM32: int = 1126
 """
 ``VCVTTSS2SI r64, xmm1/m32``
 
 ``VEX.LIG.F3.0F.W1 2C /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTTSS2SI_R32_XMMM32_SAE: Code = 1127 # type: ignore
+EVEX_VCVTTSS2SI_R32_XMMM32_SAE: int = 1127
 """
 ``VCVTTSS2SI r32, xmm1/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W0 2C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSS2SI_R64_XMMM32_SAE: Code = 1128 # type: ignore
+EVEX_VCVTTSS2SI_R64_XMMM32_SAE: int = 1128
 """
 ``VCVTTSS2SI r64, xmm1/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W1 2C /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-CVTTSD2SI_R32_XMMM64: Code = 1129 # type: ignore
+CVTTSD2SI_R32_XMMM64: int = 1129
 """
 ``CVTTSD2SI r32, xmm1/m64``
 
 ``F2 0F 2C /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTTSD2SI_R64_XMMM64: Code = 1130 # type: ignore
+CVTTSD2SI_R64_XMMM64: int = 1130
 """
 ``CVTTSD2SI r64, xmm1/m64``
 
 ``F2 o64 0F 2C /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VCVTTSD2SI_R32_XMMM64: Code = 1131 # type: ignore
+VEX_VCVTTSD2SI_R32_XMMM64: int = 1131
 """
 ``VCVTTSD2SI r32, xmm1/m64``
 
 ``VEX.LIG.F2.0F.W0 2C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTSD2SI_R64_XMMM64: Code = 1132 # type: ignore
+VEX_VCVTTSD2SI_R64_XMMM64: int = 1132
 """
 ``VCVTTSD2SI r64, xmm1/m64``
 
 ``VEX.LIG.F2.0F.W1 2C /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTTSD2SI_R32_XMMM64_SAE: Code = 1133 # type: ignore
+EVEX_VCVTTSD2SI_R32_XMMM64_SAE: int = 1133
 """
 ``VCVTTSD2SI r32, xmm1/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W0 2C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSD2SI_R64_XMMM64_SAE: Code = 1134 # type: ignore
+EVEX_VCVTTSD2SI_R64_XMMM64_SAE: int = 1134
 """
 ``VCVTTSD2SI r64, xmm1/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W1 2C /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-CVTPS2PI_MM_XMMM64: Code = 1135 # type: ignore
+CVTPS2PI_MM_XMMM64: int = 1135
 """
 ``CVTPS2PI mm, xmm/m64``
 
 ``NP 0F 2D /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTPD2PI_MM_XMMM128: Code = 1136 # type: ignore
+CVTPD2PI_MM_XMMM128: int = 1136
 """
 ``CVTPD2PI mm, xmm/m128``
 
 ``66 0F 2D /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTSS2SI_R32_XMMM32: Code = 1137 # type: ignore
+CVTSS2SI_R32_XMMM32: int = 1137
 """
 ``CVTSS2SI r32, xmm1/m32``
 
 ``F3 0F 2D /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-CVTSS2SI_R64_XMMM32: Code = 1138 # type: ignore
+CVTSS2SI_R64_XMMM32: int = 1138
 """
 ``CVTSS2SI r64, xmm1/m32``
 
 ``F3 o64 0F 2D /r``
 
 ``SSE``
 
 ``64-bit``
 """
-VEX_VCVTSS2SI_R32_XMMM32: Code = 1139 # type: ignore
+VEX_VCVTSS2SI_R32_XMMM32: int = 1139
 """
 ``VCVTSS2SI r32, xmm1/m32``
 
 ``VEX.LIG.F3.0F.W0 2D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSS2SI_R64_XMMM32: Code = 1140 # type: ignore
+VEX_VCVTSS2SI_R64_XMMM32: int = 1140
 """
 ``VCVTSS2SI r64, xmm1/m32``
 
 ``VEX.LIG.F3.0F.W1 2D /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTSS2SI_R32_XMMM32_ER: Code = 1141 # type: ignore
+EVEX_VCVTSS2SI_R32_XMMM32_ER: int = 1141
 """
 ``VCVTSS2SI r32, xmm1/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 2D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSS2SI_R64_XMMM32_ER: Code = 1142 # type: ignore
+EVEX_VCVTSS2SI_R64_XMMM32_ER: int = 1142
 """
 ``VCVTSS2SI r64, xmm1/m32{er}``
 
 ``EVEX.LIG.F3.0F.W1 2D /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-CVTSD2SI_R32_XMMM64: Code = 1143 # type: ignore
+CVTSD2SI_R32_XMMM64: int = 1143
 """
 ``CVTSD2SI r32, xmm1/m64``
 
 ``F2 0F 2D /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-CVTSD2SI_R64_XMMM64: Code = 1144 # type: ignore
+CVTSD2SI_R64_XMMM64: int = 1144
 """
 ``CVTSD2SI r64, xmm1/m64``
 
 ``F2 o64 0F 2D /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VCVTSD2SI_R32_XMMM64: Code = 1145 # type: ignore
+VEX_VCVTSD2SI_R32_XMMM64: int = 1145
 """
 ``VCVTSD2SI r32, xmm1/m64``
 
 ``VEX.LIG.F2.0F.W0 2D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSD2SI_R64_XMMM64: Code = 1146 # type: ignore
+VEX_VCVTSD2SI_R64_XMMM64: int = 1146
 """
 ``VCVTSD2SI r64, xmm1/m64``
 
 ``VEX.LIG.F2.0F.W1 2D /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VCVTSD2SI_R32_XMMM64_ER: Code = 1147 # type: ignore
+EVEX_VCVTSD2SI_R32_XMMM64_ER: int = 1147
 """
 ``VCVTSD2SI r32, xmm1/m64{er}``
 
 ``EVEX.LIG.F2.0F.W0 2D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSD2SI_R64_XMMM64_ER: Code = 1148 # type: ignore
+EVEX_VCVTSD2SI_R64_XMMM64_ER: int = 1148
 """
 ``VCVTSD2SI r64, xmm1/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 2D /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-UCOMISS_XMM_XMMM32: Code = 1149 # type: ignore
+UCOMISS_XMM_XMMM32: int = 1149
 """
 ``UCOMISS xmm1, xmm2/m32``
 
 ``NP 0F 2E /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VUCOMISS_XMM_XMMM32: Code = 1150 # type: ignore
+VEX_VUCOMISS_XMM_XMMM32: int = 1150
 """
 ``VUCOMISS xmm1, xmm2/m32``
 
 ``VEX.LIG.0F.WIG 2E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUCOMISS_XMM_XMMM32_SAE: Code = 1151 # type: ignore
+EVEX_VUCOMISS_XMM_XMMM32_SAE: int = 1151
 """
 ``VUCOMISS xmm1, xmm2/m32{sae}``
 
 ``EVEX.LIG.0F.W0 2E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UCOMISD_XMM_XMMM64: Code = 1152 # type: ignore
+UCOMISD_XMM_XMMM64: int = 1152
 """
 ``UCOMISD xmm1, xmm2/m64``
 
 ``66 0F 2E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VUCOMISD_XMM_XMMM64: Code = 1153 # type: ignore
+VEX_VUCOMISD_XMM_XMMM64: int = 1153
 """
 ``VUCOMISD xmm1, xmm2/m64``
 
 ``VEX.LIG.66.0F.WIG 2E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VUCOMISD_XMM_XMMM64_SAE: Code = 1154 # type: ignore
+EVEX_VUCOMISD_XMM_XMMM64_SAE: int = 1154
 """
 ``VUCOMISD xmm1, xmm2/m64{sae}``
 
 ``EVEX.LIG.66.0F.W1 2E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-COMISS_XMM_XMMM32: Code = 1155 # type: ignore
+COMISS_XMM_XMMM32: int = 1155
 """
 ``COMISS xmm1, xmm2/m32``
 
 ``NP 0F 2F /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-COMISD_XMM_XMMM64: Code = 1156 # type: ignore
+COMISD_XMM_XMMM64: int = 1156
 """
 ``COMISD xmm1, xmm2/m64``
 
 ``66 0F 2F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCOMISS_XMM_XMMM32: Code = 1157 # type: ignore
+VEX_VCOMISS_XMM_XMMM32: int = 1157
 """
 ``VCOMISS xmm1, xmm2/m32``
 
 ``VEX.LIG.0F.WIG 2F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCOMISD_XMM_XMMM64: Code = 1158 # type: ignore
+VEX_VCOMISD_XMM_XMMM64: int = 1158
 """
 ``VCOMISD xmm1, xmm2/m64``
 
 ``VEX.LIG.66.0F.WIG 2F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMISS_XMM_XMMM32_SAE: Code = 1159 # type: ignore
+EVEX_VCOMISS_XMM_XMMM32_SAE: int = 1159
 """
 ``VCOMISS xmm1, xmm2/m32{sae}``
 
 ``EVEX.LIG.0F.W0 2F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMISD_XMM_XMMM64_SAE: Code = 1160 # type: ignore
+EVEX_VCOMISD_XMM_XMMM64_SAE: int = 1160
 """
 ``VCOMISD xmm1, xmm2/m64{sae}``
 
 ``EVEX.LIG.66.0F.W1 2F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-WRMSR: Code = 1161 # type: ignore
+WRMSR: int = 1161
 """
 ``WRMSR``
 
 ``0F 30``
 
 ``MSR``
 
 ``16/32/64-bit``
 """
-RDTSC: Code = 1162 # type: ignore
+RDTSC: int = 1162
 """
 ``RDTSC``
 
 ``0F 31``
 
 ``TSC``
 
 ``16/32/64-bit``
 """
-RDMSR: Code = 1163 # type: ignore
+RDMSR: int = 1163
 """
 ``RDMSR``
 
 ``0F 32``
 
 ``MSR``
 
 ``16/32/64-bit``
 """
-RDPMC: Code = 1164 # type: ignore
+RDPMC: int = 1164
 """
 ``RDPMC``
 
 ``0F 33``
 
 ``Pentium MMX or later, or Pentium Pro or later``
 
 ``16/32/64-bit``
 """
-SYSENTER: Code = 1165 # type: ignore
+SYSENTER: int = 1165
 """
 ``SYSENTER``
 
 ``0F 34``
 
 ``SEP``
 
 ``16/32/64-bit``
 """
-SYSEXITD: Code = 1166 # type: ignore
+SYSEXITD: int = 1166
 """
 ``SYSEXIT``
 
 ``0F 35``
 
 ``SEP``
 
 ``16/32/64-bit``
 """
-SYSEXITQ: Code = 1167 # type: ignore
+SYSEXITQ: int = 1167
 """
 ``SYSEXITQ``
 
 ``o64 0F 35``
 
 ``SEP``
 
 ``64-bit``
 """
-GETSECD: Code = 1168 # type: ignore
+GETSECD: int = 1168
 """
 ``GETSEC``
 
 ``NP 0F 37``
 
 ``SMX``
 
 ``16/32/64-bit``
 """
-CMOVO_R16_RM16: Code = 1169 # type: ignore
+CMOVO_R16_RM16: int = 1169
 """
 ``CMOVO r16, r/m16``
 
 ``o16 0F 40 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVO_R32_RM32: Code = 1170 # type: ignore
+CMOVO_R32_RM32: int = 1170
 """
 ``CMOVO r32, r/m32``
 
 ``o32 0F 40 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVO_R64_RM64: Code = 1171 # type: ignore
+CMOVO_R64_RM64: int = 1171
 """
 ``CMOVO r64, r/m64``
 
 ``o64 0F 40 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVNO_R16_RM16: Code = 1172 # type: ignore
+CMOVNO_R16_RM16: int = 1172
 """
 ``CMOVNO r16, r/m16``
 
 ``o16 0F 41 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNO_R32_RM32: Code = 1173 # type: ignore
+CMOVNO_R32_RM32: int = 1173
 """
 ``CMOVNO r32, r/m32``
 
 ``o32 0F 41 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNO_R64_RM64: Code = 1174 # type: ignore
+CMOVNO_R64_RM64: int = 1174
 """
 ``CMOVNO r64, r/m64``
 
 ``o64 0F 41 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVB_R16_RM16: Code = 1175 # type: ignore
+CMOVB_R16_RM16: int = 1175
 """
 ``CMOVB r16, r/m16``
 
 ``o16 0F 42 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVB_R32_RM32: Code = 1176 # type: ignore
+CMOVB_R32_RM32: int = 1176
 """
 ``CMOVB r32, r/m32``
 
 ``o32 0F 42 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVB_R64_RM64: Code = 1177 # type: ignore
+CMOVB_R64_RM64: int = 1177
 """
 ``CMOVB r64, r/m64``
 
 ``o64 0F 42 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVAE_R16_RM16: Code = 1178 # type: ignore
+CMOVAE_R16_RM16: int = 1178
 """
 ``CMOVAE r16, r/m16``
 
 ``o16 0F 43 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVAE_R32_RM32: Code = 1179 # type: ignore
+CMOVAE_R32_RM32: int = 1179
 """
 ``CMOVAE r32, r/m32``
 
 ``o32 0F 43 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVAE_R64_RM64: Code = 1180 # type: ignore
+CMOVAE_R64_RM64: int = 1180
 """
 ``CMOVAE r64, r/m64``
 
 ``o64 0F 43 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVE_R16_RM16: Code = 1181 # type: ignore
+CMOVE_R16_RM16: int = 1181
 """
 ``CMOVE r16, r/m16``
 
 ``o16 0F 44 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVE_R32_RM32: Code = 1182 # type: ignore
+CMOVE_R32_RM32: int = 1182
 """
 ``CMOVE r32, r/m32``
 
 ``o32 0F 44 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVE_R64_RM64: Code = 1183 # type: ignore
+CMOVE_R64_RM64: int = 1183
 """
 ``CMOVE r64, r/m64``
 
 ``o64 0F 44 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVNE_R16_RM16: Code = 1184 # type: ignore
+CMOVNE_R16_RM16: int = 1184
 """
 ``CMOVNE r16, r/m16``
 
 ``o16 0F 45 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNE_R32_RM32: Code = 1185 # type: ignore
+CMOVNE_R32_RM32: int = 1185
 """
 ``CMOVNE r32, r/m32``
 
 ``o32 0F 45 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNE_R64_RM64: Code = 1186 # type: ignore
+CMOVNE_R64_RM64: int = 1186
 """
 ``CMOVNE r64, r/m64``
 
 ``o64 0F 45 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVBE_R16_RM16: Code = 1187 # type: ignore
+CMOVBE_R16_RM16: int = 1187
 """
 ``CMOVBE r16, r/m16``
 
 ``o16 0F 46 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVBE_R32_RM32: Code = 1188 # type: ignore
+CMOVBE_R32_RM32: int = 1188
 """
 ``CMOVBE r32, r/m32``
 
 ``o32 0F 46 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVBE_R64_RM64: Code = 1189 # type: ignore
+CMOVBE_R64_RM64: int = 1189
 """
 ``CMOVBE r64, r/m64``
 
 ``o64 0F 46 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVA_R16_RM16: Code = 1190 # type: ignore
+CMOVA_R16_RM16: int = 1190
 """
 ``CMOVA r16, r/m16``
 
 ``o16 0F 47 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVA_R32_RM32: Code = 1191 # type: ignore
+CMOVA_R32_RM32: int = 1191
 """
 ``CMOVA r32, r/m32``
 
 ``o32 0F 47 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVA_R64_RM64: Code = 1192 # type: ignore
+CMOVA_R64_RM64: int = 1192
 """
 ``CMOVA r64, r/m64``
 
 ``o64 0F 47 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVS_R16_RM16: Code = 1193 # type: ignore
+CMOVS_R16_RM16: int = 1193
 """
 ``CMOVS r16, r/m16``
 
 ``o16 0F 48 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVS_R32_RM32: Code = 1194 # type: ignore
+CMOVS_R32_RM32: int = 1194
 """
 ``CMOVS r32, r/m32``
 
 ``o32 0F 48 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVS_R64_RM64: Code = 1195 # type: ignore
+CMOVS_R64_RM64: int = 1195
 """
 ``CMOVS r64, r/m64``
 
 ``o64 0F 48 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVNS_R16_RM16: Code = 1196 # type: ignore
+CMOVNS_R16_RM16: int = 1196
 """
 ``CMOVNS r16, r/m16``
 
 ``o16 0F 49 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNS_R32_RM32: Code = 1197 # type: ignore
+CMOVNS_R32_RM32: int = 1197
 """
 ``CMOVNS r32, r/m32``
 
 ``o32 0F 49 /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNS_R64_RM64: Code = 1198 # type: ignore
+CMOVNS_R64_RM64: int = 1198
 """
 ``CMOVNS r64, r/m64``
 
 ``o64 0F 49 /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVP_R16_RM16: Code = 1199 # type: ignore
+CMOVP_R16_RM16: int = 1199
 """
 ``CMOVP r16, r/m16``
 
 ``o16 0F 4A /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVP_R32_RM32: Code = 1200 # type: ignore
+CMOVP_R32_RM32: int = 1200
 """
 ``CMOVP r32, r/m32``
 
 ``o32 0F 4A /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVP_R64_RM64: Code = 1201 # type: ignore
+CMOVP_R64_RM64: int = 1201
 """
 ``CMOVP r64, r/m64``
 
 ``o64 0F 4A /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVNP_R16_RM16: Code = 1202 # type: ignore
+CMOVNP_R16_RM16: int = 1202
 """
 ``CMOVNP r16, r/m16``
 
 ``o16 0F 4B /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNP_R32_RM32: Code = 1203 # type: ignore
+CMOVNP_R32_RM32: int = 1203
 """
 ``CMOVNP r32, r/m32``
 
 ``o32 0F 4B /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVNP_R64_RM64: Code = 1204 # type: ignore
+CMOVNP_R64_RM64: int = 1204
 """
 ``CMOVNP r64, r/m64``
 
 ``o64 0F 4B /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVL_R16_RM16: Code = 1205 # type: ignore
+CMOVL_R16_RM16: int = 1205
 """
 ``CMOVL r16, r/m16``
 
 ``o16 0F 4C /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVL_R32_RM32: Code = 1206 # type: ignore
+CMOVL_R32_RM32: int = 1206
 """
 ``CMOVL r32, r/m32``
 
 ``o32 0F 4C /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVL_R64_RM64: Code = 1207 # type: ignore
+CMOVL_R64_RM64: int = 1207
 """
 ``CMOVL r64, r/m64``
 
 ``o64 0F 4C /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVGE_R16_RM16: Code = 1208 # type: ignore
+CMOVGE_R16_RM16: int = 1208
 """
 ``CMOVGE r16, r/m16``
 
 ``o16 0F 4D /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVGE_R32_RM32: Code = 1209 # type: ignore
+CMOVGE_R32_RM32: int = 1209
 """
 ``CMOVGE r32, r/m32``
 
 ``o32 0F 4D /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVGE_R64_RM64: Code = 1210 # type: ignore
+CMOVGE_R64_RM64: int = 1210
 """
 ``CMOVGE r64, r/m64``
 
 ``o64 0F 4D /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVLE_R16_RM16: Code = 1211 # type: ignore
+CMOVLE_R16_RM16: int = 1211
 """
 ``CMOVLE r16, r/m16``
 
 ``o16 0F 4E /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVLE_R32_RM32: Code = 1212 # type: ignore
+CMOVLE_R32_RM32: int = 1212
 """
 ``CMOVLE r32, r/m32``
 
 ``o32 0F 4E /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVLE_R64_RM64: Code = 1213 # type: ignore
+CMOVLE_R64_RM64: int = 1213
 """
 ``CMOVLE r64, r/m64``
 
 ``o64 0F 4E /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-CMOVG_R16_RM16: Code = 1214 # type: ignore
+CMOVG_R16_RM16: int = 1214
 """
 ``CMOVG r16, r/m16``
 
 ``o16 0F 4F /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVG_R32_RM32: Code = 1215 # type: ignore
+CMOVG_R32_RM32: int = 1215
 """
 ``CMOVG r32, r/m32``
 
 ``o32 0F 4F /r``
 
 ``CMOV``
 
 ``16/32/64-bit``
 """
-CMOVG_R64_RM64: Code = 1216 # type: ignore
+CMOVG_R64_RM64: int = 1216
 """
 ``CMOVG r64, r/m64``
 
 ``o64 0F 4F /r``
 
 ``CMOV``
 
 ``64-bit``
 """
-VEX_KANDW_KR_KR_KR: Code = 1217 # type: ignore
+VEX_KANDW_KR_KR_KR: int = 1217
 """
 ``KANDW k1, k2, k3``
 
 ``VEX.L1.0F.W0 41 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KANDQ_KR_KR_KR: Code = 1218 # type: ignore
+VEX_KANDQ_KR_KR_KR: int = 1218
 """
 ``KANDQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 41 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KANDB_KR_KR_KR: Code = 1219 # type: ignore
+VEX_KANDB_KR_KR_KR: int = 1219
 """
 ``KANDB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 41 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KANDD_KR_KR_KR: Code = 1220 # type: ignore
+VEX_KANDD_KR_KR_KR: int = 1220
 """
 ``KANDD k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 41 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KANDNW_KR_KR_KR: Code = 1221 # type: ignore
+VEX_KANDNW_KR_KR_KR: int = 1221
 """
 ``KANDNW k1, k2, k3``
 
 ``VEX.L1.0F.W0 42 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KANDNQ_KR_KR_KR: Code = 1222 # type: ignore
+VEX_KANDNQ_KR_KR_KR: int = 1222
 """
 ``KANDNQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 42 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KANDNB_KR_KR_KR: Code = 1223 # type: ignore
+VEX_KANDNB_KR_KR_KR: int = 1223
 """
 ``KANDNB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 42 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KANDND_KR_KR_KR: Code = 1224 # type: ignore
+VEX_KANDND_KR_KR_KR: int = 1224
 """
 ``KANDND k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 42 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KNOTW_KR_KR: Code = 1225 # type: ignore
+VEX_KNOTW_KR_KR: int = 1225
 """
 ``KNOTW k1, k2``
 
 ``VEX.L0.0F.W0 44 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KNOTQ_KR_KR: Code = 1226 # type: ignore
+VEX_KNOTQ_KR_KR: int = 1226
 """
 ``KNOTQ k1, k2``
 
 ``VEX.L0.0F.W1 44 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KNOTB_KR_KR: Code = 1227 # type: ignore
+VEX_KNOTB_KR_KR: int = 1227
 """
 ``KNOTB k1, k2``
 
 ``VEX.L0.66.0F.W0 44 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KNOTD_KR_KR: Code = 1228 # type: ignore
+VEX_KNOTD_KR_KR: int = 1228
 """
 ``KNOTD k1, k2``
 
 ``VEX.L0.66.0F.W1 44 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KORW_KR_KR_KR: Code = 1229 # type: ignore
+VEX_KORW_KR_KR_KR: int = 1229
 """
 ``KORW k1, k2, k3``
 
 ``VEX.L1.0F.W0 45 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KORQ_KR_KR_KR: Code = 1230 # type: ignore
+VEX_KORQ_KR_KR_KR: int = 1230
 """
 ``KORQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 45 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KORB_KR_KR_KR: Code = 1231 # type: ignore
+VEX_KORB_KR_KR_KR: int = 1231
 """
 ``KORB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 45 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KORD_KR_KR_KR: Code = 1232 # type: ignore
+VEX_KORD_KR_KR_KR: int = 1232
 """
 ``KORD k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 45 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KXNORW_KR_KR_KR: Code = 1233 # type: ignore
+VEX_KXNORW_KR_KR_KR: int = 1233
 """
 ``KXNORW k1, k2, k3``
 
 ``VEX.L1.0F.W0 46 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KXNORQ_KR_KR_KR: Code = 1234 # type: ignore
+VEX_KXNORQ_KR_KR_KR: int = 1234
 """
 ``KXNORQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 46 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KXNORB_KR_KR_KR: Code = 1235 # type: ignore
+VEX_KXNORB_KR_KR_KR: int = 1235
 """
 ``KXNORB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 46 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KXNORD_KR_KR_KR: Code = 1236 # type: ignore
+VEX_KXNORD_KR_KR_KR: int = 1236
 """
 ``KXNORD k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 46 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KXORW_KR_KR_KR: Code = 1237 # type: ignore
+VEX_KXORW_KR_KR_KR: int = 1237
 """
 ``KXORW k1, k2, k3``
 
 ``VEX.L1.0F.W0 47 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KXORQ_KR_KR_KR: Code = 1238 # type: ignore
+VEX_KXORQ_KR_KR_KR: int = 1238
 """
 ``KXORQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 47 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KXORB_KR_KR_KR: Code = 1239 # type: ignore
+VEX_KXORB_KR_KR_KR: int = 1239
 """
 ``KXORB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 47 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KXORD_KR_KR_KR: Code = 1240 # type: ignore
+VEX_KXORD_KR_KR_KR: int = 1240
 """
 ``KXORD k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 47 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KADDW_KR_KR_KR: Code = 1241 # type: ignore
+VEX_KADDW_KR_KR_KR: int = 1241
 """
 ``KADDW k1, k2, k3``
 
 ``VEX.L1.0F.W0 4A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KADDQ_KR_KR_KR: Code = 1242 # type: ignore
+VEX_KADDQ_KR_KR_KR: int = 1242
 """
 ``KADDQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 4A /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KADDB_KR_KR_KR: Code = 1243 # type: ignore
+VEX_KADDB_KR_KR_KR: int = 1243
 """
 ``KADDB k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 4A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KADDD_KR_KR_KR: Code = 1244 # type: ignore
+VEX_KADDD_KR_KR_KR: int = 1244
 """
 ``KADDD k1, k2, k3``
 
 ``VEX.L1.66.0F.W1 4A /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KUNPCKWD_KR_KR_KR: Code = 1245 # type: ignore
+VEX_KUNPCKWD_KR_KR_KR: int = 1245
 """
 ``KUNPCKWD k1, k2, k3``
 
 ``VEX.L1.0F.W0 4B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KUNPCKDQ_KR_KR_KR: Code = 1246 # type: ignore
+VEX_KUNPCKDQ_KR_KR_KR: int = 1246
 """
 ``KUNPCKDQ k1, k2, k3``
 
 ``VEX.L1.0F.W1 4B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KUNPCKBW_KR_KR_KR: Code = 1247 # type: ignore
+VEX_KUNPCKBW_KR_KR_KR: int = 1247
 """
 ``KUNPCKBW k1, k2, k3``
 
 ``VEX.L1.66.0F.W0 4B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVMSKPS_R32_XMM: Code = 1248 # type: ignore
+MOVMSKPS_R32_XMM: int = 1248
 """
 ``MOVMSKPS r32, xmm``
 
 ``NP 0F 50 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-MOVMSKPS_R64_XMM: Code = 1249 # type: ignore
+MOVMSKPS_R64_XMM: int = 1249
 """
 ``MOVMSKPS r64, xmm``
 
 ``NP o64 0F 50 /r``
 
 ``SSE``
 
 ``64-bit``
 """
-VEX_VMOVMSKPS_R32_XMM: Code = 1250 # type: ignore
+VEX_VMOVMSKPS_R32_XMM: int = 1250
 """
 ``VMOVMSKPS r32, xmm2``
 
 ``VEX.128.0F.W0 50 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVMSKPS_R64_XMM: Code = 1251 # type: ignore
+VEX_VMOVMSKPS_R64_XMM: int = 1251
 """
 ``VMOVMSKPS r64, xmm2``
 
 ``VEX.128.0F.W1 50 /r``
 
 ``AVX``
 
 ``64-bit``
 """
-VEX_VMOVMSKPS_R32_YMM: Code = 1252 # type: ignore
+VEX_VMOVMSKPS_R32_YMM: int = 1252
 """
 ``VMOVMSKPS r32, ymm2``
 
 ``VEX.256.0F.W0 50 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVMSKPS_R64_YMM: Code = 1253 # type: ignore
+VEX_VMOVMSKPS_R64_YMM: int = 1253
 """
 ``VMOVMSKPS r64, ymm2``
 
 ``VEX.256.0F.W1 50 /r``
 
 ``AVX``
 
 ``64-bit``
 """
-MOVMSKPD_R32_XMM: Code = 1254 # type: ignore
+MOVMSKPD_R32_XMM: int = 1254
 """
 ``MOVMSKPD r32, xmm``
 
 ``66 0F 50 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MOVMSKPD_R64_XMM: Code = 1255 # type: ignore
+MOVMSKPD_R64_XMM: int = 1255
 """
 ``MOVMSKPD r64, xmm``
 
 ``66 o64 0F 50 /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VMOVMSKPD_R32_XMM: Code = 1256 # type: ignore
+VEX_VMOVMSKPD_R32_XMM: int = 1256
 """
 ``VMOVMSKPD r32, xmm2``
 
 ``VEX.128.66.0F.W0 50 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVMSKPD_R64_XMM: Code = 1257 # type: ignore
+VEX_VMOVMSKPD_R64_XMM: int = 1257
 """
 ``VMOVMSKPD r64, xmm2``
 
 ``VEX.128.66.0F.W1 50 /r``
 
 ``AVX``
 
 ``64-bit``
 """
-VEX_VMOVMSKPD_R32_YMM: Code = 1258 # type: ignore
+VEX_VMOVMSKPD_R32_YMM: int = 1258
 """
 ``VMOVMSKPD r32, ymm2``
 
 ``VEX.256.66.0F.W0 50 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVMSKPD_R64_YMM: Code = 1259 # type: ignore
+VEX_VMOVMSKPD_R64_YMM: int = 1259
 """
 ``VMOVMSKPD r64, ymm2``
 
 ``VEX.256.66.0F.W1 50 /r``
 
 ``AVX``
 
 ``64-bit``
 """
-SQRTPS_XMM_XMMM128: Code = 1260 # type: ignore
+SQRTPS_XMM_XMMM128: int = 1260
 """
 ``SQRTPS xmm1, xmm2/m128``
 
 ``NP 0F 51 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTPS_XMM_XMMM128: Code = 1261 # type: ignore
+VEX_VSQRTPS_XMM_XMMM128: int = 1261
 """
 ``VSQRTPS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTPS_YMM_YMMM256: Code = 1262 # type: ignore
+VEX_VSQRTPS_YMM_YMMM256: int = 1262
 """
 ``VSQRTPS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPS_XMM_K1Z_XMMM128B32: Code = 1263 # type: ignore
+EVEX_VSQRTPS_XMM_K1Z_XMMM128B32: int = 1263
 """
 ``VSQRTPS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.0F.W0 51 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPS_YMM_K1Z_YMMM256B32: Code = 1264 # type: ignore
+EVEX_VSQRTPS_YMM_K1Z_YMMM256B32: int = 1264
 """
 ``VSQRTPS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.0F.W0 51 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPS_ZMM_K1Z_ZMMM512B32_ER: Code = 1265 # type: ignore
+EVEX_VSQRTPS_ZMM_K1Z_ZMMM512B32_ER: int = 1265
 """
 ``VSQRTPS zmm1 {k1}{z}, zmm2/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 51 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SQRTPD_XMM_XMMM128: Code = 1266 # type: ignore
+SQRTPD_XMM_XMMM128: int = 1266
 """
 ``SQRTPD xmm1, xmm2/m128``
 
 ``66 0F 51 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTPD_XMM_XMMM128: Code = 1267 # type: ignore
+VEX_VSQRTPD_XMM_XMMM128: int = 1267
 """
 ``VSQRTPD xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTPD_YMM_YMMM256: Code = 1268 # type: ignore
+VEX_VSQRTPD_YMM_YMMM256: int = 1268
 """
 ``VSQRTPD ymm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPD_XMM_K1Z_XMMM128B64: Code = 1269 # type: ignore
+EVEX_VSQRTPD_XMM_K1Z_XMMM128B64: int = 1269
 """
 ``VSQRTPD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 51 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPD_YMM_K1Z_YMMM256B64: Code = 1270 # type: ignore
+EVEX_VSQRTPD_YMM_K1Z_YMMM256B64: int = 1270
 """
 ``VSQRTPD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 51 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTPD_ZMM_K1Z_ZMMM512B64_ER: Code = 1271 # type: ignore
+EVEX_VSQRTPD_ZMM_K1Z_ZMMM512B64_ER: int = 1271
 """
 ``VSQRTPD zmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 51 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SQRTSS_XMM_XMMM32: Code = 1272 # type: ignore
+SQRTSS_XMM_XMMM32: int = 1272
 """
 ``SQRTSS xmm1, xmm2/m32``
 
 ``F3 0F 51 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTSS_XMM_XMM_XMMM32: Code = 1273 # type: ignore
+VEX_VSQRTSS_XMM_XMM_XMMM32: int = 1273
 """
 ``VSQRTSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTSS_XMM_K1Z_XMM_XMMM32_ER: Code = 1274 # type: ignore
+EVEX_VSQRTSS_XMM_K1Z_XMM_XMMM32_ER: int = 1274
 """
 ``VSQRTSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 51 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SQRTSD_XMM_XMMM64: Code = 1275 # type: ignore
+SQRTSD_XMM_XMMM64: int = 1275
 """
 ``SQRTSD xmm1, xmm2/m64``
 
 ``F2 0F 51 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VSQRTSD_XMM_XMM_XMMM64: Code = 1276 # type: ignore
+VEX_VSQRTSD_XMM_XMM_XMMM64: int = 1276
 """
 ``VSQRTSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 51 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSQRTSD_XMM_K1Z_XMM_XMMM64_ER: Code = 1277 # type: ignore
+EVEX_VSQRTSD_XMM_K1Z_XMM_XMMM64_ER: int = 1277
 """
 ``VSQRTSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 51 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-RSQRTPS_XMM_XMMM128: Code = 1278 # type: ignore
+RSQRTPS_XMM_XMMM128: int = 1278
 """
 ``RSQRTPS xmm1, xmm2/m128``
 
 ``NP 0F 52 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VRSQRTPS_XMM_XMMM128: Code = 1279 # type: ignore
+VEX_VRSQRTPS_XMM_XMMM128: int = 1279
 """
 ``VRSQRTPS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 52 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VRSQRTPS_YMM_YMMM256: Code = 1280 # type: ignore
+VEX_VRSQRTPS_YMM_YMMM256: int = 1280
 """
 ``VRSQRTPS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 52 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-RSQRTSS_XMM_XMMM32: Code = 1281 # type: ignore
+RSQRTSS_XMM_XMMM32: int = 1281
 """
 ``RSQRTSS xmm1, xmm2/m32``
 
 ``F3 0F 52 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VRSQRTSS_XMM_XMM_XMMM32: Code = 1282 # type: ignore
+VEX_VRSQRTSS_XMM_XMM_XMMM32: int = 1282
 """
 ``VRSQRTSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 52 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-RCPPS_XMM_XMMM128: Code = 1283 # type: ignore
+RCPPS_XMM_XMMM128: int = 1283
 """
 ``RCPPS xmm1, xmm2/m128``
 
 ``NP 0F 53 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VRCPPS_XMM_XMMM128: Code = 1284 # type: ignore
+VEX_VRCPPS_XMM_XMMM128: int = 1284
 """
 ``VRCPPS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 53 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VRCPPS_YMM_YMMM256: Code = 1285 # type: ignore
+VEX_VRCPPS_YMM_YMMM256: int = 1285
 """
 ``VRCPPS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 53 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-RCPSS_XMM_XMMM32: Code = 1286 # type: ignore
+RCPSS_XMM_XMMM32: int = 1286
 """
 ``RCPSS xmm1, xmm2/m32``
 
 ``F3 0F 53 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VRCPSS_XMM_XMM_XMMM32: Code = 1287 # type: ignore
+VEX_VRCPSS_XMM_XMM_XMMM32: int = 1287
 """
 ``VRCPSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 53 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-ANDPS_XMM_XMMM128: Code = 1288 # type: ignore
+ANDPS_XMM_XMMM128: int = 1288
 """
 ``ANDPS xmm1, xmm2/m128``
 
 ``NP 0F 54 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VANDPS_XMM_XMM_XMMM128: Code = 1289 # type: ignore
+VEX_VANDPS_XMM_XMM_XMMM128: int = 1289
 """
 ``VANDPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 54 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VANDPS_YMM_YMM_YMMM256: Code = 1290 # type: ignore
+VEX_VANDPS_YMM_YMM_YMMM256: int = 1290
 """
 ``VANDPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 54 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPS_XMM_K1Z_XMM_XMMM128B32: Code = 1291 # type: ignore
+EVEX_VANDPS_XMM_K1Z_XMM_XMMM128B32: int = 1291
 """
 ``VANDPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 54 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPS_YMM_K1Z_YMM_YMMM256B32: Code = 1292 # type: ignore
+EVEX_VANDPS_YMM_K1Z_YMM_YMMM256B32: int = 1292
 """
 ``VANDPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 54 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1293 # type: ignore
+EVEX_VANDPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 1293
 """
 ``VANDPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 54 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ANDPD_XMM_XMMM128: Code = 1294 # type: ignore
+ANDPD_XMM_XMMM128: int = 1294
 """
 ``ANDPD xmm1, xmm2/m128``
 
 ``66 0F 54 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VANDPD_XMM_XMM_XMMM128: Code = 1295 # type: ignore
+VEX_VANDPD_XMM_XMM_XMMM128: int = 1295
 """
 ``VANDPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 54 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VANDPD_YMM_YMM_YMMM256: Code = 1296 # type: ignore
+VEX_VANDPD_YMM_YMM_YMMM256: int = 1296
 """
 ``VANDPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 54 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPD_XMM_K1Z_XMM_XMMM128B64: Code = 1297 # type: ignore
+EVEX_VANDPD_XMM_K1Z_XMM_XMMM128B64: int = 1297
 """
 ``VANDPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 54 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPD_YMM_K1Z_YMM_YMMM256B64: Code = 1298 # type: ignore
+EVEX_VANDPD_YMM_K1Z_YMM_YMMM256B64: int = 1298
 """
 ``VANDPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 54 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1299 # type: ignore
+EVEX_VANDPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 1299
 """
 ``VANDPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 54 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ANDNPS_XMM_XMMM128: Code = 1300 # type: ignore
+ANDNPS_XMM_XMMM128: int = 1300
 """
 ``ANDNPS xmm1, xmm2/m128``
 
 ``NP 0F 55 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VANDNPS_XMM_XMM_XMMM128: Code = 1301 # type: ignore
+VEX_VANDNPS_XMM_XMM_XMMM128: int = 1301
 """
 ``VANDNPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 55 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VANDNPS_YMM_YMM_YMMM256: Code = 1302 # type: ignore
+VEX_VANDNPS_YMM_YMM_YMMM256: int = 1302
 """
 ``VANDNPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 55 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPS_XMM_K1Z_XMM_XMMM128B32: Code = 1303 # type: ignore
+EVEX_VANDNPS_XMM_K1Z_XMM_XMMM128B32: int = 1303
 """
 ``VANDNPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 55 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPS_YMM_K1Z_YMM_YMMM256B32: Code = 1304 # type: ignore
+EVEX_VANDNPS_YMM_K1Z_YMM_YMMM256B32: int = 1304
 """
 ``VANDNPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 55 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1305 # type: ignore
+EVEX_VANDNPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 1305
 """
 ``VANDNPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 55 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ANDNPD_XMM_XMMM128: Code = 1306 # type: ignore
+ANDNPD_XMM_XMMM128: int = 1306
 """
 ``ANDNPD xmm1, xmm2/m128``
 
 ``66 0F 55 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VANDNPD_XMM_XMM_XMMM128: Code = 1307 # type: ignore
+VEX_VANDNPD_XMM_XMM_XMMM128: int = 1307
 """
 ``VANDNPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 55 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VANDNPD_YMM_YMM_YMMM256: Code = 1308 # type: ignore
+VEX_VANDNPD_YMM_YMM_YMMM256: int = 1308
 """
 ``VANDNPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 55 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPD_XMM_K1Z_XMM_XMMM128B64: Code = 1309 # type: ignore
+EVEX_VANDNPD_XMM_K1Z_XMM_XMMM128B64: int = 1309
 """
 ``VANDNPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 55 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPD_YMM_K1Z_YMM_YMMM256B64: Code = 1310 # type: ignore
+EVEX_VANDNPD_YMM_K1Z_YMM_YMMM256B64: int = 1310
 """
 ``VANDNPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 55 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VANDNPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1311 # type: ignore
+EVEX_VANDNPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 1311
 """
 ``VANDNPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 55 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ORPS_XMM_XMMM128: Code = 1312 # type: ignore
+ORPS_XMM_XMMM128: int = 1312
 """
 ``ORPS xmm1, xmm2/m128``
 
 ``NP 0F 56 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VORPS_XMM_XMM_XMMM128: Code = 1313 # type: ignore
+VEX_VORPS_XMM_XMM_XMMM128: int = 1313
 """
 ``VORPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 56 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VORPS_YMM_YMM_YMMM256: Code = 1314 # type: ignore
+VEX_VORPS_YMM_YMM_YMMM256: int = 1314
 """
 ``VORPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 56 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VORPS_XMM_K1Z_XMM_XMMM128B32: Code = 1315 # type: ignore
+EVEX_VORPS_XMM_K1Z_XMM_XMMM128B32: int = 1315
 """
 ``VORPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 56 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VORPS_YMM_K1Z_YMM_YMMM256B32: Code = 1316 # type: ignore
+EVEX_VORPS_YMM_K1Z_YMM_YMMM256B32: int = 1316
 """
 ``VORPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 56 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VORPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1317 # type: ignore
+EVEX_VORPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 1317
 """
 ``VORPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 56 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ORPD_XMM_XMMM128: Code = 1318 # type: ignore
+ORPD_XMM_XMMM128: int = 1318
 """
 ``ORPD xmm1, xmm2/m128``
 
 ``66 0F 56 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VORPD_XMM_XMM_XMMM128: Code = 1319 # type: ignore
+VEX_VORPD_XMM_XMM_XMMM128: int = 1319
 """
 ``VORPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 56 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VORPD_YMM_YMM_YMMM256: Code = 1320 # type: ignore
+VEX_VORPD_YMM_YMM_YMMM256: int = 1320
 """
 ``VORPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 56 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VORPD_XMM_K1Z_XMM_XMMM128B64: Code = 1321 # type: ignore
+EVEX_VORPD_XMM_K1Z_XMM_XMMM128B64: int = 1321
 """
 ``VORPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 56 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VORPD_YMM_K1Z_YMM_YMMM256B64: Code = 1322 # type: ignore
+EVEX_VORPD_YMM_K1Z_YMM_YMMM256B64: int = 1322
 """
 ``VORPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 56 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VORPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1323 # type: ignore
+EVEX_VORPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 1323
 """
 ``VORPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 56 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-XORPS_XMM_XMMM128: Code = 1324 # type: ignore
+XORPS_XMM_XMMM128: int = 1324
 """
 ``XORPS xmm1, xmm2/m128``
 
 ``NP 0F 57 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VXORPS_XMM_XMM_XMMM128: Code = 1325 # type: ignore
+VEX_VXORPS_XMM_XMM_XMMM128: int = 1325
 """
 ``VXORPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 57 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VXORPS_YMM_YMM_YMMM256: Code = 1326 # type: ignore
+VEX_VXORPS_YMM_YMM_YMMM256: int = 1326
 """
 ``VXORPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 57 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPS_XMM_K1Z_XMM_XMMM128B32: Code = 1327 # type: ignore
+EVEX_VXORPS_XMM_K1Z_XMM_XMMM128B32: int = 1327
 """
 ``VXORPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 57 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPS_YMM_K1Z_YMM_YMMM256B32: Code = 1328 # type: ignore
+EVEX_VXORPS_YMM_K1Z_YMM_YMMM256B32: int = 1328
 """
 ``VXORPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 57 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1329 # type: ignore
+EVEX_VXORPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 1329
 """
 ``VXORPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.0F.W0 57 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-XORPD_XMM_XMMM128: Code = 1330 # type: ignore
+XORPD_XMM_XMMM128: int = 1330
 """
 ``XORPD xmm1, xmm2/m128``
 
 ``66 0F 57 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VXORPD_XMM_XMM_XMMM128: Code = 1331 # type: ignore
+VEX_VXORPD_XMM_XMM_XMMM128: int = 1331
 """
 ``VXORPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 57 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VXORPD_YMM_YMM_YMMM256: Code = 1332 # type: ignore
+VEX_VXORPD_YMM_YMM_YMMM256: int = 1332
 """
 ``VXORPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 57 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPD_XMM_K1Z_XMM_XMMM128B64: Code = 1333 # type: ignore
+EVEX_VXORPD_XMM_K1Z_XMM_XMMM128B64: int = 1333
 """
 ``VXORPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 57 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPD_YMM_K1Z_YMM_YMMM256B64: Code = 1334 # type: ignore
+EVEX_VXORPD_YMM_K1Z_YMM_YMMM256B64: int = 1334
 """
 ``VXORPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 57 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VXORPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1335 # type: ignore
+EVEX_VXORPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 1335
 """
 ``VXORPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 57 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-ADDPS_XMM_XMMM128: Code = 1336 # type: ignore
+ADDPS_XMM_XMMM128: int = 1336
 """
 ``ADDPS xmm1, xmm2/m128``
 
 ``NP 0F 58 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VADDPS_XMM_XMM_XMMM128: Code = 1337 # type: ignore
+VEX_VADDPS_XMM_XMM_XMMM128: int = 1337
 """
 ``VADDPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VADDPS_YMM_YMM_YMMM256: Code = 1338 # type: ignore
+VEX_VADDPS_YMM_YMM_YMMM256: int = 1338
 """
 ``VADDPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPS_XMM_K1Z_XMM_XMMM128B32: Code = 1339 # type: ignore
+EVEX_VADDPS_XMM_K1Z_XMM_XMMM128B32: int = 1339
 """
 ``VADDPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPS_YMM_K1Z_YMM_YMMM256B32: Code = 1340 # type: ignore
+EVEX_VADDPS_YMM_K1Z_YMM_YMMM256B32: int = 1340
 """
 ``VADDPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 1341 # type: ignore
+EVEX_VADDPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 1341
 """
 ``VADDPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 58 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ADDPD_XMM_XMMM128: Code = 1342 # type: ignore
+ADDPD_XMM_XMMM128: int = 1342
 """
 ``ADDPD xmm1, xmm2/m128``
 
 ``66 0F 58 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VADDPD_XMM_XMM_XMMM128: Code = 1343 # type: ignore
+VEX_VADDPD_XMM_XMM_XMMM128: int = 1343
 """
 ``VADDPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VADDPD_YMM_YMM_YMMM256: Code = 1344 # type: ignore
+VEX_VADDPD_YMM_YMM_YMMM256: int = 1344
 """
 ``VADDPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPD_XMM_K1Z_XMM_XMMM128B64: Code = 1345 # type: ignore
+EVEX_VADDPD_XMM_K1Z_XMM_XMMM128B64: int = 1345
 """
 ``VADDPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPD_YMM_K1Z_YMM_YMMM256B64: Code = 1346 # type: ignore
+EVEX_VADDPD_YMM_K1Z_YMM_YMMM256B64: int = 1346
 """
 ``VADDPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VADDPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 1347 # type: ignore
+EVEX_VADDPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 1347
 """
 ``VADDPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 58 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ADDSS_XMM_XMMM32: Code = 1348 # type: ignore
+ADDSS_XMM_XMMM32: int = 1348
 """
 ``ADDSS xmm1, xmm2/m32``
 
 ``F3 0F 58 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VADDSS_XMM_XMM_XMMM32: Code = 1349 # type: ignore
+VEX_VADDSS_XMM_XMM_XMMM32: int = 1349
 """
 ``VADDSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VADDSS_XMM_K1Z_XMM_XMMM32_ER: Code = 1350 # type: ignore
+EVEX_VADDSS_XMM_K1Z_XMM_XMMM32_ER: int = 1350
 """
 ``VADDSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 58 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ADDSD_XMM_XMMM64: Code = 1351 # type: ignore
+ADDSD_XMM_XMMM64: int = 1351
 """
 ``ADDSD xmm1, xmm2/m64``
 
 ``F2 0F 58 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VADDSD_XMM_XMM_XMMM64: Code = 1352 # type: ignore
+VEX_VADDSD_XMM_XMM_XMMM64: int = 1352
 """
 ``VADDSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 58 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VADDSD_XMM_K1Z_XMM_XMMM64_ER: Code = 1353 # type: ignore
+EVEX_VADDSD_XMM_K1Z_XMM_XMMM64_ER: int = 1353
 """
 ``VADDSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 58 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MULPS_XMM_XMMM128: Code = 1354 # type: ignore
+MULPS_XMM_XMMM128: int = 1354
 """
 ``MULPS xmm1, xmm2/m128``
 
 ``NP 0F 59 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMULPS_XMM_XMM_XMMM128: Code = 1355 # type: ignore
+VEX_VMULPS_XMM_XMM_XMMM128: int = 1355
 """
 ``VMULPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMULPS_YMM_YMM_YMMM256: Code = 1356 # type: ignore
+VEX_VMULPS_YMM_YMM_YMMM256: int = 1356
 """
 ``VMULPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPS_XMM_K1Z_XMM_XMMM128B32: Code = 1357 # type: ignore
+EVEX_VMULPS_XMM_K1Z_XMM_XMMM128B32: int = 1357
 """
 ``VMULPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPS_YMM_K1Z_YMM_YMMM256B32: Code = 1358 # type: ignore
+EVEX_VMULPS_YMM_K1Z_YMM_YMMM256B32: int = 1358
 """
 ``VMULPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 1359 # type: ignore
+EVEX_VMULPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 1359
 """
 ``VMULPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 59 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MULPD_XMM_XMMM128: Code = 1360 # type: ignore
+MULPD_XMM_XMMM128: int = 1360
 """
 ``MULPD xmm1, xmm2/m128``
 
 ``66 0F 59 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMULPD_XMM_XMM_XMMM128: Code = 1361 # type: ignore
+VEX_VMULPD_XMM_XMM_XMMM128: int = 1361
 """
 ``VMULPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMULPD_YMM_YMM_YMMM256: Code = 1362 # type: ignore
+VEX_VMULPD_YMM_YMM_YMMM256: int = 1362
 """
 ``VMULPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPD_XMM_K1Z_XMM_XMMM128B64: Code = 1363 # type: ignore
+EVEX_VMULPD_XMM_K1Z_XMM_XMMM128B64: int = 1363
 """
 ``VMULPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPD_YMM_K1Z_YMM_YMMM256B64: Code = 1364 # type: ignore
+EVEX_VMULPD_YMM_K1Z_YMM_YMMM256B64: int = 1364
 """
 ``VMULPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMULPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 1365 # type: ignore
+EVEX_VMULPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 1365
 """
 ``VMULPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 59 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MULSS_XMM_XMMM32: Code = 1366 # type: ignore
+MULSS_XMM_XMMM32: int = 1366
 """
 ``MULSS xmm1, xmm2/m32``
 
 ``F3 0F 59 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMULSS_XMM_XMM_XMMM32: Code = 1367 # type: ignore
+VEX_VMULSS_XMM_XMM_XMMM32: int = 1367
 """
 ``VMULSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMULSS_XMM_K1Z_XMM_XMMM32_ER: Code = 1368 # type: ignore
+EVEX_VMULSS_XMM_K1Z_XMM_XMMM32_ER: int = 1368
 """
 ``VMULSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 59 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MULSD_XMM_XMMM64: Code = 1369 # type: ignore
+MULSD_XMM_XMMM64: int = 1369
 """
 ``MULSD xmm1, xmm2/m64``
 
 ``F2 0F 59 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMULSD_XMM_XMM_XMMM64: Code = 1370 # type: ignore
+VEX_VMULSD_XMM_XMM_XMMM64: int = 1370
 """
 ``VMULSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 59 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMULSD_XMM_K1Z_XMM_XMMM64_ER: Code = 1371 # type: ignore
+EVEX_VMULSD_XMM_K1Z_XMM_XMMM64_ER: int = 1371
 """
 ``VMULSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 59 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTPS2PD_XMM_XMMM64: Code = 1372 # type: ignore
+CVTPS2PD_XMM_XMMM64: int = 1372
 """
 ``CVTPS2PD xmm1, xmm2/m64``
 
 ``NP 0F 5A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2PD_XMM_XMMM64: Code = 1373 # type: ignore
+VEX_VCVTPS2PD_XMM_XMMM64: int = 1373
 """
 ``VCVTPS2PD xmm1, xmm2/m64``
 
 ``VEX.128.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2PD_YMM_XMMM128: Code = 1374 # type: ignore
+VEX_VCVTPS2PD_YMM_XMMM128: int = 1374
 """
 ``VCVTPS2PD ymm1, xmm2/m128``
 
 ``VEX.256.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PD_XMM_K1Z_XMMM64B32: Code = 1375 # type: ignore
+EVEX_VCVTPS2PD_XMM_K1Z_XMMM64B32: int = 1375
 """
 ``VCVTPS2PD xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.0F.W0 5A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PD_YMM_K1Z_XMMM128B32: Code = 1376 # type: ignore
+EVEX_VCVTPS2PD_YMM_K1Z_XMMM128B32: int = 1376
 """
 ``VCVTPS2PD ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.0F.W0 5A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PD_ZMM_K1Z_YMMM256B32_SAE: Code = 1377 # type: ignore
+EVEX_VCVTPS2PD_ZMM_K1Z_YMMM256B32_SAE: int = 1377
 """
 ``VCVTPS2PD zmm1 {k1}{z}, ymm2/m256/m32bcst{sae}``
 
 ``EVEX.512.0F.W0 5A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTPD2PS_XMM_XMMM128: Code = 1378 # type: ignore
+CVTPD2PS_XMM_XMMM128: int = 1378
 """
 ``CVTPD2PS xmm1, xmm2/m128``
 
 ``66 0F 5A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPD2PS_XMM_XMMM128: Code = 1379 # type: ignore
+VEX_VCVTPD2PS_XMM_XMMM128: int = 1379
 """
 ``VCVTPD2PS xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPD2PS_XMM_YMMM256: Code = 1380 # type: ignore
+VEX_VCVTPD2PS_XMM_YMMM256: int = 1380
 """
 ``VCVTPD2PS xmm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2PS_XMM_K1Z_XMMM128B64: Code = 1381 # type: ignore
+EVEX_VCVTPD2PS_XMM_K1Z_XMMM128B64: int = 1381
 """
 ``VCVTPD2PS xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 5A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2PS_XMM_K1Z_YMMM256B64: Code = 1382 # type: ignore
+EVEX_VCVTPD2PS_XMM_K1Z_YMMM256B64: int = 1382
 """
 ``VCVTPD2PS xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 5A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2PS_YMM_K1Z_ZMMM512B64_ER: Code = 1383 # type: ignore
+EVEX_VCVTPD2PS_YMM_K1Z_ZMMM512B64_ER: int = 1383
 """
 ``VCVTPD2PS ymm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 5A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTSS2SD_XMM_XMMM32: Code = 1384 # type: ignore
+CVTSS2SD_XMM_XMMM32: int = 1384
 """
 ``CVTSS2SD xmm1, xmm2/m32``
 
 ``F3 0F 5A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSS2SD_XMM_XMM_XMMM32: Code = 1385 # type: ignore
+VEX_VCVTSS2SD_XMM_XMM_XMMM32: int = 1385
 """
 ``VCVTSS2SD xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSS2SD_XMM_K1Z_XMM_XMMM32_SAE: Code = 1386 # type: ignore
+EVEX_VCVTSS2SD_XMM_K1Z_XMM_XMMM32_SAE: int = 1386
 """
 ``VCVTSS2SD xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W0 5A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTSD2SS_XMM_XMMM64: Code = 1387 # type: ignore
+CVTSD2SS_XMM_XMMM64: int = 1387
 """
 ``CVTSD2SS xmm1, xmm2/m64``
 
 ``F2 0F 5A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTSD2SS_XMM_XMM_XMMM64: Code = 1388 # type: ignore
+VEX_VCVTSD2SS_XMM_XMM_XMMM64: int = 1388
 """
 ``VCVTSD2SS xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 5A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSD2SS_XMM_K1Z_XMM_XMMM64_ER: Code = 1389 # type: ignore
+EVEX_VCVTSD2SS_XMM_K1Z_XMM_XMMM64_ER: int = 1389
 """
 ``VCVTSD2SS xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 5A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTDQ2PS_XMM_XMMM128: Code = 1390 # type: ignore
+CVTDQ2PS_XMM_XMMM128: int = 1390
 """
 ``CVTDQ2PS xmm1, xmm2/m128``
 
 ``NP 0F 5B /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTDQ2PS_XMM_XMMM128: Code = 1391 # type: ignore
+VEX_VCVTDQ2PS_XMM_XMMM128: int = 1391
 """
 ``VCVTDQ2PS xmm1, xmm2/m128``
 
 ``VEX.128.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTDQ2PS_YMM_YMMM256: Code = 1392 # type: ignore
+VEX_VCVTDQ2PS_YMM_YMMM256: int = 1392
 """
 ``VCVTDQ2PS ymm1, ymm2/m256``
 
 ``VEX.256.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PS_XMM_K1Z_XMMM128B32: Code = 1393 # type: ignore
+EVEX_VCVTDQ2PS_XMM_K1Z_XMMM128B32: int = 1393
 """
 ``VCVTDQ2PS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PS_YMM_K1Z_YMMM256B32: Code = 1394 # type: ignore
+EVEX_VCVTDQ2PS_YMM_K1Z_YMMM256B32: int = 1394
 """
 ``VCVTDQ2PS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PS_ZMM_K1Z_ZMMM512B32_ER: Code = 1395 # type: ignore
+EVEX_VCVTDQ2PS_ZMM_K1Z_ZMMM512B32_ER: int = 1395
 """
 ``VCVTDQ2PS zmm1 {k1}{z}, zmm2/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 5B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PS_XMM_K1Z_XMMM128B64: Code = 1396 # type: ignore
+EVEX_VCVTQQ2PS_XMM_K1Z_XMMM128B64: int = 1396
 """
 ``VCVTQQ2PS xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.0F.W1 5B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PS_XMM_K1Z_YMMM256B64: Code = 1397 # type: ignore
+EVEX_VCVTQQ2PS_XMM_K1Z_YMMM256B64: int = 1397
 """
 ``VCVTQQ2PS xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.0F.W1 5B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PS_YMM_K1Z_ZMMM512B64_ER: Code = 1398 # type: ignore
+EVEX_VCVTQQ2PS_YMM_K1Z_ZMMM512B64_ER: int = 1398
 """
 ``VCVTQQ2PS ymm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.0F.W1 5B /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-CVTPS2DQ_XMM_XMMM128: Code = 1399 # type: ignore
+CVTPS2DQ_XMM_XMMM128: int = 1399
 """
 ``CVTPS2DQ xmm1, xmm2/m128``
 
 ``66 0F 5B /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2DQ_XMM_XMMM128: Code = 1400 # type: ignore
+VEX_VCVTPS2DQ_XMM_XMMM128: int = 1400
 """
 ``VCVTPS2DQ xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2DQ_YMM_YMMM256: Code = 1401 # type: ignore
+VEX_VCVTPS2DQ_YMM_YMMM256: int = 1401
 """
 ``VCVTPS2DQ ymm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2DQ_XMM_K1Z_XMMM128B32: Code = 1402 # type: ignore
+EVEX_VCVTPS2DQ_XMM_K1Z_XMMM128B32: int = 1402
 """
 ``VCVTPS2DQ xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2DQ_YMM_K1Z_YMMM256B32: Code = 1403 # type: ignore
+EVEX_VCVTPS2DQ_YMM_K1Z_YMMM256B32: int = 1403
 """
 ``VCVTPS2DQ ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2DQ_ZMM_K1Z_ZMMM512B32_ER: Code = 1404 # type: ignore
+EVEX_VCVTPS2DQ_ZMM_K1Z_ZMMM512B32_ER: int = 1404
 """
 ``VCVTPS2DQ zmm1 {k1}{z}, zmm2/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F.W0 5B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTTPS2DQ_XMM_XMMM128: Code = 1405 # type: ignore
+CVTTPS2DQ_XMM_XMMM128: int = 1405
 """
 ``CVTTPS2DQ xmm1, xmm2/m128``
 
 ``F3 0F 5B /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTPS2DQ_XMM_XMMM128: Code = 1406 # type: ignore
+VEX_VCVTTPS2DQ_XMM_XMMM128: int = 1406
 """
 ``VCVTTPS2DQ xmm1, xmm2/m128``
 
 ``VEX.128.F3.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTPS2DQ_YMM_YMMM256: Code = 1407 # type: ignore
+VEX_VCVTTPS2DQ_YMM_YMMM256: int = 1407
 """
 ``VCVTTPS2DQ ymm1, ymm2/m256``
 
 ``VEX.256.F3.0F.WIG 5B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2DQ_XMM_K1Z_XMMM128B32: Code = 1408 # type: ignore
+EVEX_VCVTTPS2DQ_XMM_K1Z_XMMM128B32: int = 1408
 """
 ``VCVTTPS2DQ xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.F3.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2DQ_YMM_K1Z_YMMM256B32: Code = 1409 # type: ignore
+EVEX_VCVTTPS2DQ_YMM_K1Z_YMMM256B32: int = 1409
 """
 ``VCVTTPS2DQ ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.F3.0F.W0 5B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2DQ_ZMM_K1Z_ZMMM512B32_SAE: Code = 1410 # type: ignore
+EVEX_VCVTTPS2DQ_ZMM_K1Z_ZMMM512B32_SAE: int = 1410
 """
 ``VCVTTPS2DQ zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.F3.0F.W0 5B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SUBPS_XMM_XMMM128: Code = 1411 # type: ignore
+SUBPS_XMM_XMMM128: int = 1411
 """
 ``SUBPS xmm1, xmm2/m128``
 
 ``NP 0F 5C /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VSUBPS_XMM_XMM_XMMM128: Code = 1412 # type: ignore
+VEX_VSUBPS_XMM_XMM_XMMM128: int = 1412
 """
 ``VSUBPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSUBPS_YMM_YMM_YMMM256: Code = 1413 # type: ignore
+VEX_VSUBPS_YMM_YMM_YMMM256: int = 1413
 """
 ``VSUBPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPS_XMM_K1Z_XMM_XMMM128B32: Code = 1414 # type: ignore
+EVEX_VSUBPS_XMM_K1Z_XMM_XMMM128B32: int = 1414
 """
 ``VSUBPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 5C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPS_YMM_K1Z_YMM_YMMM256B32: Code = 1415 # type: ignore
+EVEX_VSUBPS_YMM_K1Z_YMM_YMMM256B32: int = 1415
 """
 ``VSUBPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 5C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 1416 # type: ignore
+EVEX_VSUBPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 1416
 """
 ``VSUBPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 5C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SUBPD_XMM_XMMM128: Code = 1417 # type: ignore
+SUBPD_XMM_XMMM128: int = 1417
 """
 ``SUBPD xmm1, xmm2/m128``
 
 ``66 0F 5C /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VSUBPD_XMM_XMM_XMMM128: Code = 1418 # type: ignore
+VEX_VSUBPD_XMM_XMM_XMMM128: int = 1418
 """
 ``VSUBPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSUBPD_YMM_YMM_YMMM256: Code = 1419 # type: ignore
+VEX_VSUBPD_YMM_YMM_YMMM256: int = 1419
 """
 ``VSUBPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPD_XMM_K1Z_XMM_XMMM128B64: Code = 1420 # type: ignore
+EVEX_VSUBPD_XMM_K1Z_XMM_XMMM128B64: int = 1420
 """
 ``VSUBPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 5C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPD_YMM_K1Z_YMM_YMMM256B64: Code = 1421 # type: ignore
+EVEX_VSUBPD_YMM_K1Z_YMM_YMMM256B64: int = 1421
 """
 ``VSUBPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 5C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 1422 # type: ignore
+EVEX_VSUBPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 1422
 """
 ``VSUBPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 5C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SUBSS_XMM_XMMM32: Code = 1423 # type: ignore
+SUBSS_XMM_XMMM32: int = 1423
 """
 ``SUBSS xmm1, xmm2/m32``
 
 ``F3 0F 5C /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VSUBSS_XMM_XMM_XMMM32: Code = 1424 # type: ignore
+VEX_VSUBSS_XMM_XMM_XMMM32: int = 1424
 """
 ``VSUBSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBSS_XMM_K1Z_XMM_XMMM32_ER: Code = 1425 # type: ignore
+EVEX_VSUBSS_XMM_K1Z_XMM_XMMM32_ER: int = 1425
 """
 ``VSUBSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 5C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SUBSD_XMM_XMMM64: Code = 1426 # type: ignore
+SUBSD_XMM_XMMM64: int = 1426
 """
 ``SUBSD xmm1, xmm2/m64``
 
 ``F2 0F 5C /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VSUBSD_XMM_XMM_XMMM64: Code = 1427 # type: ignore
+VEX_VSUBSD_XMM_XMM_XMMM64: int = 1427
 """
 ``VSUBSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 5C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSUBSD_XMM_K1Z_XMM_XMMM64_ER: Code = 1428 # type: ignore
+EVEX_VSUBSD_XMM_K1Z_XMM_XMMM64_ER: int = 1428
 """
 ``VSUBSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 5C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MINPS_XMM_XMMM128: Code = 1429 # type: ignore
+MINPS_XMM_XMMM128: int = 1429
 """
 ``MINPS xmm1, xmm2/m128``
 
 ``NP 0F 5D /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMINPS_XMM_XMM_XMMM128: Code = 1430 # type: ignore
+VEX_VMINPS_XMM_XMM_XMMM128: int = 1430
 """
 ``VMINPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMINPS_YMM_YMM_YMMM256: Code = 1431 # type: ignore
+VEX_VMINPS_YMM_YMM_YMMM256: int = 1431
 """
 ``VMINPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPS_XMM_K1Z_XMM_XMMM128B32: Code = 1432 # type: ignore
+EVEX_VMINPS_XMM_K1Z_XMM_XMMM128B32: int = 1432
 """
 ``VMINPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 5D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPS_YMM_K1Z_YMM_YMMM256B32: Code = 1433 # type: ignore
+EVEX_VMINPS_YMM_K1Z_YMM_YMMM256B32: int = 1433
 """
 ``VMINPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 5D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPS_ZMM_K1Z_ZMM_ZMMM512B32_SAE: Code = 1434 # type: ignore
+EVEX_VMINPS_ZMM_K1Z_ZMM_ZMMM512B32_SAE: int = 1434
 """
 ``VMINPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{sae}``
 
 ``EVEX.512.0F.W0 5D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MINPD_XMM_XMMM128: Code = 1435 # type: ignore
+MINPD_XMM_XMMM128: int = 1435
 """
 ``MINPD xmm1, xmm2/m128``
 
 ``66 0F 5D /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMINPD_XMM_XMM_XMMM128: Code = 1436 # type: ignore
+VEX_VMINPD_XMM_XMM_XMMM128: int = 1436
 """
 ``VMINPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMINPD_YMM_YMM_YMMM256: Code = 1437 # type: ignore
+VEX_VMINPD_YMM_YMM_YMMM256: int = 1437
 """
 ``VMINPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPD_XMM_K1Z_XMM_XMMM128B64: Code = 1438 # type: ignore
+EVEX_VMINPD_XMM_K1Z_XMM_XMMM128B64: int = 1438
 """
 ``VMINPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 5D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPD_YMM_K1Z_YMM_YMMM256B64: Code = 1439 # type: ignore
+EVEX_VMINPD_YMM_K1Z_YMM_YMMM256B64: int = 1439
 """
 ``VMINPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 5D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMINPD_ZMM_K1Z_ZMM_ZMMM512B64_SAE: Code = 1440 # type: ignore
+EVEX_VMINPD_ZMM_K1Z_ZMM_ZMMM512B64_SAE: int = 1440
 """
 ``VMINPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F.W1 5D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MINSS_XMM_XMMM32: Code = 1441 # type: ignore
+MINSS_XMM_XMMM32: int = 1441
 """
 ``MINSS xmm1, xmm2/m32``
 
 ``F3 0F 5D /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMINSS_XMM_XMM_XMMM32: Code = 1442 # type: ignore
+VEX_VMINSS_XMM_XMM_XMMM32: int = 1442
 """
 ``VMINSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMINSS_XMM_K1Z_XMM_XMMM32_SAE: Code = 1443 # type: ignore
+EVEX_VMINSS_XMM_K1Z_XMM_XMMM32_SAE: int = 1443
 """
 ``VMINSS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W0 5D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MINSD_XMM_XMMM64: Code = 1444 # type: ignore
+MINSD_XMM_XMMM64: int = 1444
 """
 ``MINSD xmm1, xmm2/m64``
 
 ``F2 0F 5D /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMINSD_XMM_XMM_XMMM64: Code = 1445 # type: ignore
+VEX_VMINSD_XMM_XMM_XMMM64: int = 1445
 """
 ``VMINSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 5D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMINSD_XMM_K1Z_XMM_XMMM64_SAE: Code = 1446 # type: ignore
+EVEX_VMINSD_XMM_K1Z_XMM_XMMM64_SAE: int = 1446
 """
 ``VMINSD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W1 5D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-DIVPS_XMM_XMMM128: Code = 1447 # type: ignore
+DIVPS_XMM_XMMM128: int = 1447
 """
 ``DIVPS xmm1, xmm2/m128``
 
 ``NP 0F 5E /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VDIVPS_XMM_XMM_XMMM128: Code = 1448 # type: ignore
+VEX_VDIVPS_XMM_XMM_XMMM128: int = 1448
 """
 ``VDIVPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VDIVPS_YMM_YMM_YMMM256: Code = 1449 # type: ignore
+VEX_VDIVPS_YMM_YMM_YMMM256: int = 1449
 """
 ``VDIVPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPS_XMM_K1Z_XMM_XMMM128B32: Code = 1450 # type: ignore
+EVEX_VDIVPS_XMM_K1Z_XMM_XMMM128B32: int = 1450
 """
 ``VDIVPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 5E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPS_YMM_K1Z_YMM_YMMM256B32: Code = 1451 # type: ignore
+EVEX_VDIVPS_YMM_K1Z_YMM_YMMM256B32: int = 1451
 """
 ``VDIVPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 5E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 1452 # type: ignore
+EVEX_VDIVPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 1452
 """
 ``VDIVPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 5E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-DIVPD_XMM_XMMM128: Code = 1453 # type: ignore
+DIVPD_XMM_XMMM128: int = 1453
 """
 ``DIVPD xmm1, xmm2/m128``
 
 ``66 0F 5E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VDIVPD_XMM_XMM_XMMM128: Code = 1454 # type: ignore
+VEX_VDIVPD_XMM_XMM_XMMM128: int = 1454
 """
 ``VDIVPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VDIVPD_YMM_YMM_YMMM256: Code = 1455 # type: ignore
+VEX_VDIVPD_YMM_YMM_YMMM256: int = 1455
 """
 ``VDIVPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPD_XMM_K1Z_XMM_XMMM128B64: Code = 1456 # type: ignore
+EVEX_VDIVPD_XMM_K1Z_XMM_XMMM128B64: int = 1456
 """
 ``VDIVPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 5E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPD_YMM_K1Z_YMM_YMMM256B64: Code = 1457 # type: ignore
+EVEX_VDIVPD_YMM_K1Z_YMM_YMMM256B64: int = 1457
 """
 ``VDIVPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 5E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 1458 # type: ignore
+EVEX_VDIVPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 1458
 """
 ``VDIVPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 5E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-DIVSS_XMM_XMMM32: Code = 1459 # type: ignore
+DIVSS_XMM_XMMM32: int = 1459
 """
 ``DIVSS xmm1, xmm2/m32``
 
 ``F3 0F 5E /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VDIVSS_XMM_XMM_XMMM32: Code = 1460 # type: ignore
+VEX_VDIVSS_XMM_XMM_XMMM32: int = 1460
 """
 ``VDIVSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVSS_XMM_K1Z_XMM_XMMM32_ER: Code = 1461 # type: ignore
+EVEX_VDIVSS_XMM_K1Z_XMM_XMMM32_ER: int = 1461
 """
 ``VDIVSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 5E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-DIVSD_XMM_XMMM64: Code = 1462 # type: ignore
+DIVSD_XMM_XMMM64: int = 1462
 """
 ``DIVSD xmm1, xmm2/m64``
 
 ``F2 0F 5E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VDIVSD_XMM_XMM_XMMM64: Code = 1463 # type: ignore
+VEX_VDIVSD_XMM_XMM_XMMM64: int = 1463
 """
 ``VDIVSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 5E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VDIVSD_XMM_K1Z_XMM_XMMM64_ER: Code = 1464 # type: ignore
+EVEX_VDIVSD_XMM_K1Z_XMM_XMMM64_ER: int = 1464
 """
 ``VDIVSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 5E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MAXPS_XMM_XMMM128: Code = 1465 # type: ignore
+MAXPS_XMM_XMMM128: int = 1465
 """
 ``MAXPS xmm1, xmm2/m128``
 
 ``NP 0F 5F /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMAXPS_XMM_XMM_XMMM128: Code = 1466 # type: ignore
+VEX_VMAXPS_XMM_XMM_XMMM128: int = 1466
 """
 ``VMAXPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMAXPS_YMM_YMM_YMMM256: Code = 1467 # type: ignore
+VEX_VMAXPS_YMM_YMM_YMMM256: int = 1467
 """
 ``VMAXPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPS_XMM_K1Z_XMM_XMMM128B32: Code = 1468 # type: ignore
+EVEX_VMAXPS_XMM_K1Z_XMM_XMMM128B32: int = 1468
 """
 ``VMAXPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.0F.W0 5F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPS_YMM_K1Z_YMM_YMMM256B32: Code = 1469 # type: ignore
+EVEX_VMAXPS_YMM_K1Z_YMM_YMMM256B32: int = 1469
 """
 ``VMAXPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.0F.W0 5F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPS_ZMM_K1Z_ZMM_ZMMM512B32_SAE: Code = 1470 # type: ignore
+EVEX_VMAXPS_ZMM_K1Z_ZMM_ZMMM512B32_SAE: int = 1470
 """
 ``VMAXPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{sae}``
 
 ``EVEX.512.0F.W0 5F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MAXPD_XMM_XMMM128: Code = 1471 # type: ignore
+MAXPD_XMM_XMMM128: int = 1471
 """
 ``MAXPD xmm1, xmm2/m128``
 
 ``66 0F 5F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMAXPD_XMM_XMM_XMMM128: Code = 1472 # type: ignore
+VEX_VMAXPD_XMM_XMM_XMMM128: int = 1472
 """
 ``VMAXPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMAXPD_YMM_YMM_YMMM256: Code = 1473 # type: ignore
+VEX_VMAXPD_YMM_YMM_YMMM256: int = 1473
 """
 ``VMAXPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPD_XMM_K1Z_XMM_XMMM128B64: Code = 1474 # type: ignore
+EVEX_VMAXPD_XMM_K1Z_XMM_XMMM128B64: int = 1474
 """
 ``VMAXPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 5F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPD_YMM_K1Z_YMM_YMMM256B64: Code = 1475 # type: ignore
+EVEX_VMAXPD_YMM_K1Z_YMM_YMMM256B64: int = 1475
 """
 ``VMAXPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 5F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXPD_ZMM_K1Z_ZMM_ZMMM512B64_SAE: Code = 1476 # type: ignore
+EVEX_VMAXPD_ZMM_K1Z_ZMM_ZMMM512B64_SAE: int = 1476
 """
 ``VMAXPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F.W1 5F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MAXSS_XMM_XMMM32: Code = 1477 # type: ignore
+MAXSS_XMM_XMMM32: int = 1477
 """
 ``MAXSS xmm1, xmm2/m32``
 
 ``F3 0F 5F /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VMAXSS_XMM_XMM_XMMM32: Code = 1478 # type: ignore
+VEX_VMAXSS_XMM_XMM_XMMM32: int = 1478
 """
 ``VMAXSS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.F3.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXSS_XMM_K1Z_XMM_XMMM32_SAE: Code = 1479 # type: ignore
+EVEX_VMAXSS_XMM_K1Z_XMM_XMMM32_SAE: int = 1479
 """
 ``VMAXSS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W0 5F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MAXSD_XMM_XMMM64: Code = 1480 # type: ignore
+MAXSD_XMM_XMMM64: int = 1480
 """
 ``MAXSD xmm1, xmm2/m64``
 
 ``F2 0F 5F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMAXSD_XMM_XMM_XMMM64: Code = 1481 # type: ignore
+VEX_VMAXSD_XMM_XMM_XMMM64: int = 1481
 """
 ``VMAXSD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.F2.0F.WIG 5F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMAXSD_XMM_K1Z_XMM_XMMM64_SAE: Code = 1482 # type: ignore
+EVEX_VMAXSD_XMM_K1Z_XMM_XMMM64_SAE: int = 1482
 """
 ``VMAXSD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W1 5F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PUNPCKLBW_MM_MMM32: Code = 1483 # type: ignore
+PUNPCKLBW_MM_MMM32: int = 1483
 """
 ``PUNPCKLBW mm, mm/m32``
 
 ``NP 0F 60 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKLBW_XMM_XMMM128: Code = 1484 # type: ignore
+PUNPCKLBW_XMM_XMMM128: int = 1484
 """
 ``PUNPCKLBW xmm1, xmm2/m128``
 
 ``66 0F 60 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLBW_XMM_XMM_XMMM128: Code = 1485 # type: ignore
+VEX_VPUNPCKLBW_XMM_XMM_XMMM128: int = 1485
 """
 ``VPUNPCKLBW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 60 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLBW_YMM_YMM_YMMM256: Code = 1486 # type: ignore
+VEX_VPUNPCKLBW_YMM_YMM_YMMM256: int = 1486
 """
 ``VPUNPCKLBW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 60 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLBW_XMM_K1Z_XMM_XMMM128: Code = 1487 # type: ignore
+EVEX_VPUNPCKLBW_XMM_K1Z_XMM_XMMM128: int = 1487
 """
 ``VPUNPCKLBW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 60 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLBW_YMM_K1Z_YMM_YMMM256: Code = 1488 # type: ignore
+EVEX_VPUNPCKLBW_YMM_K1Z_YMM_YMMM256: int = 1488
 """
 ``VPUNPCKLBW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 60 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLBW_ZMM_K1Z_ZMM_ZMMM512: Code = 1489 # type: ignore
+EVEX_VPUNPCKLBW_ZMM_K1Z_ZMM_ZMMM512: int = 1489
 """
 ``VPUNPCKLBW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 60 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKLWD_MM_MMM32: Code = 1490 # type: ignore
+PUNPCKLWD_MM_MMM32: int = 1490
 """
 ``PUNPCKLWD mm, mm/m32``
 
 ``NP 0F 61 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKLWD_XMM_XMMM128: Code = 1491 # type: ignore
+PUNPCKLWD_XMM_XMMM128: int = 1491
 """
 ``PUNPCKLWD xmm1, xmm2/m128``
 
 ``66 0F 61 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLWD_XMM_XMM_XMMM128: Code = 1492 # type: ignore
+VEX_VPUNPCKLWD_XMM_XMM_XMMM128: int = 1492
 """
 ``VPUNPCKLWD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 61 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLWD_YMM_YMM_YMMM256: Code = 1493 # type: ignore
+VEX_VPUNPCKLWD_YMM_YMM_YMMM256: int = 1493
 """
 ``VPUNPCKLWD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 61 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLWD_XMM_K1Z_XMM_XMMM128: Code = 1494 # type: ignore
+EVEX_VPUNPCKLWD_XMM_K1Z_XMM_XMMM128: int = 1494
 """
 ``VPUNPCKLWD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 61 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLWD_YMM_K1Z_YMM_YMMM256: Code = 1495 # type: ignore
+EVEX_VPUNPCKLWD_YMM_K1Z_YMM_YMMM256: int = 1495
 """
 ``VPUNPCKLWD ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 61 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLWD_ZMM_K1Z_ZMM_ZMMM512: Code = 1496 # type: ignore
+EVEX_VPUNPCKLWD_ZMM_K1Z_ZMM_ZMMM512: int = 1496
 """
 ``VPUNPCKLWD zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 61 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKLDQ_MM_MMM32: Code = 1497 # type: ignore
+PUNPCKLDQ_MM_MMM32: int = 1497
 """
 ``PUNPCKLDQ mm, mm/m32``
 
 ``NP 0F 62 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKLDQ_XMM_XMMM128: Code = 1498 # type: ignore
+PUNPCKLDQ_XMM_XMMM128: int = 1498
 """
 ``PUNPCKLDQ xmm1, xmm2/m128``
 
 ``66 0F 62 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLDQ_XMM_XMM_XMMM128: Code = 1499 # type: ignore
+VEX_VPUNPCKLDQ_XMM_XMM_XMMM128: int = 1499
 """
 ``VPUNPCKLDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 62 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLDQ_YMM_YMM_YMMM256: Code = 1500 # type: ignore
+VEX_VPUNPCKLDQ_YMM_YMM_YMMM256: int = 1500
 """
 ``VPUNPCKLDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 62 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLDQ_XMM_K1Z_XMM_XMMM128B32: Code = 1501 # type: ignore
+EVEX_VPUNPCKLDQ_XMM_K1Z_XMM_XMMM128B32: int = 1501
 """
 ``VPUNPCKLDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 62 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLDQ_YMM_K1Z_YMM_YMMM256B32: Code = 1502 # type: ignore
+EVEX_VPUNPCKLDQ_YMM_K1Z_YMM_YMMM256B32: int = 1502
 """
 ``VPUNPCKLDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 62 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLDQ_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1503 # type: ignore
+EVEX_VPUNPCKLDQ_ZMM_K1Z_ZMM_ZMMM512B32: int = 1503
 """
 ``VPUNPCKLDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 62 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PACKSSWB_MM_MMM64: Code = 1504 # type: ignore
+PACKSSWB_MM_MMM64: int = 1504
 """
 ``PACKSSWB mm1, mm2/m64``
 
 ``NP 0F 63 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PACKSSWB_XMM_XMMM128: Code = 1505 # type: ignore
+PACKSSWB_XMM_XMMM128: int = 1505
 """
 ``PACKSSWB xmm1, xmm2/m128``
 
 ``66 0F 63 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPACKSSWB_XMM_XMM_XMMM128: Code = 1506 # type: ignore
+VEX_VPACKSSWB_XMM_XMM_XMMM128: int = 1506
 """
 ``VPACKSSWB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 63 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPACKSSWB_YMM_YMM_YMMM256: Code = 1507 # type: ignore
+VEX_VPACKSSWB_YMM_YMM_YMMM256: int = 1507
 """
 ``VPACKSSWB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 63 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSWB_XMM_K1Z_XMM_XMMM128: Code = 1508 # type: ignore
+EVEX_VPACKSSWB_XMM_K1Z_XMM_XMMM128: int = 1508
 """
 ``VPACKSSWB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 63 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSWB_YMM_K1Z_YMM_YMMM256: Code = 1509 # type: ignore
+EVEX_VPACKSSWB_YMM_K1Z_YMM_YMMM256: int = 1509
 """
 ``VPACKSSWB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 63 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSWB_ZMM_K1Z_ZMM_ZMMM512: Code = 1510 # type: ignore
+EVEX_VPACKSSWB_ZMM_K1Z_ZMM_ZMMM512: int = 1510
 """
 ``VPACKSSWB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 63 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPGTB_MM_MMM64: Code = 1511 # type: ignore
+PCMPGTB_MM_MMM64: int = 1511
 """
 ``PCMPGTB mm, mm/m64``
 
 ``NP 0F 64 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPGTB_XMM_XMMM128: Code = 1512 # type: ignore
+PCMPGTB_XMM_XMMM128: int = 1512
 """
 ``PCMPGTB xmm1, xmm2/m128``
 
 ``66 0F 64 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTB_XMM_XMM_XMMM128: Code = 1513 # type: ignore
+VEX_VPCMPGTB_XMM_XMM_XMMM128: int = 1513
 """
 ``VPCMPGTB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 64 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTB_YMM_YMM_YMMM256: Code = 1514 # type: ignore
+VEX_VPCMPGTB_YMM_YMM_YMMM256: int = 1514
 """
 ``VPCMPGTB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 64 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTB_KR_K1_XMM_XMMM128: Code = 1515 # type: ignore
+EVEX_VPCMPGTB_KR_K1_XMM_XMMM128: int = 1515
 """
 ``VPCMPGTB k1 {k2}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 64 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTB_KR_K1_YMM_YMMM256: Code = 1516 # type: ignore
+EVEX_VPCMPGTB_KR_K1_YMM_YMMM256: int = 1516
 """
 ``VPCMPGTB k1 {k2}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 64 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTB_KR_K1_ZMM_ZMMM512: Code = 1517 # type: ignore
+EVEX_VPCMPGTB_KR_K1_ZMM_ZMMM512: int = 1517
 """
 ``VPCMPGTB k1 {k2}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 64 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPGTW_MM_MMM64: Code = 1518 # type: ignore
+PCMPGTW_MM_MMM64: int = 1518
 """
 ``PCMPGTW mm, mm/m64``
 
 ``NP 0F 65 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPGTW_XMM_XMMM128: Code = 1519 # type: ignore
+PCMPGTW_XMM_XMMM128: int = 1519
 """
 ``PCMPGTW xmm1, xmm2/m128``
 
 ``66 0F 65 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTW_XMM_XMM_XMMM128: Code = 1520 # type: ignore
+VEX_VPCMPGTW_XMM_XMM_XMMM128: int = 1520
 """
 ``VPCMPGTW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 65 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTW_YMM_YMM_YMMM256: Code = 1521 # type: ignore
+VEX_VPCMPGTW_YMM_YMM_YMMM256: int = 1521
 """
 ``VPCMPGTW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 65 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTW_KR_K1_XMM_XMMM128: Code = 1522 # type: ignore
+EVEX_VPCMPGTW_KR_K1_XMM_XMMM128: int = 1522
 """
 ``VPCMPGTW k1 {k2}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 65 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTW_KR_K1_YMM_YMMM256: Code = 1523 # type: ignore
+EVEX_VPCMPGTW_KR_K1_YMM_YMMM256: int = 1523
 """
 ``VPCMPGTW k1 {k2}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 65 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTW_KR_K1_ZMM_ZMMM512: Code = 1524 # type: ignore
+EVEX_VPCMPGTW_KR_K1_ZMM_ZMMM512: int = 1524
 """
 ``VPCMPGTW k1 {k2}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 65 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPGTD_MM_MMM64: Code = 1525 # type: ignore
+PCMPGTD_MM_MMM64: int = 1525
 """
 ``PCMPGTD mm, mm/m64``
 
 ``NP 0F 66 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPGTD_XMM_XMMM128: Code = 1526 # type: ignore
+PCMPGTD_XMM_XMMM128: int = 1526
 """
 ``PCMPGTD xmm1, xmm2/m128``
 
 ``66 0F 66 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTD_XMM_XMM_XMMM128: Code = 1527 # type: ignore
+VEX_VPCMPGTD_XMM_XMM_XMMM128: int = 1527
 """
 ``VPCMPGTD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 66 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTD_YMM_YMM_YMMM256: Code = 1528 # type: ignore
+VEX_VPCMPGTD_YMM_YMM_YMMM256: int = 1528
 """
 ``VPCMPGTD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 66 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTD_KR_K1_XMM_XMMM128B32: Code = 1529 # type: ignore
+EVEX_VPCMPGTD_KR_K1_XMM_XMMM128B32: int = 1529
 """
 ``VPCMPGTD k1 {k2}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 66 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTD_KR_K1_YMM_YMMM256B32: Code = 1530 # type: ignore
+EVEX_VPCMPGTD_KR_K1_YMM_YMMM256B32: int = 1530
 """
 ``VPCMPGTD k1 {k2}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 66 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTD_KR_K1_ZMM_ZMMM512B32: Code = 1531 # type: ignore
+EVEX_VPCMPGTD_KR_K1_ZMM_ZMMM512B32: int = 1531
 """
 ``VPCMPGTD k1 {k2}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 66 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PACKUSWB_MM_MMM64: Code = 1532 # type: ignore
+PACKUSWB_MM_MMM64: int = 1532
 """
 ``PACKUSWB mm, mm/m64``
 
 ``NP 0F 67 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PACKUSWB_XMM_XMMM128: Code = 1533 # type: ignore
+PACKUSWB_XMM_XMMM128: int = 1533
 """
 ``PACKUSWB xmm1, xmm2/m128``
 
 ``66 0F 67 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPACKUSWB_XMM_XMM_XMMM128: Code = 1534 # type: ignore
+VEX_VPACKUSWB_XMM_XMM_XMMM128: int = 1534
 """
 ``VPACKUSWB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 67 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPACKUSWB_YMM_YMM_YMMM256: Code = 1535 # type: ignore
+VEX_VPACKUSWB_YMM_YMM_YMMM256: int = 1535
 """
 ``VPACKUSWB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 67 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSWB_XMM_K1Z_XMM_XMMM128: Code = 1536 # type: ignore
+EVEX_VPACKUSWB_XMM_K1Z_XMM_XMMM128: int = 1536
 """
 ``VPACKUSWB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 67 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSWB_YMM_K1Z_YMM_YMMM256: Code = 1537 # type: ignore
+EVEX_VPACKUSWB_YMM_K1Z_YMM_YMMM256: int = 1537
 """
 ``VPACKUSWB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 67 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSWB_ZMM_K1Z_ZMM_ZMMM512: Code = 1538 # type: ignore
+EVEX_VPACKUSWB_ZMM_K1Z_ZMM_ZMMM512: int = 1538
 """
 ``VPACKUSWB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 67 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKHBW_MM_MMM64: Code = 1539 # type: ignore
+PUNPCKHBW_MM_MMM64: int = 1539
 """
 ``PUNPCKHBW mm, mm/m64``
 
 ``NP 0F 68 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKHBW_XMM_XMMM128: Code = 1540 # type: ignore
+PUNPCKHBW_XMM_XMMM128: int = 1540
 """
 ``PUNPCKHBW xmm1, xmm2/m128``
 
 ``66 0F 68 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHBW_XMM_XMM_XMMM128: Code = 1541 # type: ignore
+VEX_VPUNPCKHBW_XMM_XMM_XMMM128: int = 1541
 """
 ``VPUNPCKHBW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 68 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHBW_YMM_YMM_YMMM256: Code = 1542 # type: ignore
+VEX_VPUNPCKHBW_YMM_YMM_YMMM256: int = 1542
 """
 ``VPUNPCKHBW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 68 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHBW_XMM_K1Z_XMM_XMMM128: Code = 1543 # type: ignore
+EVEX_VPUNPCKHBW_XMM_K1Z_XMM_XMMM128: int = 1543
 """
 ``VPUNPCKHBW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 68 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHBW_YMM_K1Z_YMM_YMMM256: Code = 1544 # type: ignore
+EVEX_VPUNPCKHBW_YMM_K1Z_YMM_YMMM256: int = 1544
 """
 ``VPUNPCKHBW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 68 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHBW_ZMM_K1Z_ZMM_ZMMM512: Code = 1545 # type: ignore
+EVEX_VPUNPCKHBW_ZMM_K1Z_ZMM_ZMMM512: int = 1545
 """
 ``VPUNPCKHBW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 68 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKHWD_MM_MMM64: Code = 1546 # type: ignore
+PUNPCKHWD_MM_MMM64: int = 1546
 """
 ``PUNPCKHWD mm, mm/m64``
 
 ``NP 0F 69 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKHWD_XMM_XMMM128: Code = 1547 # type: ignore
+PUNPCKHWD_XMM_XMMM128: int = 1547
 """
 ``PUNPCKHWD xmm1, xmm2/m128``
 
 ``66 0F 69 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHWD_XMM_XMM_XMMM128: Code = 1548 # type: ignore
+VEX_VPUNPCKHWD_XMM_XMM_XMMM128: int = 1548
 """
 ``VPUNPCKHWD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 69 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHWD_YMM_YMM_YMMM256: Code = 1549 # type: ignore
+VEX_VPUNPCKHWD_YMM_YMM_YMMM256: int = 1549
 """
 ``VPUNPCKHWD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 69 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHWD_XMM_K1Z_XMM_XMMM128: Code = 1550 # type: ignore
+EVEX_VPUNPCKHWD_XMM_K1Z_XMM_XMMM128: int = 1550
 """
 ``VPUNPCKHWD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 69 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHWD_YMM_K1Z_YMM_YMMM256: Code = 1551 # type: ignore
+EVEX_VPUNPCKHWD_YMM_K1Z_YMM_YMMM256: int = 1551
 """
 ``VPUNPCKHWD ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 69 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHWD_ZMM_K1Z_ZMM_ZMMM512: Code = 1552 # type: ignore
+EVEX_VPUNPCKHWD_ZMM_K1Z_ZMM_ZMMM512: int = 1552
 """
 ``VPUNPCKHWD zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 69 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKHDQ_MM_MMM64: Code = 1553 # type: ignore
+PUNPCKHDQ_MM_MMM64: int = 1553
 """
 ``PUNPCKHDQ mm, mm/m64``
 
 ``NP 0F 6A /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PUNPCKHDQ_XMM_XMMM128: Code = 1554 # type: ignore
+PUNPCKHDQ_XMM_XMMM128: int = 1554
 """
 ``PUNPCKHDQ xmm1, xmm2/m128``
 
 ``66 0F 6A /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHDQ_XMM_XMM_XMMM128: Code = 1555 # type: ignore
+VEX_VPUNPCKHDQ_XMM_XMM_XMMM128: int = 1555
 """
 ``VPUNPCKHDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 6A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHDQ_YMM_YMM_YMMM256: Code = 1556 # type: ignore
+VEX_VPUNPCKHDQ_YMM_YMM_YMMM256: int = 1556
 """
 ``VPUNPCKHDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 6A /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHDQ_XMM_K1Z_XMM_XMMM128B32: Code = 1557 # type: ignore
+EVEX_VPUNPCKHDQ_XMM_K1Z_XMM_XMMM128B32: int = 1557
 """
 ``VPUNPCKHDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 6A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHDQ_YMM_K1Z_YMM_YMMM256B32: Code = 1558 # type: ignore
+EVEX_VPUNPCKHDQ_YMM_K1Z_YMM_YMMM256B32: int = 1558
 """
 ``VPUNPCKHDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 6A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHDQ_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1559 # type: ignore
+EVEX_VPUNPCKHDQ_ZMM_K1Z_ZMM_ZMMM512B32: int = 1559
 """
 ``VPUNPCKHDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 6A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PACKSSDW_MM_MMM64: Code = 1560 # type: ignore
+PACKSSDW_MM_MMM64: int = 1560
 """
 ``PACKSSDW mm1, mm2/m64``
 
 ``NP 0F 6B /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PACKSSDW_XMM_XMMM128: Code = 1561 # type: ignore
+PACKSSDW_XMM_XMMM128: int = 1561
 """
 ``PACKSSDW xmm1, xmm2/m128``
 
 ``66 0F 6B /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPACKSSDW_XMM_XMM_XMMM128: Code = 1562 # type: ignore
+VEX_VPACKSSDW_XMM_XMM_XMMM128: int = 1562
 """
 ``VPACKSSDW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 6B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPACKSSDW_YMM_YMM_YMMM256: Code = 1563 # type: ignore
+VEX_VPACKSSDW_YMM_YMM_YMMM256: int = 1563
 """
 ``VPACKSSDW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 6B /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSDW_XMM_K1Z_XMM_XMMM128B32: Code = 1564 # type: ignore
+EVEX_VPACKSSDW_XMM_K1Z_XMM_XMMM128B32: int = 1564
 """
 ``VPACKSSDW xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 6B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSDW_YMM_K1Z_YMM_YMMM256B32: Code = 1565 # type: ignore
+EVEX_VPACKSSDW_YMM_K1Z_YMM_YMMM256B32: int = 1565
 """
 ``VPACKSSDW ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 6B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKSSDW_ZMM_K1Z_ZMM_ZMMM512B32: Code = 1566 # type: ignore
+EVEX_VPACKSSDW_ZMM_K1Z_ZMM_ZMMM512B32: int = 1566
 """
 ``VPACKSSDW zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 6B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUNPCKLQDQ_XMM_XMMM128: Code = 1567 # type: ignore
+PUNPCKLQDQ_XMM_XMMM128: int = 1567
 """
 ``PUNPCKLQDQ xmm1, xmm2/m128``
 
 ``66 0F 6C /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLQDQ_XMM_XMM_XMMM128: Code = 1568 # type: ignore
+VEX_VPUNPCKLQDQ_XMM_XMM_XMMM128: int = 1568
 """
 ``VPUNPCKLQDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 6C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKLQDQ_YMM_YMM_YMMM256: Code = 1569 # type: ignore
+VEX_VPUNPCKLQDQ_YMM_YMM_YMMM256: int = 1569
 """
 ``VPUNPCKLQDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 6C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLQDQ_XMM_K1Z_XMM_XMMM128B64: Code = 1570 # type: ignore
+EVEX_VPUNPCKLQDQ_XMM_K1Z_XMM_XMMM128B64: int = 1570
 """
 ``VPUNPCKLQDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 6C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLQDQ_YMM_K1Z_YMM_YMMM256B64: Code = 1571 # type: ignore
+EVEX_VPUNPCKLQDQ_YMM_K1Z_YMM_YMMM256B64: int = 1571
 """
 ``VPUNPCKLQDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 6C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKLQDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1572 # type: ignore
+EVEX_VPUNPCKLQDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 1572
 """
 ``VPUNPCKLQDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 6C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PUNPCKHQDQ_XMM_XMMM128: Code = 1573 # type: ignore
+PUNPCKHQDQ_XMM_XMMM128: int = 1573
 """
 ``PUNPCKHQDQ xmm1, xmm2/m128``
 
 ``66 0F 6D /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHQDQ_XMM_XMM_XMMM128: Code = 1574 # type: ignore
+VEX_VPUNPCKHQDQ_XMM_XMM_XMMM128: int = 1574
 """
 ``VPUNPCKHQDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 6D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPUNPCKHQDQ_YMM_YMM_YMMM256: Code = 1575 # type: ignore
+VEX_VPUNPCKHQDQ_YMM_YMM_YMMM256: int = 1575
 """
 ``VPUNPCKHQDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 6D /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHQDQ_XMM_K1Z_XMM_XMMM128B64: Code = 1576 # type: ignore
+EVEX_VPUNPCKHQDQ_XMM_K1Z_XMM_XMMM128B64: int = 1576
 """
 ``VPUNPCKHQDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 6D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHQDQ_YMM_K1Z_YMM_YMMM256B64: Code = 1577 # type: ignore
+EVEX_VPUNPCKHQDQ_YMM_K1Z_YMM_YMMM256B64: int = 1577
 """
 ``VPUNPCKHQDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 6D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPUNPCKHQDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 1578 # type: ignore
+EVEX_VPUNPCKHQDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 1578
 """
 ``VPUNPCKHQDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 6D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVD_MM_RM32: Code = 1579 # type: ignore
+MOVD_MM_RM32: int = 1579
 """
 ``MOVD mm, r/m32``
 
 ``NP 0F 6E /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-MOVQ_MM_RM64: Code = 1580 # type: ignore
+MOVQ_MM_RM64: int = 1580
 """
 ``MOVQ mm, r/m64``
 
 ``NP o64 0F 6E /r``
 
 ``MMX``
 
 ``64-bit``
 """
-MOVD_XMM_RM32: Code = 1581 # type: ignore
+MOVD_XMM_RM32: int = 1581
 """
 ``MOVD xmm, r/m32``
 
 ``66 0F 6E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MOVQ_XMM_RM64: Code = 1582 # type: ignore
+MOVQ_XMM_RM64: int = 1582
 """
 ``MOVQ xmm, r/m64``
 
 ``66 o64 0F 6E /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VMOVD_XMM_RM32: Code = 1583 # type: ignore
+VEX_VMOVD_XMM_RM32: int = 1583
 """
 ``VMOVD xmm1, r/m32``
 
 ``VEX.128.66.0F.W0 6E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVQ_XMM_RM64: Code = 1584 # type: ignore
+VEX_VMOVQ_XMM_RM64: int = 1584
 """
 ``VMOVQ xmm1, r/m64``
 
 ``VEX.128.66.0F.W1 6E /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VMOVD_XMM_RM32: Code = 1585 # type: ignore
+EVEX_VMOVD_XMM_RM32: int = 1585
 """
 ``VMOVD xmm1, r/m32``
 
 ``EVEX.128.66.0F.W0 6E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVQ_XMM_RM64: Code = 1586 # type: ignore
+EVEX_VMOVQ_XMM_RM64: int = 1586
 """
 ``VMOVQ xmm1, r/m64``
 
 ``EVEX.128.66.0F.W1 6E /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-MOVQ_MM_MMM64: Code = 1587 # type: ignore
+MOVQ_MM_MMM64: int = 1587
 """
 ``MOVQ mm, mm/m64``
 
 ``NP 0F 6F /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-MOVDQA_XMM_XMMM128: Code = 1588 # type: ignore
+MOVDQA_XMM_XMMM128: int = 1588
 """
 ``MOVDQA xmm1, xmm2/m128``
 
 ``66 0F 6F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQA_XMM_XMMM128: Code = 1589 # type: ignore
+VEX_VMOVDQA_XMM_XMMM128: int = 1589
 """
 ``VMOVDQA xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG 6F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQA_YMM_YMMM256: Code = 1590 # type: ignore
+VEX_VMOVDQA_YMM_YMMM256: int = 1590
 """
 ``VMOVDQA ymm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG 6F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_XMM_K1Z_XMMM128: Code = 1591 # type: ignore
+EVEX_VMOVDQA32_XMM_K1Z_XMMM128: int = 1591
 """
 ``VMOVDQA32 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F.W0 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_YMM_K1Z_YMMM256: Code = 1592 # type: ignore
+EVEX_VMOVDQA32_YMM_K1Z_YMMM256: int = 1592
 """
 ``VMOVDQA32 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F.W0 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_ZMM_K1Z_ZMMM512: Code = 1593 # type: ignore
+EVEX_VMOVDQA32_ZMM_K1Z_ZMMM512: int = 1593
 """
 ``VMOVDQA32 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F.W0 6F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_XMM_K1Z_XMMM128: Code = 1594 # type: ignore
+EVEX_VMOVDQA64_XMM_K1Z_XMMM128: int = 1594
 """
 ``VMOVDQA64 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F.W1 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_YMM_K1Z_YMMM256: Code = 1595 # type: ignore
+EVEX_VMOVDQA64_YMM_K1Z_YMMM256: int = 1595
 """
 ``VMOVDQA64 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F.W1 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_ZMM_K1Z_ZMMM512: Code = 1596 # type: ignore
+EVEX_VMOVDQA64_ZMM_K1Z_ZMMM512: int = 1596
 """
 ``VMOVDQA64 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F.W1 6F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVDQU_XMM_XMMM128: Code = 1597 # type: ignore
+MOVDQU_XMM_XMMM128: int = 1597
 """
 ``MOVDQU xmm1, xmm2/m128``
 
 ``F3 0F 6F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQU_XMM_XMMM128: Code = 1598 # type: ignore
+VEX_VMOVDQU_XMM_XMMM128: int = 1598
 """
 ``VMOVDQU xmm1, xmm2/m128``
 
 ``VEX.128.F3.0F.WIG 6F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQU_YMM_YMMM256: Code = 1599 # type: ignore
+VEX_VMOVDQU_YMM_YMMM256: int = 1599
 """
 ``VMOVDQU ymm1, ymm2/m256``
 
 ``VEX.256.F3.0F.WIG 6F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_XMM_K1Z_XMMM128: Code = 1600 # type: ignore
+EVEX_VMOVDQU32_XMM_K1Z_XMMM128: int = 1600
 """
 ``VMOVDQU32 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F3.0F.W0 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_YMM_K1Z_YMMM256: Code = 1601 # type: ignore
+EVEX_VMOVDQU32_YMM_K1Z_YMMM256: int = 1601
 """
 ``VMOVDQU32 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F3.0F.W0 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_ZMM_K1Z_ZMMM512: Code = 1602 # type: ignore
+EVEX_VMOVDQU32_ZMM_K1Z_ZMMM512: int = 1602
 """
 ``VMOVDQU32 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F3.0F.W0 6F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_XMM_K1Z_XMMM128: Code = 1603 # type: ignore
+EVEX_VMOVDQU64_XMM_K1Z_XMMM128: int = 1603
 """
 ``VMOVDQU64 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F3.0F.W1 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_YMM_K1Z_YMMM256: Code = 1604 # type: ignore
+EVEX_VMOVDQU64_YMM_K1Z_YMMM256: int = 1604
 """
 ``VMOVDQU64 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F3.0F.W1 6F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_ZMM_K1Z_ZMMM512: Code = 1605 # type: ignore
+EVEX_VMOVDQU64_ZMM_K1Z_ZMMM512: int = 1605
 """
 ``VMOVDQU64 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F3.0F.W1 6F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_XMM_K1Z_XMMM128: Code = 1606 # type: ignore
+EVEX_VMOVDQU8_XMM_K1Z_XMMM128: int = 1606
 """
 ``VMOVDQU8 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F2.0F.W0 6F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_YMM_K1Z_YMMM256: Code = 1607 # type: ignore
+EVEX_VMOVDQU8_YMM_K1Z_YMMM256: int = 1607
 """
 ``VMOVDQU8 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F2.0F.W0 6F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_ZMM_K1Z_ZMMM512: Code = 1608 # type: ignore
+EVEX_VMOVDQU8_ZMM_K1Z_ZMMM512: int = 1608
 """
 ``VMOVDQU8 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F2.0F.W0 6F /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_XMM_K1Z_XMMM128: Code = 1609 # type: ignore
+EVEX_VMOVDQU16_XMM_K1Z_XMMM128: int = 1609
 """
 ``VMOVDQU16 xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.F2.0F.W1 6F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_YMM_K1Z_YMMM256: Code = 1610 # type: ignore
+EVEX_VMOVDQU16_YMM_K1Z_YMMM256: int = 1610
 """
 ``VMOVDQU16 ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.F2.0F.W1 6F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_ZMM_K1Z_ZMMM512: Code = 1611 # type: ignore
+EVEX_VMOVDQU16_ZMM_K1Z_ZMMM512: int = 1611
 """
 ``VMOVDQU16 zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.F2.0F.W1 6F /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSHUFW_MM_MMM64_IMM8: Code = 1612 # type: ignore
+PSHUFW_MM_MMM64_IMM8: int = 1612
 """
 ``PSHUFW mm1, mm2/m64, imm8``
 
 ``NP 0F 70 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PSHUFD_XMM_XMMM128_IMM8: Code = 1613 # type: ignore
+PSHUFD_XMM_XMMM128_IMM8: int = 1613
 """
 ``PSHUFD xmm1, xmm2/m128, imm8``
 
 ``66 0F 70 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFD_XMM_XMMM128_IMM8: Code = 1614 # type: ignore
+VEX_VPSHUFD_XMM_XMMM128_IMM8: int = 1614
 """
 ``VPSHUFD xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F.WIG 70 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFD_YMM_YMMM256_IMM8: Code = 1615 # type: ignore
+VEX_VPSHUFD_YMM_YMMM256_IMM8: int = 1615
 """
 ``VPSHUFD ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F.WIG 70 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFD_XMM_K1Z_XMMM128B32_IMM8: Code = 1616 # type: ignore
+EVEX_VPSHUFD_XMM_K1Z_XMMM128B32_IMM8: int = 1616
 """
 ``VPSHUFD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 70 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFD_YMM_K1Z_YMMM256B32_IMM8: Code = 1617 # type: ignore
+EVEX_VPSHUFD_YMM_K1Z_YMMM256B32_IMM8: int = 1617
 """
 ``VPSHUFD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 70 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1618 # type: ignore
+EVEX_VPSHUFD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1618
 """
 ``VPSHUFD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 70 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSHUFHW_XMM_XMMM128_IMM8: Code = 1619 # type: ignore
+PSHUFHW_XMM_XMMM128_IMM8: int = 1619
 """
 ``PSHUFHW xmm1, xmm2/m128, imm8``
 
 ``F3 0F 70 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFHW_XMM_XMMM128_IMM8: Code = 1620 # type: ignore
+VEX_VPSHUFHW_XMM_XMMM128_IMM8: int = 1620
 """
 ``VPSHUFHW xmm1, xmm2/m128, imm8``
 
 ``VEX.128.F3.0F.WIG 70 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFHW_YMM_YMMM256_IMM8: Code = 1621 # type: ignore
+VEX_VPSHUFHW_YMM_YMMM256_IMM8: int = 1621
 """
 ``VPSHUFHW ymm1, ymm2/m256, imm8``
 
 ``VEX.256.F3.0F.WIG 70 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFHW_XMM_K1Z_XMMM128_IMM8: Code = 1622 # type: ignore
+EVEX_VPSHUFHW_XMM_K1Z_XMMM128_IMM8: int = 1622
 """
 ``VPSHUFHW xmm1 {k1}{z}, xmm2/m128, imm8``
 
 ``EVEX.128.F3.0F.WIG 70 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFHW_YMM_K1Z_YMMM256_IMM8: Code = 1623 # type: ignore
+EVEX_VPSHUFHW_YMM_K1Z_YMMM256_IMM8: int = 1623
 """
 ``VPSHUFHW ymm1 {k1}{z}, ymm2/m256, imm8``
 
 ``EVEX.256.F3.0F.WIG 70 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFHW_ZMM_K1Z_ZMMM512_IMM8: Code = 1624 # type: ignore
+EVEX_VPSHUFHW_ZMM_K1Z_ZMMM512_IMM8: int = 1624
 """
 ``VPSHUFHW zmm1 {k1}{z}, zmm2/m512, imm8``
 
 ``EVEX.512.F3.0F.WIG 70 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSHUFLW_XMM_XMMM128_IMM8: Code = 1625 # type: ignore
+PSHUFLW_XMM_XMMM128_IMM8: int = 1625
 """
 ``PSHUFLW xmm1, xmm2/m128, imm8``
 
 ``F2 0F 70 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFLW_XMM_XMMM128_IMM8: Code = 1626 # type: ignore
+VEX_VPSHUFLW_XMM_XMMM128_IMM8: int = 1626
 """
 ``VPSHUFLW xmm1, xmm2/m128, imm8``
 
 ``VEX.128.F2.0F.WIG 70 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFLW_YMM_YMMM256_IMM8: Code = 1627 # type: ignore
+VEX_VPSHUFLW_YMM_YMMM256_IMM8: int = 1627
 """
 ``VPSHUFLW ymm1, ymm2/m256, imm8``
 
 ``VEX.256.F2.0F.WIG 70 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFLW_XMM_K1Z_XMMM128_IMM8: Code = 1628 # type: ignore
+EVEX_VPSHUFLW_XMM_K1Z_XMMM128_IMM8: int = 1628
 """
 ``VPSHUFLW xmm1 {k1}{z}, xmm2/m128, imm8``
 
 ``EVEX.128.F2.0F.WIG 70 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFLW_YMM_K1Z_YMMM256_IMM8: Code = 1629 # type: ignore
+EVEX_VPSHUFLW_YMM_K1Z_YMMM256_IMM8: int = 1629
 """
 ``VPSHUFLW ymm1 {k1}{z}, ymm2/m256, imm8``
 
 ``EVEX.256.F2.0F.WIG 70 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFLW_ZMM_K1Z_ZMMM512_IMM8: Code = 1630 # type: ignore
+EVEX_VPSHUFLW_ZMM_K1Z_ZMMM512_IMM8: int = 1630
 """
 ``VPSHUFLW zmm1 {k1}{z}, zmm2/m512, imm8``
 
 ``EVEX.512.F2.0F.WIG 70 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSRLW_MM_IMM8: Code = 1631 # type: ignore
+PSRLW_MM_IMM8: int = 1631
 """
 ``PSRLW mm, imm8``
 
 ``NP 0F 71 /2 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLW_XMM_IMM8: Code = 1632 # type: ignore
+PSRLW_XMM_IMM8: int = 1632
 """
 ``PSRLW xmm1, imm8``
 
 ``66 0F 71 /2 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLW_XMM_XMM_IMM8: Code = 1633 # type: ignore
+VEX_VPSRLW_XMM_XMM_IMM8: int = 1633
 """
 ``VPSRLW xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 71 /2 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLW_YMM_YMM_IMM8: Code = 1634 # type: ignore
+VEX_VPSRLW_YMM_YMM_IMM8: int = 1634
 """
 ``VPSRLW ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 71 /2 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_XMM_K1Z_XMMM128_IMM8: Code = 1635 # type: ignore
+EVEX_VPSRLW_XMM_K1Z_XMMM128_IMM8: int = 1635
 """
 ``VPSRLW xmm1 {k1}{z}, xmm2/m128, imm8``
 
 ``EVEX.128.66.0F.WIG 71 /2 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_YMM_K1Z_YMMM256_IMM8: Code = 1636 # type: ignore
+EVEX_VPSRLW_YMM_K1Z_YMMM256_IMM8: int = 1636
 """
 ``VPSRLW ymm1 {k1}{z}, ymm2/m256, imm8``
 
 ``EVEX.256.66.0F.WIG 71 /2 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_ZMM_K1Z_ZMMM512_IMM8: Code = 1637 # type: ignore
+EVEX_VPSRLW_ZMM_K1Z_ZMMM512_IMM8: int = 1637
 """
 ``VPSRLW zmm1 {k1}{z}, zmm2/m512, imm8``
 
 ``EVEX.512.66.0F.WIG 71 /2 ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSRAW_MM_IMM8: Code = 1638 # type: ignore
+PSRAW_MM_IMM8: int = 1638
 """
 ``PSRAW mm, imm8``
 
 ``NP 0F 71 /4 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRAW_XMM_IMM8: Code = 1639 # type: ignore
+PSRAW_XMM_IMM8: int = 1639
 """
 ``PSRAW xmm1, imm8``
 
 ``66 0F 71 /4 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAW_XMM_XMM_IMM8: Code = 1640 # type: ignore
+VEX_VPSRAW_XMM_XMM_IMM8: int = 1640
 """
 ``VPSRAW xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 71 /4 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAW_YMM_YMM_IMM8: Code = 1641 # type: ignore
+VEX_VPSRAW_YMM_YMM_IMM8: int = 1641
 """
 ``VPSRAW ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 71 /4 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_XMM_K1Z_XMMM128_IMM8: Code = 1642 # type: ignore
+EVEX_VPSRAW_XMM_K1Z_XMMM128_IMM8: int = 1642
 """
 ``VPSRAW xmm1 {k1}{z}, xmm2/m128, imm8``
 
 ``EVEX.128.66.0F.WIG 71 /4 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_YMM_K1Z_YMMM256_IMM8: Code = 1643 # type: ignore
+EVEX_VPSRAW_YMM_K1Z_YMMM256_IMM8: int = 1643
 """
 ``VPSRAW ymm1 {k1}{z}, ymm2/m256, imm8``
 
 ``EVEX.256.66.0F.WIG 71 /4 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_ZMM_K1Z_ZMMM512_IMM8: Code = 1644 # type: ignore
+EVEX_VPSRAW_ZMM_K1Z_ZMMM512_IMM8: int = 1644
 """
 ``VPSRAW zmm1 {k1}{z}, zmm2/m512, imm8``
 
 ``EVEX.512.66.0F.WIG 71 /4 ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSLLW_MM_IMM8: Code = 1645 # type: ignore
+PSLLW_MM_IMM8: int = 1645
 """
 ``PSLLW mm1, imm8``
 
 ``NP 0F 71 /6 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLW_XMM_IMM8: Code = 1646 # type: ignore
+PSLLW_XMM_IMM8: int = 1646
 """
 ``PSLLW xmm1, imm8``
 
 ``66 0F 71 /6 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLW_XMM_XMM_IMM8: Code = 1647 # type: ignore
+VEX_VPSLLW_XMM_XMM_IMM8: int = 1647
 """
 ``VPSLLW xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 71 /6 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLW_YMM_YMM_IMM8: Code = 1648 # type: ignore
+VEX_VPSLLW_YMM_YMM_IMM8: int = 1648
 """
 ``VPSLLW ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 71 /6 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_XMM_K1Z_XMMM128_IMM8: Code = 1649 # type: ignore
+EVEX_VPSLLW_XMM_K1Z_XMMM128_IMM8: int = 1649
 """
 ``VPSLLW xmm1 {k1}{z}, xmm2/m128, imm8``
 
 ``EVEX.128.66.0F.WIG 71 /6 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_YMM_K1Z_YMMM256_IMM8: Code = 1650 # type: ignore
+EVEX_VPSLLW_YMM_K1Z_YMMM256_IMM8: int = 1650
 """
 ``VPSLLW ymm1 {k1}{z}, ymm2/m256, imm8``
 
 ``EVEX.256.66.0F.WIG 71 /6 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_ZMM_K1Z_ZMMM512_IMM8: Code = 1651 # type: ignore
+EVEX_VPSLLW_ZMM_K1Z_ZMMM512_IMM8: int = 1651
 """
 ``VPSLLW zmm1 {k1}{z}, zmm2/m512, imm8``
 
 ``EVEX.512.66.0F.WIG 71 /6 ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORD_XMM_K1Z_XMMM128B32_IMM8: Code = 1652 # type: ignore
+EVEX_VPRORD_XMM_K1Z_XMMM128B32_IMM8: int = 1652
 """
 ``VPRORD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 72 /0 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORD_YMM_K1Z_YMMM256B32_IMM8: Code = 1653 # type: ignore
+EVEX_VPRORD_YMM_K1Z_YMMM256B32_IMM8: int = 1653
 """
 ``VPRORD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 72 /0 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1654 # type: ignore
+EVEX_VPRORD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1654
 """
 ``VPRORD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 72 /0 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORQ_XMM_K1Z_XMMM128B64_IMM8: Code = 1655 # type: ignore
+EVEX_VPRORQ_XMM_K1Z_XMMM128B64_IMM8: int = 1655
 """
 ``VPRORQ xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 72 /0 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORQ_YMM_K1Z_YMMM256B64_IMM8: Code = 1656 # type: ignore
+EVEX_VPRORQ_YMM_K1Z_YMMM256B64_IMM8: int = 1656
 """
 ``VPRORQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 72 /0 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 1657 # type: ignore
+EVEX_VPRORQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 1657
 """
 ``VPRORQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 72 /0 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLD_XMM_K1Z_XMMM128B32_IMM8: Code = 1658 # type: ignore
+EVEX_VPROLD_XMM_K1Z_XMMM128B32_IMM8: int = 1658
 """
 ``VPROLD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 72 /1 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLD_YMM_K1Z_YMMM256B32_IMM8: Code = 1659 # type: ignore
+EVEX_VPROLD_YMM_K1Z_YMMM256B32_IMM8: int = 1659
 """
 ``VPROLD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 72 /1 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1660 # type: ignore
+EVEX_VPROLD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1660
 """
 ``VPROLD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 72 /1 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLQ_XMM_K1Z_XMMM128B64_IMM8: Code = 1661 # type: ignore
+EVEX_VPROLQ_XMM_K1Z_XMMM128B64_IMM8: int = 1661
 """
 ``VPROLQ xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 72 /1 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLQ_YMM_K1Z_YMMM256B64_IMM8: Code = 1662 # type: ignore
+EVEX_VPROLQ_YMM_K1Z_YMMM256B64_IMM8: int = 1662
 """
 ``VPROLQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 72 /1 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 1663 # type: ignore
+EVEX_VPROLQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 1663
 """
 ``VPROLQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 72 /1 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSRLD_MM_IMM8: Code = 1664 # type: ignore
+PSRLD_MM_IMM8: int = 1664
 """
 ``PSRLD mm, imm8``
 
 ``NP 0F 72 /2 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLD_XMM_IMM8: Code = 1665 # type: ignore
+PSRLD_XMM_IMM8: int = 1665
 """
 ``PSRLD xmm1, imm8``
 
 ``66 0F 72 /2 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLD_XMM_XMM_IMM8: Code = 1666 # type: ignore
+VEX_VPSRLD_XMM_XMM_IMM8: int = 1666
 """
 ``VPSRLD xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 72 /2 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLD_YMM_YMM_IMM8: Code = 1667 # type: ignore
+VEX_VPSRLD_YMM_YMM_IMM8: int = 1667
 """
 ``VPSRLD ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 72 /2 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_XMM_K1Z_XMMM128B32_IMM8: Code = 1668 # type: ignore
+EVEX_VPSRLD_XMM_K1Z_XMMM128B32_IMM8: int = 1668
 """
 ``VPSRLD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 72 /2 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_YMM_K1Z_YMMM256B32_IMM8: Code = 1669 # type: ignore
+EVEX_VPSRLD_YMM_K1Z_YMMM256B32_IMM8: int = 1669
 """
 ``VPSRLD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 72 /2 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1670 # type: ignore
+EVEX_VPSRLD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1670
 """
 ``VPSRLD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 72 /2 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSRAD_MM_IMM8: Code = 1671 # type: ignore
+PSRAD_MM_IMM8: int = 1671
 """
 ``PSRAD mm, imm8``
 
 ``NP 0F 72 /4 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRAD_XMM_IMM8: Code = 1672 # type: ignore
+PSRAD_XMM_IMM8: int = 1672
 """
 ``PSRAD xmm1, imm8``
 
 ``66 0F 72 /4 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAD_XMM_XMM_IMM8: Code = 1673 # type: ignore
+VEX_VPSRAD_XMM_XMM_IMM8: int = 1673
 """
 ``VPSRAD xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 72 /4 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAD_YMM_YMM_IMM8: Code = 1674 # type: ignore
+VEX_VPSRAD_YMM_YMM_IMM8: int = 1674
 """
 ``VPSRAD ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 72 /4 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_XMM_K1Z_XMMM128B32_IMM8: Code = 1675 # type: ignore
+EVEX_VPSRAD_XMM_K1Z_XMMM128B32_IMM8: int = 1675
 """
 ``VPSRAD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 72 /4 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_YMM_K1Z_YMMM256B32_IMM8: Code = 1676 # type: ignore
+EVEX_VPSRAD_YMM_K1Z_YMMM256B32_IMM8: int = 1676
 """
 ``VPSRAD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 72 /4 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1677 # type: ignore
+EVEX_VPSRAD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1677
 """
 ``VPSRAD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 72 /4 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_XMM_K1Z_XMMM128B64_IMM8: Code = 1678 # type: ignore
+EVEX_VPSRAQ_XMM_K1Z_XMMM128B64_IMM8: int = 1678
 """
 ``VPSRAQ xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 72 /4 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_YMM_K1Z_YMMM256B64_IMM8: Code = 1679 # type: ignore
+EVEX_VPSRAQ_YMM_K1Z_YMMM256B64_IMM8: int = 1679
 """
 ``VPSRAQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 72 /4 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 1680 # type: ignore
+EVEX_VPSRAQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 1680
 """
 ``VPSRAQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 72 /4 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSLLD_MM_IMM8: Code = 1681 # type: ignore
+PSLLD_MM_IMM8: int = 1681
 """
 ``PSLLD mm, imm8``
 
 ``NP 0F 72 /6 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLD_XMM_IMM8: Code = 1682 # type: ignore
+PSLLD_XMM_IMM8: int = 1682
 """
 ``PSLLD xmm1, imm8``
 
 ``66 0F 72 /6 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLD_XMM_XMM_IMM8: Code = 1683 # type: ignore
+VEX_VPSLLD_XMM_XMM_IMM8: int = 1683
 """
 ``VPSLLD xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 72 /6 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLD_YMM_YMM_IMM8: Code = 1684 # type: ignore
+VEX_VPSLLD_YMM_YMM_IMM8: int = 1684
 """
 ``VPSLLD ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 72 /6 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_XMM_K1Z_XMMM128B32_IMM8: Code = 1685 # type: ignore
+EVEX_VPSLLD_XMM_K1Z_XMMM128B32_IMM8: int = 1685
 """
 ``VPSLLD xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F.W0 72 /6 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_YMM_K1Z_YMMM256B32_IMM8: Code = 1686 # type: ignore
+EVEX_VPSLLD_YMM_K1Z_YMMM256B32_IMM8: int = 1686
 """
 ``VPSLLD ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F.W0 72 /6 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_ZMM_K1Z_ZMMM512B32_IMM8: Code = 1687 # type: ignore
+EVEX_VPSLLD_ZMM_K1Z_ZMMM512B32_IMM8: int = 1687
 """
 ``VPSLLD zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F.W0 72 /6 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSRLQ_MM_IMM8: Code = 1688 # type: ignore
+PSRLQ_MM_IMM8: int = 1688
 """
 ``PSRLQ mm, imm8``
 
 ``NP 0F 73 /2 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLQ_XMM_IMM8: Code = 1689 # type: ignore
+PSRLQ_XMM_IMM8: int = 1689
 """
 ``PSRLQ xmm1, imm8``
 
 ``66 0F 73 /2 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLQ_XMM_XMM_IMM8: Code = 1690 # type: ignore
+VEX_VPSRLQ_XMM_XMM_IMM8: int = 1690
 """
 ``VPSRLQ xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 73 /2 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLQ_YMM_YMM_IMM8: Code = 1691 # type: ignore
+VEX_VPSRLQ_YMM_YMM_IMM8: int = 1691
 """
 ``VPSRLQ ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 73 /2 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_XMM_K1Z_XMMM128B64_IMM8: Code = 1692 # type: ignore
+EVEX_VPSRLQ_XMM_K1Z_XMMM128B64_IMM8: int = 1692
 """
 ``VPSRLQ xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 73 /2 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_YMM_K1Z_YMMM256B64_IMM8: Code = 1693 # type: ignore
+EVEX_VPSRLQ_YMM_K1Z_YMMM256B64_IMM8: int = 1693
 """
 ``VPSRLQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 73 /2 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 1694 # type: ignore
+EVEX_VPSRLQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 1694
 """
 ``VPSRLQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 73 /2 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSRLDQ_XMM_IMM8: Code = 1695 # type: ignore
+PSRLDQ_XMM_IMM8: int = 1695
 """
 ``PSRLDQ xmm1, imm8``
 
 ``66 0F 73 /3 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLDQ_XMM_XMM_IMM8: Code = 1696 # type: ignore
+VEX_VPSRLDQ_XMM_XMM_IMM8: int = 1696
 """
 ``VPSRLDQ xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 73 /3 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLDQ_YMM_YMM_IMM8: Code = 1697 # type: ignore
+VEX_VPSRLDQ_YMM_YMM_IMM8: int = 1697
 """
 ``VPSRLDQ ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 73 /3 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLDQ_XMM_XMMM128_IMM8: Code = 1698 # type: ignore
+EVEX_VPSRLDQ_XMM_XMMM128_IMM8: int = 1698
 """
 ``VPSRLDQ xmm1, xmm2/m128, imm8``
 
 ``EVEX.128.66.0F.WIG 73 /3 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLDQ_YMM_YMMM256_IMM8: Code = 1699 # type: ignore
+EVEX_VPSRLDQ_YMM_YMMM256_IMM8: int = 1699
 """
 ``VPSRLDQ ymm1, ymm2/m256, imm8``
 
 ``EVEX.256.66.0F.WIG 73 /3 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLDQ_ZMM_ZMMM512_IMM8: Code = 1700 # type: ignore
+EVEX_VPSRLDQ_ZMM_ZMMM512_IMM8: int = 1700
 """
 ``VPSRLDQ zmm1, zmm2/m512, imm8``
 
 ``EVEX.512.66.0F.WIG 73 /3 ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSLLQ_MM_IMM8: Code = 1701 # type: ignore
+PSLLQ_MM_IMM8: int = 1701
 """
 ``PSLLQ mm, imm8``
 
 ``NP 0F 73 /6 ib``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLQ_XMM_IMM8: Code = 1702 # type: ignore
+PSLLQ_XMM_IMM8: int = 1702
 """
 ``PSLLQ xmm1, imm8``
 
 ``66 0F 73 /6 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLQ_XMM_XMM_IMM8: Code = 1703 # type: ignore
+VEX_VPSLLQ_XMM_XMM_IMM8: int = 1703
 """
 ``VPSLLQ xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 73 /6 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLQ_YMM_YMM_IMM8: Code = 1704 # type: ignore
+VEX_VPSLLQ_YMM_YMM_IMM8: int = 1704
 """
 ``VPSLLQ ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 73 /6 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_XMM_K1Z_XMMM128B64_IMM8: Code = 1705 # type: ignore
+EVEX_VPSLLQ_XMM_K1Z_XMMM128B64_IMM8: int = 1705
 """
 ``VPSLLQ xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 73 /6 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_YMM_K1Z_YMMM256B64_IMM8: Code = 1706 # type: ignore
+EVEX_VPSLLQ_YMM_K1Z_YMMM256B64_IMM8: int = 1706
 """
 ``VPSLLQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 73 /6 ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 1707 # type: ignore
+EVEX_VPSLLQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 1707
 """
 ``VPSLLQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 73 /6 ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSLLDQ_XMM_IMM8: Code = 1708 # type: ignore
+PSLLDQ_XMM_IMM8: int = 1708
 """
 ``PSLLDQ xmm1, imm8``
 
 ``66 0F 73 /7 ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLDQ_XMM_XMM_IMM8: Code = 1709 # type: ignore
+VEX_VPSLLDQ_XMM_XMM_IMM8: int = 1709
 """
 ``VPSLLDQ xmm1, xmm2, imm8``
 
 ``VEX.128.66.0F.WIG 73 /7 ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLDQ_YMM_YMM_IMM8: Code = 1710 # type: ignore
+VEX_VPSLLDQ_YMM_YMM_IMM8: int = 1710
 """
 ``VPSLLDQ ymm1, ymm2, imm8``
 
 ``VEX.256.66.0F.WIG 73 /7 ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLDQ_XMM_XMMM128_IMM8: Code = 1711 # type: ignore
+EVEX_VPSLLDQ_XMM_XMMM128_IMM8: int = 1711
 """
 ``VPSLLDQ xmm1, xmm2/m128, imm8``
 
 ``EVEX.128.66.0F.WIG 73 /7 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLDQ_YMM_YMMM256_IMM8: Code = 1712 # type: ignore
+EVEX_VPSLLDQ_YMM_YMMM256_IMM8: int = 1712
 """
 ``VPSLLDQ ymm1, ymm2/m256, imm8``
 
 ``EVEX.256.66.0F.WIG 73 /7 ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLDQ_ZMM_ZMMM512_IMM8: Code = 1713 # type: ignore
+EVEX_VPSLLDQ_ZMM_ZMMM512_IMM8: int = 1713
 """
 ``VPSLLDQ zmm1, zmm2/m512, imm8``
 
 ``EVEX.512.66.0F.WIG 73 /7 ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPEQB_MM_MMM64: Code = 1714 # type: ignore
+PCMPEQB_MM_MMM64: int = 1714
 """
 ``PCMPEQB mm, mm/m64``
 
 ``NP 0F 74 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPEQB_XMM_XMMM128: Code = 1715 # type: ignore
+PCMPEQB_XMM_XMMM128: int = 1715
 """
 ``PCMPEQB xmm1, xmm2/m128``
 
 ``66 0F 74 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQB_XMM_XMM_XMMM128: Code = 1716 # type: ignore
+VEX_VPCMPEQB_XMM_XMM_XMMM128: int = 1716
 """
 ``VPCMPEQB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 74 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQB_YMM_YMM_YMMM256: Code = 1717 # type: ignore
+VEX_VPCMPEQB_YMM_YMM_YMMM256: int = 1717
 """
 ``VPCMPEQB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 74 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQB_KR_K1_XMM_XMMM128: Code = 1718 # type: ignore
+EVEX_VPCMPEQB_KR_K1_XMM_XMMM128: int = 1718
 """
 ``VPCMPEQB k1 {k2}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 74 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQB_KR_K1_YMM_YMMM256: Code = 1719 # type: ignore
+EVEX_VPCMPEQB_KR_K1_YMM_YMMM256: int = 1719
 """
 ``VPCMPEQB k1 {k2}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 74 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQB_KR_K1_ZMM_ZMMM512: Code = 1720 # type: ignore
+EVEX_VPCMPEQB_KR_K1_ZMM_ZMMM512: int = 1720
 """
 ``VPCMPEQB k1 {k2}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 74 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPEQW_MM_MMM64: Code = 1721 # type: ignore
+PCMPEQW_MM_MMM64: int = 1721
 """
 ``PCMPEQW mm, mm/m64``
 
 ``NP 0F 75 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPEQW_XMM_XMMM128: Code = 1722 # type: ignore
+PCMPEQW_XMM_XMMM128: int = 1722
 """
 ``PCMPEQW xmm1, xmm2/m128``
 
 ``66 0F 75 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQW_XMM_XMM_XMMM128: Code = 1723 # type: ignore
+VEX_VPCMPEQW_XMM_XMM_XMMM128: int = 1723
 """
 ``VPCMPEQW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 75 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQW_YMM_YMM_YMMM256: Code = 1724 # type: ignore
+VEX_VPCMPEQW_YMM_YMM_YMMM256: int = 1724
 """
 ``VPCMPEQW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 75 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQW_KR_K1_XMM_XMMM128: Code = 1725 # type: ignore
+EVEX_VPCMPEQW_KR_K1_XMM_XMMM128: int = 1725
 """
 ``VPCMPEQW k1 {k2}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG 75 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQW_KR_K1_YMM_YMMM256: Code = 1726 # type: ignore
+EVEX_VPCMPEQW_KR_K1_YMM_YMMM256: int = 1726
 """
 ``VPCMPEQW k1 {k2}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG 75 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQW_KR_K1_ZMM_ZMMM512: Code = 1727 # type: ignore
+EVEX_VPCMPEQW_KR_K1_ZMM_ZMMM512: int = 1727
 """
 ``VPCMPEQW k1 {k2}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG 75 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPEQD_MM_MMM64: Code = 1728 # type: ignore
+PCMPEQD_MM_MMM64: int = 1728
 """
 ``PCMPEQD mm, mm/m64``
 
 ``NP 0F 76 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PCMPEQD_XMM_XMMM128: Code = 1729 # type: ignore
+PCMPEQD_XMM_XMMM128: int = 1729
 """
 ``PCMPEQD xmm1, xmm2/m128``
 
 ``66 0F 76 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQD_XMM_XMM_XMMM128: Code = 1730 # type: ignore
+VEX_VPCMPEQD_XMM_XMM_XMMM128: int = 1730
 """
 ``VPCMPEQD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 76 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQD_YMM_YMM_YMMM256: Code = 1731 # type: ignore
+VEX_VPCMPEQD_YMM_YMM_YMMM256: int = 1731
 """
 ``VPCMPEQD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 76 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQD_KR_K1_XMM_XMMM128B32: Code = 1732 # type: ignore
+EVEX_VPCMPEQD_KR_K1_XMM_XMMM128B32: int = 1732
 """
 ``VPCMPEQD k1 {k2}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQD_KR_K1_YMM_YMMM256B32: Code = 1733 # type: ignore
+EVEX_VPCMPEQD_KR_K1_YMM_YMMM256B32: int = 1733
 """
 ``VPCMPEQD k1 {k2}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQD_KR_K1_ZMM_ZMMM512B32: Code = 1734 # type: ignore
+EVEX_VPCMPEQD_KR_K1_ZMM_ZMMM512B32: int = 1734
 """
 ``VPCMPEQD k1 {k2}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 76 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EMMS: Code = 1735 # type: ignore
+EMMS: int = 1735
 """
 ``EMMS``
 
 ``NP 0F 77``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-VEX_VZEROUPPER: Code = 1736 # type: ignore
+VEX_VZEROUPPER: int = 1736
 """
 ``VZEROUPPER``
 
 ``VEX.128.0F.WIG 77``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VZEROALL: Code = 1737 # type: ignore
+VEX_VZEROALL: int = 1737
 """
 ``VZEROALL``
 
 ``VEX.256.0F.WIG 77``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VMREAD_RM32_R32: Code = 1738 # type: ignore
+VMREAD_RM32_R32: int = 1738
 """
 ``VMREAD r/m32, r32``
 
 ``NP 0F 78 /r``
 
 ``VMX``
 
 ``16/32-bit``
 """
-VMREAD_RM64_R64: Code = 1739 # type: ignore
+VMREAD_RM64_R64: int = 1739
 """
 ``VMREAD r/m64, r64``
 
 ``NP 0F 78 /r``
 
 ``VMX``
 
 ``64-bit``
 """
-EVEX_VCVTTPS2UDQ_XMM_K1Z_XMMM128B32: Code = 1740 # type: ignore
+EVEX_VCVTTPS2UDQ_XMM_K1Z_XMMM128B32: int = 1740
 """
 ``VCVTTPS2UDQ xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.0F.W0 78 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2UDQ_YMM_K1Z_YMMM256B32: Code = 1741 # type: ignore
+EVEX_VCVTTPS2UDQ_YMM_K1Z_YMMM256B32: int = 1741
 """
 ``VCVTTPS2UDQ ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.0F.W0 78 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2UDQ_ZMM_K1Z_ZMMM512B32_SAE: Code = 1742 # type: ignore
+EVEX_VCVTTPS2UDQ_ZMM_K1Z_ZMMM512B32_SAE: int = 1742
 """
 ``VCVTTPS2UDQ zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.0F.W0 78 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UDQ_XMM_K1Z_XMMM128B64: Code = 1743 # type: ignore
+EVEX_VCVTTPD2UDQ_XMM_K1Z_XMMM128B64: int = 1743
 """
 ``VCVTTPD2UDQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.0F.W1 78 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UDQ_XMM_K1Z_YMMM256B64: Code = 1744 # type: ignore
+EVEX_VCVTTPD2UDQ_XMM_K1Z_YMMM256B64: int = 1744
 """
 ``VCVTTPD2UDQ xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.0F.W1 78 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UDQ_YMM_K1Z_ZMMM512B64_SAE: Code = 1745 # type: ignore
+EVEX_VCVTTPD2UDQ_YMM_K1Z_ZMMM512B64_SAE: int = 1745
 """
 ``VCVTTPD2UDQ ymm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.0F.W1 78 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EXTRQ_XMM_IMM8_IMM8: Code = 1746 # type: ignore
+EXTRQ_XMM_IMM8_IMM8: int = 1746
 """
 ``EXTRQ xmm1, imm8, imm8``
 
 ``66 0F 78 /0 ib ib``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2UQQ_XMM_K1Z_XMMM64B32: Code = 1747 # type: ignore
+EVEX_VCVTTPS2UQQ_XMM_K1Z_XMMM64B32: int = 1747
 """
 ``VCVTTPS2UQQ xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.66.0F.W0 78 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2UQQ_YMM_K1Z_XMMM128B32: Code = 1748 # type: ignore
+EVEX_VCVTTPS2UQQ_YMM_K1Z_XMMM128B32: int = 1748
 """
 ``VCVTTPS2UQQ ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.66.0F.W0 78 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2UQQ_ZMM_K1Z_YMMM256B32_SAE: Code = 1749 # type: ignore
+EVEX_VCVTTPS2UQQ_ZMM_K1Z_YMMM256B32_SAE: int = 1749
 """
 ``VCVTTPS2UQQ zmm1 {k1}{z}, ymm2/m256/m32bcst{sae}``
 
 ``EVEX.512.66.0F.W0 78 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UQQ_XMM_K1Z_XMMM128B64: Code = 1750 # type: ignore
+EVEX_VCVTTPD2UQQ_XMM_K1Z_XMMM128B64: int = 1750
 """
 ``VCVTTPD2UQQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 78 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UQQ_YMM_K1Z_YMMM256B64: Code = 1751 # type: ignore
+EVEX_VCVTTPD2UQQ_YMM_K1Z_YMMM256B64: int = 1751
 """
 ``VCVTTPD2UQQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 78 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2UQQ_ZMM_K1Z_ZMMM512B64_SAE: Code = 1752 # type: ignore
+EVEX_VCVTTPD2UQQ_ZMM_K1Z_ZMMM512B64_SAE: int = 1752
 """
 ``VCVTTPD2UQQ zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F.W1 78 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSS2USI_R32_XMMM32_SAE: Code = 1753 # type: ignore
+EVEX_VCVTTSS2USI_R32_XMMM32_SAE: int = 1753
 """
 ``VCVTTSS2USI r32, xmm1/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W0 78 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSS2USI_R64_XMMM32_SAE: Code = 1754 # type: ignore
+EVEX_VCVTTSS2USI_R64_XMMM32_SAE: int = 1754
 """
 ``VCVTTSS2USI r64, xmm1/m32{sae}``
 
 ``EVEX.LIG.F3.0F.W1 78 /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-INSERTQ_XMM_XMM_IMM8_IMM8: Code = 1755 # type: ignore
+INSERTQ_XMM_XMM_IMM8_IMM8: int = 1755
 """
 ``INSERTQ xmm1, xmm2, imm8, imm8``
 
 ``F2 0F 78 /r ib ib``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSD2USI_R32_XMMM64_SAE: Code = 1756 # type: ignore
+EVEX_VCVTTSD2USI_R32_XMMM64_SAE: int = 1756
 """
 ``VCVTTSD2USI r32, xmm1/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W0 78 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTSD2USI_R64_XMMM64_SAE: Code = 1757 # type: ignore
+EVEX_VCVTTSD2USI_R64_XMMM64_SAE: int = 1757
 """
 ``VCVTTSD2USI r64, xmm1/m64{sae}``
 
 ``EVEX.LIG.F2.0F.W1 78 /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-VMWRITE_R32_RM32: Code = 1758 # type: ignore
+VMWRITE_R32_RM32: int = 1758
 """
 ``VMWRITE r32, r/m32``
 
 ``NP 0F 79 /r``
 
 ``VMX``
 
 ``16/32-bit``
 """
-VMWRITE_R64_RM64: Code = 1759 # type: ignore
+VMWRITE_R64_RM64: int = 1759
 """
 ``VMWRITE r64, r/m64``
 
 ``NP 0F 79 /r``
 
 ``VMX``
 
 ``64-bit``
 """
-EVEX_VCVTPS2UDQ_XMM_K1Z_XMMM128B32: Code = 1760 # type: ignore
+EVEX_VCVTPS2UDQ_XMM_K1Z_XMMM128B32: int = 1760
 """
 ``VCVTPS2UDQ xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.0F.W0 79 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2UDQ_YMM_K1Z_YMMM256B32: Code = 1761 # type: ignore
+EVEX_VCVTPS2UDQ_YMM_K1Z_YMMM256B32: int = 1761
 """
 ``VCVTPS2UDQ ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.0F.W0 79 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2UDQ_ZMM_K1Z_ZMMM512B32_ER: Code = 1762 # type: ignore
+EVEX_VCVTPS2UDQ_ZMM_K1Z_ZMMM512B32_ER: int = 1762
 """
 ``VCVTPS2UDQ zmm1 {k1}{z}, zmm2/m512/m32bcst{er}``
 
 ``EVEX.512.0F.W0 79 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UDQ_XMM_K1Z_XMMM128B64: Code = 1763 # type: ignore
+EVEX_VCVTPD2UDQ_XMM_K1Z_XMMM128B64: int = 1763
 """
 ``VCVTPD2UDQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.0F.W1 79 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UDQ_XMM_K1Z_YMMM256B64: Code = 1764 # type: ignore
+EVEX_VCVTPD2UDQ_XMM_K1Z_YMMM256B64: int = 1764
 """
 ``VCVTPD2UDQ xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.0F.W1 79 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UDQ_YMM_K1Z_ZMMM512B64_ER: Code = 1765 # type: ignore
+EVEX_VCVTPD2UDQ_YMM_K1Z_ZMMM512B64_ER: int = 1765
 """
 ``VCVTPD2UDQ ymm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.0F.W1 79 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EXTRQ_XMM_XMM: Code = 1766 # type: ignore
+EXTRQ_XMM_XMM: int = 1766
 """
 ``EXTRQ xmm1, xmm2``
 
 ``66 0F 79 /r``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2UQQ_XMM_K1Z_XMMM64B32: Code = 1767 # type: ignore
+EVEX_VCVTPS2UQQ_XMM_K1Z_XMMM64B32: int = 1767
 """
 ``VCVTPS2UQQ xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.66.0F.W0 79 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2UQQ_YMM_K1Z_XMMM128B32: Code = 1768 # type: ignore
+EVEX_VCVTPS2UQQ_YMM_K1Z_XMMM128B32: int = 1768
 """
 ``VCVTPS2UQQ ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.66.0F.W0 79 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2UQQ_ZMM_K1Z_YMMM256B32_ER: Code = 1769 # type: ignore
+EVEX_VCVTPS2UQQ_ZMM_K1Z_YMMM256B32_ER: int = 1769
 """
 ``VCVTPS2UQQ zmm1 {k1}{z}, ymm2/m256/m32bcst{er}``
 
 ``EVEX.512.66.0F.W0 79 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UQQ_XMM_K1Z_XMMM128B64: Code = 1770 # type: ignore
+EVEX_VCVTPD2UQQ_XMM_K1Z_XMMM128B64: int = 1770
 """
 ``VCVTPD2UQQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 79 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UQQ_YMM_K1Z_YMMM256B64: Code = 1771 # type: ignore
+EVEX_VCVTPD2UQQ_YMM_K1Z_YMMM256B64: int = 1771
 """
 ``VCVTPD2UQQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 79 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2UQQ_ZMM_K1Z_ZMMM512B64_ER: Code = 1772 # type: ignore
+EVEX_VCVTPD2UQQ_ZMM_K1Z_ZMMM512B64_ER: int = 1772
 """
 ``VCVTPD2UQQ zmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 79 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSS2USI_R32_XMMM32_ER: Code = 1773 # type: ignore
+EVEX_VCVTSS2USI_R32_XMMM32_ER: int = 1773
 """
 ``VCVTSS2USI r32, xmm1/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 79 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSS2USI_R64_XMMM32_ER: Code = 1774 # type: ignore
+EVEX_VCVTSS2USI_R64_XMMM32_ER: int = 1774
 """
 ``VCVTSS2USI r64, xmm1/m32{er}``
 
 ``EVEX.LIG.F3.0F.W1 79 /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-INSERTQ_XMM_XMM: Code = 1775 # type: ignore
+INSERTQ_XMM_XMM: int = 1775
 """
 ``INSERTQ xmm1, xmm2``
 
 ``F2 0F 79 /r``
 
 ``SSE4A``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSD2USI_R32_XMMM64_ER: Code = 1776 # type: ignore
+EVEX_VCVTSD2USI_R32_XMMM64_ER: int = 1776
 """
 ``VCVTSD2USI r32, xmm1/m64{er}``
 
 ``EVEX.LIG.F2.0F.W0 79 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTSD2USI_R64_XMMM64_ER: Code = 1777 # type: ignore
+EVEX_VCVTSD2USI_R64_XMMM64_ER: int = 1777
 """
 ``VCVTSD2USI r64, xmm1/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 79 /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-EVEX_VCVTTPS2QQ_XMM_K1Z_XMMM64B32: Code = 1778 # type: ignore
+EVEX_VCVTTPS2QQ_XMM_K1Z_XMMM64B32: int = 1778
 """
 ``VCVTTPS2QQ xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.66.0F.W0 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2QQ_YMM_K1Z_XMMM128B32: Code = 1779 # type: ignore
+EVEX_VCVTTPS2QQ_YMM_K1Z_XMMM128B32: int = 1779
 """
 ``VCVTTPS2QQ ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.66.0F.W0 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPS2QQ_ZMM_K1Z_YMMM256B32_SAE: Code = 1780 # type: ignore
+EVEX_VCVTTPS2QQ_ZMM_K1Z_YMMM256B32_SAE: int = 1780
 """
 ``VCVTTPS2QQ zmm1 {k1}{z}, ymm2/m256/m32bcst{sae}``
 
 ``EVEX.512.66.0F.W0 7A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2QQ_XMM_K1Z_XMMM128B64: Code = 1781 # type: ignore
+EVEX_VCVTTPD2QQ_XMM_K1Z_XMMM128B64: int = 1781
 """
 ``VCVTTPD2QQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2QQ_YMM_K1Z_YMMM256B64: Code = 1782 # type: ignore
+EVEX_VCVTTPD2QQ_YMM_K1Z_YMMM256B64: int = 1782
 """
 ``VCVTTPD2QQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2QQ_ZMM_K1Z_ZMMM512B64_SAE: Code = 1783 # type: ignore
+EVEX_VCVTTPD2QQ_ZMM_K1Z_ZMMM512B64_SAE: int = 1783
 """
 ``VCVTTPD2QQ zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F.W1 7A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PD_XMM_K1Z_XMMM64B32: Code = 1784 # type: ignore
+EVEX_VCVTUDQ2PD_XMM_K1Z_XMMM64B32: int = 1784
 """
 ``VCVTUDQ2PD xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.F3.0F.W0 7A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PD_YMM_K1Z_XMMM128B32: Code = 1785 # type: ignore
+EVEX_VCVTUDQ2PD_YMM_K1Z_XMMM128B32: int = 1785
 """
 ``VCVTUDQ2PD ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.F3.0F.W0 7A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PD_ZMM_K1Z_YMMM256B32_ER: Code = 1786 # type: ignore
+EVEX_VCVTUDQ2PD_ZMM_K1Z_YMMM256B32_ER: int = 1786
 """
 ``VCVTUDQ2PD zmm1 {k1}{z}, ymm2/m256/m32bcst{er}``
 
 ``EVEX.512.F3.0F.W0 7A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PD_XMM_K1Z_XMMM128B64: Code = 1787 # type: ignore
+EVEX_VCVTUQQ2PD_XMM_K1Z_XMMM128B64: int = 1787
 """
 ``VCVTUQQ2PD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.F3.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PD_YMM_K1Z_YMMM256B64: Code = 1788 # type: ignore
+EVEX_VCVTUQQ2PD_YMM_K1Z_YMMM256B64: int = 1788
 """
 ``VCVTUQQ2PD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.F3.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PD_ZMM_K1Z_ZMMM512B64_ER: Code = 1789 # type: ignore
+EVEX_VCVTUQQ2PD_ZMM_K1Z_ZMMM512B64_ER: int = 1789
 """
 ``VCVTUQQ2PD zmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.F3.0F.W1 7A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PS_XMM_K1Z_XMMM128B32: Code = 1790 # type: ignore
+EVEX_VCVTUDQ2PS_XMM_K1Z_XMMM128B32: int = 1790
 """
 ``VCVTUDQ2PS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.F2.0F.W0 7A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PS_YMM_K1Z_YMMM256B32: Code = 1791 # type: ignore
+EVEX_VCVTUDQ2PS_YMM_K1Z_YMMM256B32: int = 1791
 """
 ``VCVTUDQ2PS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.F2.0F.W0 7A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUDQ2PS_ZMM_K1Z_ZMMM512B32_ER: Code = 1792 # type: ignore
+EVEX_VCVTUDQ2PS_ZMM_K1Z_ZMMM512B32_ER: int = 1792
 """
 ``VCVTUDQ2PS zmm1 {k1}{z}, zmm2/m512/m32bcst{er}``
 
 ``EVEX.512.F2.0F.W0 7A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PS_XMM_K1Z_XMMM128B64: Code = 1793 # type: ignore
+EVEX_VCVTUQQ2PS_XMM_K1Z_XMMM128B64: int = 1793
 """
 ``VCVTUQQ2PS xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.F2.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PS_XMM_K1Z_YMMM256B64: Code = 1794 # type: ignore
+EVEX_VCVTUQQ2PS_XMM_K1Z_YMMM256B64: int = 1794
 """
 ``VCVTUQQ2PS xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.F2.0F.W1 7A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUQQ2PS_YMM_K1Z_ZMMM512B64_ER: Code = 1795 # type: ignore
+EVEX_VCVTUQQ2PS_YMM_K1Z_ZMMM512B64_ER: int = 1795
 """
 ``VCVTUQQ2PS ymm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.F2.0F.W1 7A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2QQ_XMM_K1Z_XMMM64B32: Code = 1796 # type: ignore
+EVEX_VCVTPS2QQ_XMM_K1Z_XMMM64B32: int = 1796
 """
 ``VCVTPS2QQ xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.66.0F.W0 7B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2QQ_YMM_K1Z_XMMM128B32: Code = 1797 # type: ignore
+EVEX_VCVTPS2QQ_YMM_K1Z_XMMM128B32: int = 1797
 """
 ``VCVTPS2QQ ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.66.0F.W0 7B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2QQ_ZMM_K1Z_YMMM256B32_ER: Code = 1798 # type: ignore
+EVEX_VCVTPS2QQ_ZMM_K1Z_YMMM256B32_ER: int = 1798
 """
 ``VCVTPS2QQ zmm1 {k1}{z}, ymm2/m256/m32bcst{er}``
 
 ``EVEX.512.66.0F.W0 7B /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2QQ_XMM_K1Z_XMMM128B64: Code = 1799 # type: ignore
+EVEX_VCVTPD2QQ_XMM_K1Z_XMMM128B64: int = 1799
 """
 ``VCVTPD2QQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 7B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2QQ_YMM_K1Z_YMMM256B64: Code = 1800 # type: ignore
+EVEX_VCVTPD2QQ_YMM_K1Z_YMMM256B64: int = 1800
 """
 ``VCVTPD2QQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 7B /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2QQ_ZMM_K1Z_ZMMM512B64_ER: Code = 1801 # type: ignore
+EVEX_VCVTPD2QQ_ZMM_K1Z_ZMMM512B64_ER: int = 1801
 """
 ``VCVTPD2QQ zmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F.W1 7B /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUSI2SS_XMM_XMM_RM32_ER: Code = 1802 # type: ignore
+EVEX_VCVTUSI2SS_XMM_XMM_RM32_ER: int = 1802
 """
 ``VCVTUSI2SS xmm1, xmm2, r/m32{er}``
 
 ``EVEX.LIG.F3.0F.W0 7B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUSI2SS_XMM_XMM_RM64_ER: Code = 1803 # type: ignore
+EVEX_VCVTUSI2SS_XMM_XMM_RM64_ER: int = 1803
 """
 ``VCVTUSI2SS xmm1, xmm2, r/m64{er}``
 
 ``EVEX.LIG.F3.0F.W1 7B /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-EVEX_VCVTUSI2SD_XMM_XMM_RM32_ER: Code = 1804 # type: ignore
+EVEX_VCVTUSI2SD_XMM_XMM_RM32_ER: int = 1804
 """
 ``VCVTUSI2SD xmm1, xmm2, r/m32{er}``
 
 ``EVEX.LIG.F2.0F.W0 7B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTUSI2SD_XMM_XMM_RM64_ER: Code = 1805 # type: ignore
+EVEX_VCVTUSI2SD_XMM_XMM_RM64_ER: int = 1805
 """
 ``VCVTUSI2SD xmm1, xmm2, r/m64{er}``
 
 ``EVEX.LIG.F2.0F.W1 7B /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-HADDPD_XMM_XMMM128: Code = 1806 # type: ignore
+HADDPD_XMM_XMMM128: int = 1806
 """
 ``HADDPD xmm1, xmm2/m128``
 
 ``66 0F 7C /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VHADDPD_XMM_XMM_XMMM128: Code = 1807 # type: ignore
+VEX_VHADDPD_XMM_XMM_XMMM128: int = 1807
 """
 ``VHADDPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 7C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VHADDPD_YMM_YMM_YMMM256: Code = 1808 # type: ignore
+VEX_VHADDPD_YMM_YMM_YMMM256: int = 1808
 """
 ``VHADDPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 7C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-HADDPS_XMM_XMMM128: Code = 1809 # type: ignore
+HADDPS_XMM_XMMM128: int = 1809
 """
 ``HADDPS xmm1, xmm2/m128``
 
 ``F2 0F 7C /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VHADDPS_XMM_XMM_XMMM128: Code = 1810 # type: ignore
+VEX_VHADDPS_XMM_XMM_XMMM128: int = 1810
 """
 ``VHADDPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.F2.0F.WIG 7C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VHADDPS_YMM_YMM_YMMM256: Code = 1811 # type: ignore
+VEX_VHADDPS_YMM_YMM_YMMM256: int = 1811
 """
 ``VHADDPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.F2.0F.WIG 7C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-HSUBPD_XMM_XMMM128: Code = 1812 # type: ignore
+HSUBPD_XMM_XMMM128: int = 1812
 """
 ``HSUBPD xmm1, xmm2/m128``
 
 ``66 0F 7D /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VHSUBPD_XMM_XMM_XMMM128: Code = 1813 # type: ignore
+VEX_VHSUBPD_XMM_XMM_XMMM128: int = 1813
 """
 ``VHSUBPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG 7D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VHSUBPD_YMM_YMM_YMMM256: Code = 1814 # type: ignore
+VEX_VHSUBPD_YMM_YMM_YMMM256: int = 1814
 """
 ``VHSUBPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG 7D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-HSUBPS_XMM_XMMM128: Code = 1815 # type: ignore
+HSUBPS_XMM_XMMM128: int = 1815
 """
 ``HSUBPS xmm1, xmm2/m128``
 
 ``F2 0F 7D /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VHSUBPS_XMM_XMM_XMMM128: Code = 1816 # type: ignore
+VEX_VHSUBPS_XMM_XMM_XMMM128: int = 1816
 """
 ``VHSUBPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.F2.0F.WIG 7D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VHSUBPS_YMM_YMM_YMMM256: Code = 1817 # type: ignore
+VEX_VHSUBPS_YMM_YMM_YMMM256: int = 1817
 """
 ``VHSUBPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.F2.0F.WIG 7D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-MOVD_RM32_MM: Code = 1818 # type: ignore
+MOVD_RM32_MM: int = 1818
 """
 ``MOVD r/m32, mm``
 
 ``NP 0F 7E /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-MOVQ_RM64_MM: Code = 1819 # type: ignore
+MOVQ_RM64_MM: int = 1819
 """
 ``MOVQ r/m64, mm``
 
 ``NP o64 0F 7E /r``
 
 ``MMX``
 
 ``64-bit``
 """
-MOVD_RM32_XMM: Code = 1820 # type: ignore
+MOVD_RM32_XMM: int = 1820
 """
 ``MOVD r/m32, xmm``
 
 ``66 0F 7E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MOVQ_RM64_XMM: Code = 1821 # type: ignore
+MOVQ_RM64_XMM: int = 1821
 """
 ``MOVQ r/m64, xmm``
 
 ``66 o64 0F 7E /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VMOVD_RM32_XMM: Code = 1822 # type: ignore
+VEX_VMOVD_RM32_XMM: int = 1822
 """
 ``VMOVD r/m32, xmm1``
 
 ``VEX.128.66.0F.W0 7E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVQ_RM64_XMM: Code = 1823 # type: ignore
+VEX_VMOVQ_RM64_XMM: int = 1823
 """
 ``VMOVQ r/m64, xmm1``
 
 ``VEX.128.66.0F.W1 7E /r``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VMOVD_RM32_XMM: Code = 1824 # type: ignore
+EVEX_VMOVD_RM32_XMM: int = 1824
 """
 ``VMOVD r/m32, xmm1``
 
 ``EVEX.128.66.0F.W0 7E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVQ_RM64_XMM: Code = 1825 # type: ignore
+EVEX_VMOVQ_RM64_XMM: int = 1825
 """
 ``VMOVQ r/m64, xmm1``
 
 ``EVEX.128.66.0F.W1 7E /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-MOVQ_XMM_XMMM64: Code = 1826 # type: ignore
+MOVQ_XMM_XMMM64: int = 1826
 """
 ``MOVQ xmm1, xmm2/m64``
 
 ``F3 0F 7E /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVQ_XMM_XMMM64: Code = 1827 # type: ignore
+VEX_VMOVQ_XMM_XMMM64: int = 1827
 """
 ``VMOVQ xmm1, xmm2/m64``
 
 ``VEX.128.F3.0F.WIG 7E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVQ_XMM_XMMM64: Code = 1828 # type: ignore
+EVEX_VMOVQ_XMM_XMMM64: int = 1828
 """
 ``VMOVQ xmm1, xmm2/m64``
 
 ``EVEX.128.F3.0F.W1 7E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVQ_MMM64_MM: Code = 1829 # type: ignore
+MOVQ_MMM64_MM: int = 1829
 """
 ``MOVQ mm/m64, mm``
 
 ``NP 0F 7F /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-MOVDQA_XMMM128_XMM: Code = 1830 # type: ignore
+MOVDQA_XMMM128_XMM: int = 1830
 """
 ``MOVDQA xmm2/m128, xmm1``
 
 ``66 0F 7F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQA_XMMM128_XMM: Code = 1831 # type: ignore
+VEX_VMOVDQA_XMMM128_XMM: int = 1831
 """
 ``VMOVDQA xmm2/m128, xmm1``
 
 ``VEX.128.66.0F.WIG 7F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQA_YMMM256_YMM: Code = 1832 # type: ignore
+VEX_VMOVDQA_YMMM256_YMM: int = 1832
 """
 ``VMOVDQA ymm2/m256, ymm1``
 
 ``VEX.256.66.0F.WIG 7F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_XMMM128_K1Z_XMM: Code = 1833 # type: ignore
+EVEX_VMOVDQA32_XMMM128_K1Z_XMM: int = 1833
 """
 ``VMOVDQA32 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.66.0F.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_YMMM256_K1Z_YMM: Code = 1834 # type: ignore
+EVEX_VMOVDQA32_YMMM256_K1Z_YMM: int = 1834
 """
 ``VMOVDQA32 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.66.0F.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA32_ZMMM512_K1Z_ZMM: Code = 1835 # type: ignore
+EVEX_VMOVDQA32_ZMMM512_K1Z_ZMM: int = 1835
 """
 ``VMOVDQA32 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.66.0F.W0 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_XMMM128_K1Z_XMM: Code = 1836 # type: ignore
+EVEX_VMOVDQA64_XMMM128_K1Z_XMM: int = 1836
 """
 ``VMOVDQA64 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.66.0F.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_YMMM256_K1Z_YMM: Code = 1837 # type: ignore
+EVEX_VMOVDQA64_YMMM256_K1Z_YMM: int = 1837
 """
 ``VMOVDQA64 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.66.0F.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQA64_ZMMM512_K1Z_ZMM: Code = 1838 # type: ignore
+EVEX_VMOVDQA64_ZMMM512_K1Z_ZMM: int = 1838
 """
 ``VMOVDQA64 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.66.0F.W1 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVDQU_XMMM128_XMM: Code = 1839 # type: ignore
+MOVDQU_XMMM128_XMM: int = 1839
 """
 ``MOVDQU xmm2/m128, xmm1``
 
 ``F3 0F 7F /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQU_XMMM128_XMM: Code = 1840 # type: ignore
+VEX_VMOVDQU_XMMM128_XMM: int = 1840
 """
 ``VMOVDQU xmm2/m128, xmm1``
 
 ``VEX.128.F3.0F.WIG 7F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVDQU_YMMM256_YMM: Code = 1841 # type: ignore
+VEX_VMOVDQU_YMMM256_YMM: int = 1841
 """
 ``VMOVDQU ymm2/m256, ymm1``
 
 ``VEX.256.F3.0F.WIG 7F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_XMMM128_K1Z_XMM: Code = 1842 # type: ignore
+EVEX_VMOVDQU32_XMMM128_K1Z_XMM: int = 1842
 """
 ``VMOVDQU32 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.F3.0F.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_YMMM256_K1Z_YMM: Code = 1843 # type: ignore
+EVEX_VMOVDQU32_YMMM256_K1Z_YMM: int = 1843
 """
 ``VMOVDQU32 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.F3.0F.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU32_ZMMM512_K1Z_ZMM: Code = 1844 # type: ignore
+EVEX_VMOVDQU32_ZMMM512_K1Z_ZMM: int = 1844
 """
 ``VMOVDQU32 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.F3.0F.W0 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_XMMM128_K1Z_XMM: Code = 1845 # type: ignore
+EVEX_VMOVDQU64_XMMM128_K1Z_XMM: int = 1845
 """
 ``VMOVDQU64 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.F3.0F.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_YMMM256_K1Z_YMM: Code = 1846 # type: ignore
+EVEX_VMOVDQU64_YMMM256_K1Z_YMM: int = 1846
 """
 ``VMOVDQU64 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.F3.0F.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU64_ZMMM512_K1Z_ZMM: Code = 1847 # type: ignore
+EVEX_VMOVDQU64_ZMMM512_K1Z_ZMM: int = 1847
 """
 ``VMOVDQU64 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.F3.0F.W1 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_XMMM128_K1Z_XMM: Code = 1848 # type: ignore
+EVEX_VMOVDQU8_XMMM128_K1Z_XMM: int = 1848
 """
 ``VMOVDQU8 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.F2.0F.W0 7F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_YMMM256_K1Z_YMM: Code = 1849 # type: ignore
+EVEX_VMOVDQU8_YMMM256_K1Z_YMM: int = 1849
 """
 ``VMOVDQU8 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.F2.0F.W0 7F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU8_ZMMM512_K1Z_ZMM: Code = 1850 # type: ignore
+EVEX_VMOVDQU8_ZMMM512_K1Z_ZMM: int = 1850
 """
 ``VMOVDQU8 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.F2.0F.W0 7F /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_XMMM128_K1Z_XMM: Code = 1851 # type: ignore
+EVEX_VMOVDQU16_XMMM128_K1Z_XMM: int = 1851
 """
 ``VMOVDQU16 xmm2/m128 {k1}{z}, xmm1``
 
 ``EVEX.128.F2.0F.W1 7F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_YMMM256_K1Z_YMM: Code = 1852 # type: ignore
+EVEX_VMOVDQU16_YMMM256_K1Z_YMM: int = 1852
 """
 ``VMOVDQU16 ymm2/m256 {k1}{z}, ymm1``
 
 ``EVEX.256.F2.0F.W1 7F /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVDQU16_ZMMM512_K1Z_ZMM: Code = 1853 # type: ignore
+EVEX_VMOVDQU16_ZMMM512_K1Z_ZMM: int = 1853
 """
 ``VMOVDQU16 zmm2/m512 {k1}{z}, zmm1``
 
 ``EVEX.512.F2.0F.W1 7F /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-JO_REL16: Code = 1854 # type: ignore
+JO_REL16: int = 1854
 """
 ``JO rel16``
 
 ``o16 0F 80 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JO_REL32_32: Code = 1855 # type: ignore
+JO_REL32_32: int = 1855
 """
 ``JO rel32``
 
 ``o32 0F 80 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JO_REL32_64: Code = 1856 # type: ignore
+JO_REL32_64: int = 1856
 """
 ``JO rel32``
 
 ``o64 0F 80 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JNO_REL16: Code = 1857 # type: ignore
+JNO_REL16: int = 1857
 """
 ``JNO rel16``
 
 ``o16 0F 81 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JNO_REL32_32: Code = 1858 # type: ignore
+JNO_REL32_32: int = 1858
 """
 ``JNO rel32``
 
 ``o32 0F 81 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNO_REL32_64: Code = 1859 # type: ignore
+JNO_REL32_64: int = 1859
 """
 ``JNO rel32``
 
 ``o64 0F 81 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JB_REL16: Code = 1860 # type: ignore
+JB_REL16: int = 1860
 """
 ``JB rel16``
 
 ``o16 0F 82 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JB_REL32_32: Code = 1861 # type: ignore
+JB_REL32_32: int = 1861
 """
 ``JB rel32``
 
 ``o32 0F 82 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JB_REL32_64: Code = 1862 # type: ignore
+JB_REL32_64: int = 1862
 """
 ``JB rel32``
 
 ``o64 0F 82 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JAE_REL16: Code = 1863 # type: ignore
+JAE_REL16: int = 1863
 """
 ``JAE rel16``
 
 ``o16 0F 83 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JAE_REL32_32: Code = 1864 # type: ignore
+JAE_REL32_32: int = 1864
 """
 ``JAE rel32``
 
 ``o32 0F 83 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JAE_REL32_64: Code = 1865 # type: ignore
+JAE_REL32_64: int = 1865
 """
 ``JAE rel32``
 
 ``o64 0F 83 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JE_REL16: Code = 1866 # type: ignore
+JE_REL16: int = 1866
 """
 ``JE rel16``
 
 ``o16 0F 84 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JE_REL32_32: Code = 1867 # type: ignore
+JE_REL32_32: int = 1867
 """
 ``JE rel32``
 
 ``o32 0F 84 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JE_REL32_64: Code = 1868 # type: ignore
+JE_REL32_64: int = 1868
 """
 ``JE rel32``
 
 ``o64 0F 84 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JNE_REL16: Code = 1869 # type: ignore
+JNE_REL16: int = 1869
 """
 ``JNE rel16``
 
 ``o16 0F 85 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JNE_REL32_32: Code = 1870 # type: ignore
+JNE_REL32_32: int = 1870
 """
 ``JNE rel32``
 
 ``o32 0F 85 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNE_REL32_64: Code = 1871 # type: ignore
+JNE_REL32_64: int = 1871
 """
 ``JNE rel32``
 
 ``o64 0F 85 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JBE_REL16: Code = 1872 # type: ignore
+JBE_REL16: int = 1872
 """
 ``JBE rel16``
 
 ``o16 0F 86 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JBE_REL32_32: Code = 1873 # type: ignore
+JBE_REL32_32: int = 1873
 """
 ``JBE rel32``
 
 ``o32 0F 86 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JBE_REL32_64: Code = 1874 # type: ignore
+JBE_REL32_64: int = 1874
 """
 ``JBE rel32``
 
 ``o64 0F 86 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JA_REL16: Code = 1875 # type: ignore
+JA_REL16: int = 1875
 """
 ``JA rel16``
 
 ``o16 0F 87 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JA_REL32_32: Code = 1876 # type: ignore
+JA_REL32_32: int = 1876
 """
 ``JA rel32``
 
 ``o32 0F 87 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JA_REL32_64: Code = 1877 # type: ignore
+JA_REL32_64: int = 1877
 """
 ``JA rel32``
 
 ``o64 0F 87 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JS_REL16: Code = 1878 # type: ignore
+JS_REL16: int = 1878
 """
 ``JS rel16``
 
 ``o16 0F 88 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JS_REL32_32: Code = 1879 # type: ignore
+JS_REL32_32: int = 1879
 """
 ``JS rel32``
 
 ``o32 0F 88 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JS_REL32_64: Code = 1880 # type: ignore
+JS_REL32_64: int = 1880
 """
 ``JS rel32``
 
 ``o64 0F 88 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JNS_REL16: Code = 1881 # type: ignore
+JNS_REL16: int = 1881
 """
 ``JNS rel16``
 
 ``o16 0F 89 cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JNS_REL32_32: Code = 1882 # type: ignore
+JNS_REL32_32: int = 1882
 """
 ``JNS rel32``
 
 ``o32 0F 89 cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNS_REL32_64: Code = 1883 # type: ignore
+JNS_REL32_64: int = 1883
 """
 ``JNS rel32``
 
 ``o64 0F 89 cd``
 
 ``X64``
 
 ``64-bit``
 """
-JP_REL16: Code = 1884 # type: ignore
+JP_REL16: int = 1884
 """
 ``JP rel16``
 
 ``o16 0F 8A cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JP_REL32_32: Code = 1885 # type: ignore
+JP_REL32_32: int = 1885
 """
 ``JP rel32``
 
 ``o32 0F 8A cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JP_REL32_64: Code = 1886 # type: ignore
+JP_REL32_64: int = 1886
 """
 ``JP rel32``
 
 ``o64 0F 8A cd``
 
 ``X64``
 
 ``64-bit``
 """
-JNP_REL16: Code = 1887 # type: ignore
+JNP_REL16: int = 1887
 """
 ``JNP rel16``
 
 ``o16 0F 8B cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JNP_REL32_32: Code = 1888 # type: ignore
+JNP_REL32_32: int = 1888
 """
 ``JNP rel32``
 
 ``o32 0F 8B cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JNP_REL32_64: Code = 1889 # type: ignore
+JNP_REL32_64: int = 1889
 """
 ``JNP rel32``
 
 ``o64 0F 8B cd``
 
 ``X64``
 
 ``64-bit``
 """
-JL_REL16: Code = 1890 # type: ignore
+JL_REL16: int = 1890
 """
 ``JL rel16``
 
 ``o16 0F 8C cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JL_REL32_32: Code = 1891 # type: ignore
+JL_REL32_32: int = 1891
 """
 ``JL rel32``
 
 ``o32 0F 8C cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JL_REL32_64: Code = 1892 # type: ignore
+JL_REL32_64: int = 1892
 """
 ``JL rel32``
 
 ``o64 0F 8C cd``
 
 ``X64``
 
 ``64-bit``
 """
-JGE_REL16: Code = 1893 # type: ignore
+JGE_REL16: int = 1893
 """
 ``JGE rel16``
 
 ``o16 0F 8D cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JGE_REL32_32: Code = 1894 # type: ignore
+JGE_REL32_32: int = 1894
 """
 ``JGE rel32``
 
 ``o32 0F 8D cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JGE_REL32_64: Code = 1895 # type: ignore
+JGE_REL32_64: int = 1895
 """
 ``JGE rel32``
 
 ``o64 0F 8D cd``
 
 ``X64``
 
 ``64-bit``
 """
-JLE_REL16: Code = 1896 # type: ignore
+JLE_REL16: int = 1896
 """
 ``JLE rel16``
 
 ``o16 0F 8E cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JLE_REL32_32: Code = 1897 # type: ignore
+JLE_REL32_32: int = 1897
 """
 ``JLE rel32``
 
 ``o32 0F 8E cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JLE_REL32_64: Code = 1898 # type: ignore
+JLE_REL32_64: int = 1898
 """
 ``JLE rel32``
 
 ``o64 0F 8E cd``
 
 ``X64``
 
 ``64-bit``
 """
-JG_REL16: Code = 1899 # type: ignore
+JG_REL16: int = 1899
 """
 ``JG rel16``
 
 ``o16 0F 8F cw``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-JG_REL32_32: Code = 1900 # type: ignore
+JG_REL32_32: int = 1900
 """
 ``JG rel32``
 
 ``o32 0F 8F cd``
 
 ``386+``
 
 ``16/32-bit``
 """
-JG_REL32_64: Code = 1901 # type: ignore
+JG_REL32_64: int = 1901
 """
 ``JG rel32``
 
 ``o64 0F 8F cd``
 
 ``X64``
 
 ``64-bit``
 """
-SETO_RM8: Code = 1902 # type: ignore
+SETO_RM8: int = 1902
 """
 ``SETO r/m8``
 
 ``0F 90 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETNO_RM8: Code = 1903 # type: ignore
+SETNO_RM8: int = 1903
 """
 ``SETNO r/m8``
 
 ``0F 91 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETB_RM8: Code = 1904 # type: ignore
+SETB_RM8: int = 1904
 """
 ``SETB r/m8``
 
 ``0F 92 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETAE_RM8: Code = 1905 # type: ignore
+SETAE_RM8: int = 1905
 """
 ``SETAE r/m8``
 
 ``0F 93 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETE_RM8: Code = 1906 # type: ignore
+SETE_RM8: int = 1906
 """
 ``SETE r/m8``
 
 ``0F 94 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETNE_RM8: Code = 1907 # type: ignore
+SETNE_RM8: int = 1907
 """
 ``SETNE r/m8``
 
 ``0F 95 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETBE_RM8: Code = 1908 # type: ignore
+SETBE_RM8: int = 1908
 """
 ``SETBE r/m8``
 
 ``0F 96 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETA_RM8: Code = 1909 # type: ignore
+SETA_RM8: int = 1909
 """
 ``SETA r/m8``
 
 ``0F 97 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETS_RM8: Code = 1910 # type: ignore
+SETS_RM8: int = 1910
 """
 ``SETS r/m8``
 
 ``0F 98 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETNS_RM8: Code = 1911 # type: ignore
+SETNS_RM8: int = 1911
 """
 ``SETNS r/m8``
 
 ``0F 99 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETP_RM8: Code = 1912 # type: ignore
+SETP_RM8: int = 1912
 """
 ``SETP r/m8``
 
 ``0F 9A /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETNP_RM8: Code = 1913 # type: ignore
+SETNP_RM8: int = 1913
 """
 ``SETNP r/m8``
 
 ``0F 9B /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETL_RM8: Code = 1914 # type: ignore
+SETL_RM8: int = 1914
 """
 ``SETL r/m8``
 
 ``0F 9C /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETGE_RM8: Code = 1915 # type: ignore
+SETGE_RM8: int = 1915
 """
 ``SETGE r/m8``
 
 ``0F 9D /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETLE_RM8: Code = 1916 # type: ignore
+SETLE_RM8: int = 1916
 """
 ``SETLE r/m8``
 
 ``0F 9E /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SETG_RM8: Code = 1917 # type: ignore
+SETG_RM8: int = 1917
 """
 ``SETG r/m8``
 
 ``0F 9F /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-VEX_KMOVW_KR_KM16: Code = 1918 # type: ignore
+VEX_KMOVW_KR_KM16: int = 1918
 """
 ``KMOVW k1, k2/m16``
 
 ``VEX.L0.0F.W0 90 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KMOVQ_KR_KM64: Code = 1919 # type: ignore
+VEX_KMOVQ_KR_KM64: int = 1919
 """
 ``KMOVQ k1, k2/m64``
 
 ``VEX.L0.0F.W1 90 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVB_KR_KM8: Code = 1920 # type: ignore
+VEX_KMOVB_KR_KM8: int = 1920
 """
 ``KMOVB k1, k2/m8``
 
 ``VEX.L0.66.0F.W0 90 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KMOVD_KR_KM32: Code = 1921 # type: ignore
+VEX_KMOVD_KR_KM32: int = 1921
 """
 ``KMOVD k1, k2/m32``
 
 ``VEX.L0.66.0F.W1 90 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVW_M16_KR: Code = 1922 # type: ignore
+VEX_KMOVW_M16_KR: int = 1922
 """
 ``KMOVW m16, k1``
 
 ``VEX.L0.0F.W0 91 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KMOVQ_M64_KR: Code = 1923 # type: ignore
+VEX_KMOVQ_M64_KR: int = 1923
 """
 ``KMOVQ m64, k1``
 
 ``VEX.L0.0F.W1 91 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVB_M8_KR: Code = 1924 # type: ignore
+VEX_KMOVB_M8_KR: int = 1924
 """
 ``KMOVB m8, k1``
 
 ``VEX.L0.66.0F.W0 91 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KMOVD_M32_KR: Code = 1925 # type: ignore
+VEX_KMOVD_M32_KR: int = 1925
 """
 ``KMOVD m32, k1``
 
 ``VEX.L0.66.0F.W1 91 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVW_KR_R32: Code = 1926 # type: ignore
+VEX_KMOVW_KR_R32: int = 1926
 """
 ``KMOVW k1, r32``
 
 ``VEX.L0.0F.W0 92 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KMOVB_KR_R32: Code = 1927 # type: ignore
+VEX_KMOVB_KR_R32: int = 1927
 """
 ``KMOVB k1, r32``
 
 ``VEX.L0.66.0F.W0 92 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KMOVD_KR_R32: Code = 1928 # type: ignore
+VEX_KMOVD_KR_R32: int = 1928
 """
 ``KMOVD k1, r32``
 
 ``VEX.L0.F2.0F.W0 92 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVQ_KR_R64: Code = 1929 # type: ignore
+VEX_KMOVQ_KR_R64: int = 1929
 """
 ``KMOVQ k1, r64``
 
 ``VEX.L0.F2.0F.W1 92 /r``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-VEX_KMOVW_R32_KR: Code = 1930 # type: ignore
+VEX_KMOVW_R32_KR: int = 1930
 """
 ``KMOVW r32, k1``
 
 ``VEX.L0.0F.W0 93 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KMOVB_R32_KR: Code = 1931 # type: ignore
+VEX_KMOVB_R32_KR: int = 1931
 """
 ``KMOVB r32, k1``
 
 ``VEX.L0.66.0F.W0 93 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KMOVD_R32_KR: Code = 1932 # type: ignore
+VEX_KMOVD_R32_KR: int = 1932
 """
 ``KMOVD r32, k1``
 
 ``VEX.L0.F2.0F.W0 93 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KMOVQ_R64_KR: Code = 1933 # type: ignore
+VEX_KMOVQ_R64_KR: int = 1933
 """
 ``KMOVQ r64, k1``
 
 ``VEX.L0.F2.0F.W1 93 /r``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-VEX_KORTESTW_KR_KR: Code = 1934 # type: ignore
+VEX_KORTESTW_KR_KR: int = 1934
 """
 ``KORTESTW k1, k2``
 
 ``VEX.L0.0F.W0 98 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KORTESTQ_KR_KR: Code = 1935 # type: ignore
+VEX_KORTESTQ_KR_KR: int = 1935
 """
 ``KORTESTQ k1, k2``
 
 ``VEX.L0.0F.W1 98 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KORTESTB_KR_KR: Code = 1936 # type: ignore
+VEX_KORTESTB_KR_KR: int = 1936
 """
 ``KORTESTB k1, k2``
 
 ``VEX.L0.66.0F.W0 98 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KORTESTD_KR_KR: Code = 1937 # type: ignore
+VEX_KORTESTD_KR_KR: int = 1937
 """
 ``KORTESTD k1, k2``
 
 ``VEX.L0.66.0F.W1 98 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KTESTW_KR_KR: Code = 1938 # type: ignore
+VEX_KTESTW_KR_KR: int = 1938
 """
 ``KTESTW k1, k2``
 
 ``VEX.L0.0F.W0 99 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KTESTQ_KR_KR: Code = 1939 # type: ignore
+VEX_KTESTQ_KR_KR: int = 1939
 """
 ``KTESTQ k1, k2``
 
 ``VEX.L0.0F.W1 99 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KTESTB_KR_KR: Code = 1940 # type: ignore
+VEX_KTESTB_KR_KR: int = 1940
 """
 ``KTESTB k1, k2``
 
 ``VEX.L0.66.0F.W0 99 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KTESTD_KR_KR: Code = 1941 # type: ignore
+VEX_KTESTD_KR_KR: int = 1941
 """
 ``KTESTD k1, k2``
 
 ``VEX.L0.66.0F.W1 99 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PUSHW_FS: Code = 1942 # type: ignore
+PUSHW_FS: int = 1942
 """
 ``PUSH FS``
 
 ``o16 0F A0``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-PUSHD_FS: Code = 1943 # type: ignore
+PUSHD_FS: int = 1943
 """
 ``PUSH FS``
 
 ``o32 0F A0``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSHQ_FS: Code = 1944 # type: ignore
+PUSHQ_FS: int = 1944
 """
 ``PUSH FS``
 
 ``o64 0F A0``
 
 ``X64``
 
 ``64-bit``
 """
-POPW_FS: Code = 1945 # type: ignore
+POPW_FS: int = 1945
 """
 ``POP FS``
 
 ``o16 0F A1``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-POPD_FS: Code = 1946 # type: ignore
+POPD_FS: int = 1946
 """
 ``POP FS``
 
 ``o32 0F A1``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPQ_FS: Code = 1947 # type: ignore
+POPQ_FS: int = 1947
 """
 ``POP FS``
 
 ``o64 0F A1``
 
 ``X64``
 
 ``64-bit``
 """
-CPUID: Code = 1948 # type: ignore
+CPUID: int = 1948
 """
 ``CPUID``
 
 ``0F A2``
 
 ``CPUID``
 
 ``16/32/64-bit``
 """
-BT_RM16_R16: Code = 1949 # type: ignore
+BT_RM16_R16: int = 1949
 """
 ``BT r/m16, r16``
 
 ``o16 0F A3 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BT_RM32_R32: Code = 1950 # type: ignore
+BT_RM32_R32: int = 1950
 """
 ``BT r/m32, r32``
 
 ``o32 0F A3 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BT_RM64_R64: Code = 1951 # type: ignore
+BT_RM64_R64: int = 1951
 """
 ``BT r/m64, r64``
 
 ``o64 0F A3 /r``
 
 ``X64``
 
 ``64-bit``
 """
-SHLD_RM16_R16_IMM8: Code = 1952 # type: ignore
+SHLD_RM16_R16_IMM8: int = 1952
 """
 ``SHLD r/m16, r16, imm8``
 
 ``o16 0F A4 /r ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHLD_RM32_R32_IMM8: Code = 1953 # type: ignore
+SHLD_RM32_R32_IMM8: int = 1953
 """
 ``SHLD r/m32, r32, imm8``
 
 ``o32 0F A4 /r ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHLD_RM64_R64_IMM8: Code = 1954 # type: ignore
+SHLD_RM64_R64_IMM8: int = 1954
 """
 ``SHLD r/m64, r64, imm8``
 
 ``o64 0F A4 /r ib``
 
 ``X64``
 
 ``64-bit``
 """
-SHLD_RM16_R16_CL: Code = 1955 # type: ignore
+SHLD_RM16_R16_CL: int = 1955
 """
 ``SHLD r/m16, r16, CL``
 
 ``o16 0F A5 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHLD_RM32_R32_CL: Code = 1956 # type: ignore
+SHLD_RM32_R32_CL: int = 1956
 """
 ``SHLD r/m32, r32, CL``
 
 ``o32 0F A5 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHLD_RM64_R64_CL: Code = 1957 # type: ignore
+SHLD_RM64_R64_CL: int = 1957
 """
 ``SHLD r/m64, r64, CL``
 
 ``o64 0F A5 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MONTMUL_16: Code = 1958 # type: ignore
+MONTMUL_16: int = 1958
 """
 ``MONTMUL``
 
 ``a16 F3 0F A6 C0``
 
 ``PADLOCK_PMM``
 
 ``16/32-bit``
 """
-MONTMUL_32: Code = 1959 # type: ignore
+MONTMUL_32: int = 1959
 """
 ``MONTMUL``
 
 ``a32 F3 0F A6 C0``
 
 ``PADLOCK_PMM``
 
 ``16/32/64-bit``
 """
-MONTMUL_64: Code = 1960 # type: ignore
+MONTMUL_64: int = 1960
 """
 ``MONTMUL``
 
 ``a64 F3 0F A6 C0``
 
 ``PADLOCK_PMM``
 
 ``64-bit``
 """
-XSHA1_16: Code = 1961 # type: ignore
+XSHA1_16: int = 1961
 """
 ``XSHA1``
 
 ``a16 F3 0F A6 C8``
 
 ``PADLOCK_PHE``
 
 ``16/32-bit``
 """
-XSHA1_32: Code = 1962 # type: ignore
+XSHA1_32: int = 1962
 """
 ``XSHA1``
 
 ``a32 F3 0F A6 C8``
 
 ``PADLOCK_PHE``
 
 ``16/32/64-bit``
 """
-XSHA1_64: Code = 1963 # type: ignore
+XSHA1_64: int = 1963
 """
 ``XSHA1``
 
 ``a64 F3 0F A6 C8``
 
 ``PADLOCK_PHE``
 
 ``64-bit``
 """
-XSHA256_16: Code = 1964 # type: ignore
+XSHA256_16: int = 1964
 """
 ``XSHA256``
 
 ``a16 F3 0F A6 D0``
 
 ``PADLOCK_PHE``
 
 ``16/32-bit``
 """
-XSHA256_32: Code = 1965 # type: ignore
+XSHA256_32: int = 1965
 """
 ``XSHA256``
 
 ``a32 F3 0F A6 D0``
 
 ``PADLOCK_PHE``
 
 ``16/32/64-bit``
 """
-XSHA256_64: Code = 1966 # type: ignore
+XSHA256_64: int = 1966
 """
 ``XSHA256``
 
 ``a64 F3 0F A6 D0``
 
 ``PADLOCK_PHE``
 
 ``64-bit``
 """
-XBTS_R16_RM16: Code = 1967 # type: ignore
+XBTS_R16_RM16: int = 1967
 """
 ``XBTS r16, r/m16``
 
 ``o16 0F A6 /r``
 
 ``386 A0``
 
 ``16/32-bit``
 """
-XBTS_R32_RM32: Code = 1968 # type: ignore
+XBTS_R32_RM32: int = 1968
 """
 ``XBTS r32, r/m32``
 
 ``o32 0F A6 /r``
 
 ``386 A0``
 
 ``16/32-bit``
 """
-XSTORE_16: Code = 1969 # type: ignore
+XSTORE_16: int = 1969
 """
 ``XSTORE``
 
 ``a16 0F A7 C0``
 
 ``PADLOCK_RNG``
 
 ``16/32-bit``
 """
-XSTORE_32: Code = 1970 # type: ignore
+XSTORE_32: int = 1970
 """
 ``XSTORE``
 
 ``a32 0F A7 C0``
 
 ``PADLOCK_RNG``
 
 ``16/32/64-bit``
 """
-XSTORE_64: Code = 1971 # type: ignore
+XSTORE_64: int = 1971
 """
 ``XSTORE``
 
 ``a64 0F A7 C0``
 
 ``PADLOCK_RNG``
 
 ``64-bit``
 """
-XCRYPTECB_16: Code = 1972 # type: ignore
+XCRYPTECB_16: int = 1972
 """
 ``XCRYPTECB``
 
 ``a16 F3 0F A7 C8``
 
 ``PADLOCK_ACE``
 
 ``16/32-bit``
 """
-XCRYPTECB_32: Code = 1973 # type: ignore
+XCRYPTECB_32: int = 1973
 """
 ``XCRYPTECB``
 
 ``a32 F3 0F A7 C8``
 
 ``PADLOCK_ACE``
 
 ``16/32/64-bit``
 """
-XCRYPTECB_64: Code = 1974 # type: ignore
+XCRYPTECB_64: int = 1974
 """
 ``XCRYPTECB``
 
 ``a64 F3 0F A7 C8``
 
 ``PADLOCK_ACE``
 
 ``64-bit``
 """
-XCRYPTCBC_16: Code = 1975 # type: ignore
+XCRYPTCBC_16: int = 1975
 """
 ``XCRYPTCBC``
 
 ``a16 F3 0F A7 D0``
 
 ``PADLOCK_ACE``
 
 ``16/32-bit``
 """
-XCRYPTCBC_32: Code = 1976 # type: ignore
+XCRYPTCBC_32: int = 1976
 """
 ``XCRYPTCBC``
 
 ``a32 F3 0F A7 D0``
 
 ``PADLOCK_ACE``
 
 ``16/32/64-bit``
 """
-XCRYPTCBC_64: Code = 1977 # type: ignore
+XCRYPTCBC_64: int = 1977
 """
 ``XCRYPTCBC``
 
 ``a64 F3 0F A7 D0``
 
 ``PADLOCK_ACE``
 
 ``64-bit``
 """
-XCRYPTCTR_16: Code = 1978 # type: ignore
+XCRYPTCTR_16: int = 1978
 """
 ``XCRYPTCTR``
 
 ``a16 F3 0F A7 D8``
 
 ``PADLOCK_ACE``
 
 ``16/32-bit``
 """
-XCRYPTCTR_32: Code = 1979 # type: ignore
+XCRYPTCTR_32: int = 1979
 """
 ``XCRYPTCTR``
 
 ``a32 F3 0F A7 D8``
 
 ``PADLOCK_ACE``
 
 ``16/32/64-bit``
 """
-XCRYPTCTR_64: Code = 1980 # type: ignore
+XCRYPTCTR_64: int = 1980
 """
 ``XCRYPTCTR``
 
 ``a64 F3 0F A7 D8``
 
 ``PADLOCK_ACE``
 
 ``64-bit``
 """
-XCRYPTCFB_16: Code = 1981 # type: ignore
+XCRYPTCFB_16: int = 1981
 """
 ``XCRYPTCFB``
 
 ``a16 F3 0F A7 E0``
 
 ``PADLOCK_ACE``
 
 ``16/32-bit``
 """
-XCRYPTCFB_32: Code = 1982 # type: ignore
+XCRYPTCFB_32: int = 1982
 """
 ``XCRYPTCFB``
 
 ``a32 F3 0F A7 E0``
 
 ``PADLOCK_ACE``
 
 ``16/32/64-bit``
 """
-XCRYPTCFB_64: Code = 1983 # type: ignore
+XCRYPTCFB_64: int = 1983
 """
 ``XCRYPTCFB``
 
 ``a64 F3 0F A7 E0``
 
 ``PADLOCK_ACE``
 
 ``64-bit``
 """
-XCRYPTOFB_16: Code = 1984 # type: ignore
+XCRYPTOFB_16: int = 1984
 """
 ``XCRYPTOFB``
 
 ``a16 F3 0F A7 E8``
 
 ``PADLOCK_ACE``
 
 ``16/32-bit``
 """
-XCRYPTOFB_32: Code = 1985 # type: ignore
+XCRYPTOFB_32: int = 1985
 """
 ``XCRYPTOFB``
 
 ``a32 F3 0F A7 E8``
 
 ``PADLOCK_ACE``
 
 ``16/32/64-bit``
 """
-XCRYPTOFB_64: Code = 1986 # type: ignore
+XCRYPTOFB_64: int = 1986
 """
 ``XCRYPTOFB``
 
 ``a64 F3 0F A7 E8``
 
 ``PADLOCK_ACE``
 
 ``64-bit``
 """
-IBTS_RM16_R16: Code = 1987 # type: ignore
+IBTS_RM16_R16: int = 1987
 """
 ``IBTS r/m16, r16``
 
 ``o16 0F A7 /r``
 
 ``386 A0``
 
 ``16/32-bit``
 """
-IBTS_RM32_R32: Code = 1988 # type: ignore
+IBTS_RM32_R32: int = 1988
 """
 ``IBTS r/m32, r32``
 
 ``o32 0F A7 /r``
 
 ``386 A0``
 
 ``16/32-bit``
 """
-CMPXCHG486_RM8_R8: Code = 1989 # type: ignore
+CMPXCHG486_RM8_R8: int = 1989
 """
 ``CMPXCHG r/m8, r8``
 
 ``0F A6 /r``
 
 ``486 A``
 
 ``16/32-bit``
 """
-CMPXCHG486_RM16_R16: Code = 1990 # type: ignore
+CMPXCHG486_RM16_R16: int = 1990
 """
 ``CMPXCHG r/m16, r16``
 
 ``o16 0F A7 /r``
 
 ``486 A``
 
 ``16/32-bit``
 """
-CMPXCHG486_RM32_R32: Code = 1991 # type: ignore
+CMPXCHG486_RM32_R32: int = 1991
 """
 ``CMPXCHG r/m32, r32``
 
 ``o32 0F A7 /r``
 
 ``486 A``
 
 ``16/32-bit``
 """
-PUSHW_GS: Code = 1992 # type: ignore
+PUSHW_GS: int = 1992
 """
 ``PUSH GS``
 
 ``o16 0F A8``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-PUSHD_GS: Code = 1993 # type: ignore
+PUSHD_GS: int = 1993
 """
 ``PUSH GS``
 
 ``o32 0F A8``
 
 ``386+``
 
 ``16/32-bit``
 """
-PUSHQ_GS: Code = 1994 # type: ignore
+PUSHQ_GS: int = 1994
 """
 ``PUSH GS``
 
 ``o64 0F A8``
 
 ``X64``
 
 ``64-bit``
 """
-POPW_GS: Code = 1995 # type: ignore
+POPW_GS: int = 1995
 """
 ``POP GS``
 
 ``o16 0F A9``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-POPD_GS: Code = 1996 # type: ignore
+POPD_GS: int = 1996
 """
 ``POP GS``
 
 ``o32 0F A9``
 
 ``386+``
 
 ``16/32-bit``
 """
-POPQ_GS: Code = 1997 # type: ignore
+POPQ_GS: int = 1997
 """
 ``POP GS``
 
 ``o64 0F A9``
 
 ``X64``
 
 ``64-bit``
 """
-RSM: Code = 1998 # type: ignore
+RSM: int = 1998
 """
 ``RSM``
 
 ``0F AA``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTS_RM16_R16: Code = 1999 # type: ignore
+BTS_RM16_R16: int = 1999
 """
 ``BTS r/m16, r16``
 
 ``o16 0F AB /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTS_RM32_R32: Code = 2000 # type: ignore
+BTS_RM32_R32: int = 2000
 """
 ``BTS r/m32, r32``
 
 ``o32 0F AB /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTS_RM64_R64: Code = 2001 # type: ignore
+BTS_RM64_R64: int = 2001
 """
 ``BTS r/m64, r64``
 
 ``o64 0F AB /r``
 
 ``X64``
 
 ``64-bit``
 """
-SHRD_RM16_R16_IMM8: Code = 2002 # type: ignore
+SHRD_RM16_R16_IMM8: int = 2002
 """
 ``SHRD r/m16, r16, imm8``
 
 ``o16 0F AC /r ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHRD_RM32_R32_IMM8: Code = 2003 # type: ignore
+SHRD_RM32_R32_IMM8: int = 2003
 """
 ``SHRD r/m32, r32, imm8``
 
 ``o32 0F AC /r ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHRD_RM64_R64_IMM8: Code = 2004 # type: ignore
+SHRD_RM64_R64_IMM8: int = 2004
 """
 ``SHRD r/m64, r64, imm8``
 
 ``o64 0F AC /r ib``
 
 ``X64``
 
 ``64-bit``
 """
-SHRD_RM16_R16_CL: Code = 2005 # type: ignore
+SHRD_RM16_R16_CL: int = 2005
 """
 ``SHRD r/m16, r16, CL``
 
 ``o16 0F AD /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHRD_RM32_R32_CL: Code = 2006 # type: ignore
+SHRD_RM32_R32_CL: int = 2006
 """
 ``SHRD r/m32, r32, CL``
 
 ``o32 0F AD /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-SHRD_RM64_R64_CL: Code = 2007 # type: ignore
+SHRD_RM64_R64_CL: int = 2007
 """
 ``SHRD r/m64, r64, CL``
 
 ``o64 0F AD /r``
 
 ``X64``
 
 ``64-bit``
 """
-FXSAVE_M512BYTE: Code = 2008 # type: ignore
+FXSAVE_M512BYTE: int = 2008
 """
 ``FXSAVE m512byte``
 
 ``NP 0F AE /0``
 
 ``FXSR``
 
 ``16/32/64-bit``
 """
-FXSAVE64_M512BYTE: Code = 2009 # type: ignore
+FXSAVE64_M512BYTE: int = 2009
 """
 ``FXSAVE64 m512byte``
 
 ``NP o64 0F AE /0``
 
 ``FXSR``
 
 ``64-bit``
 """
-RDFSBASE_R32: Code = 2010 # type: ignore
+RDFSBASE_R32: int = 2010
 """
 ``RDFSBASE r32``
 
 ``F3 0F AE /0``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-RDFSBASE_R64: Code = 2011 # type: ignore
+RDFSBASE_R64: int = 2011
 """
 ``RDFSBASE r64``
 
 ``F3 o64 0F AE /0``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-FXRSTOR_M512BYTE: Code = 2012 # type: ignore
+FXRSTOR_M512BYTE: int = 2012
 """
 ``FXRSTOR m512byte``
 
 ``NP 0F AE /1``
 
 ``FXSR``
 
 ``16/32/64-bit``
 """
-FXRSTOR64_M512BYTE: Code = 2013 # type: ignore
+FXRSTOR64_M512BYTE: int = 2013
 """
 ``FXRSTOR64 m512byte``
 
 ``NP o64 0F AE /1``
 
 ``FXSR``
 
 ``64-bit``
 """
-RDGSBASE_R32: Code = 2014 # type: ignore
+RDGSBASE_R32: int = 2014
 """
 ``RDGSBASE r32``
 
 ``F3 0F AE /1``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-RDGSBASE_R64: Code = 2015 # type: ignore
+RDGSBASE_R64: int = 2015
 """
 ``RDGSBASE r64``
 
 ``F3 o64 0F AE /1``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-LDMXCSR_M32: Code = 2016 # type: ignore
+LDMXCSR_M32: int = 2016
 """
 ``LDMXCSR m32``
 
 ``NP 0F AE /2``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-WRFSBASE_R32: Code = 2017 # type: ignore
+WRFSBASE_R32: int = 2017
 """
 ``WRFSBASE r32``
 
 ``F3 0F AE /2``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-WRFSBASE_R64: Code = 2018 # type: ignore
+WRFSBASE_R64: int = 2018
 """
 ``WRFSBASE r64``
 
 ``F3 o64 0F AE /2``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-VEX_VLDMXCSR_M32: Code = 2019 # type: ignore
+VEX_VLDMXCSR_M32: int = 2019
 """
 ``VLDMXCSR m32``
 
 ``VEX.LZ.0F.WIG AE /2``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-STMXCSR_M32: Code = 2020 # type: ignore
+STMXCSR_M32: int = 2020
 """
 ``STMXCSR m32``
 
 ``NP 0F AE /3``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-WRGSBASE_R32: Code = 2021 # type: ignore
+WRGSBASE_R32: int = 2021
 """
 ``WRGSBASE r32``
 
 ``F3 0F AE /3``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-WRGSBASE_R64: Code = 2022 # type: ignore
+WRGSBASE_R64: int = 2022
 """
 ``WRGSBASE r64``
 
 ``F3 o64 0F AE /3``
 
 ``FSGSBASE``
 
 ``64-bit``
 """
-VEX_VSTMXCSR_M32: Code = 2023 # type: ignore
+VEX_VSTMXCSR_M32: int = 2023
 """
 ``VSTMXCSR m32``
 
 ``VEX.LZ.0F.WIG AE /3``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-XSAVE_MEM: Code = 2024 # type: ignore
+XSAVE_MEM: int = 2024
 """
 ``XSAVE mem``
 
 ``NP 0F AE /4``
 
 ``XSAVE``
 
 ``16/32/64-bit``
 """
-XSAVE64_MEM: Code = 2025 # type: ignore
+XSAVE64_MEM: int = 2025
 """
 ``XSAVE64 mem``
 
 ``NP o64 0F AE /4``
 
 ``XSAVE``
 
 ``64-bit``
 """
-PTWRITE_RM32: Code = 2026 # type: ignore
+PTWRITE_RM32: int = 2026
 """
 ``PTWRITE r/m32``
 
 ``F3 0F AE /4``
 
 ``PTWRITE``
 
 ``16/32/64-bit``
 """
-PTWRITE_RM64: Code = 2027 # type: ignore
+PTWRITE_RM64: int = 2027
 """
 ``PTWRITE r/m64``
 
 ``F3 o64 0F AE /4``
 
 ``PTWRITE``
 
 ``64-bit``
 """
-XRSTOR_MEM: Code = 2028 # type: ignore
+XRSTOR_MEM: int = 2028
 """
 ``XRSTOR mem``
 
 ``NP 0F AE /5``
 
 ``XSAVE``
 
 ``16/32/64-bit``
 """
-XRSTOR64_MEM: Code = 2029 # type: ignore
+XRSTOR64_MEM: int = 2029
 """
 ``XRSTOR64 mem``
 
 ``NP o64 0F AE /5``
 
 ``XSAVE``
 
 ``64-bit``
 """
-INCSSPD_R32: Code = 2030 # type: ignore
+INCSSPD_R32: int = 2030
 """
 ``INCSSPD r32``
 
 ``F3 0F AE /5``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-INCSSPQ_R64: Code = 2031 # type: ignore
+INCSSPQ_R64: int = 2031
 """
 ``INCSSPQ r64``
 
 ``F3 o64 0F AE /5``
 
 ``CET_SS``
 
 ``64-bit``
 """
-XSAVEOPT_MEM: Code = 2032 # type: ignore
+XSAVEOPT_MEM: int = 2032
 """
 ``XSAVEOPT mem``
 
 ``NP 0F AE /6``
 
 ``XSAVEOPT``
 
 ``16/32/64-bit``
 """
-XSAVEOPT64_MEM: Code = 2033 # type: ignore
+XSAVEOPT64_MEM: int = 2033
 """
 ``XSAVEOPT64 mem``
 
 ``NP o64 0F AE /6``
 
 ``XSAVEOPT``
 
 ``64-bit``
 """
-CLWB_M8: Code = 2034 # type: ignore
+CLWB_M8: int = 2034
 """
 ``CLWB m8``
 
 ``66 0F AE /6``
 
 ``CLWB``
 
 ``16/32/64-bit``
 """
-TPAUSE_R32: Code = 2035 # type: ignore
+TPAUSE_R32: int = 2035
 """
 ``TPAUSE r32, <edx>, <eax>``
 
 ``66 0F AE /6``
 
 ``WAITPKG``
 
 ``16/32/64-bit``
 """
-TPAUSE_R64: Code = 2036 # type: ignore
+TPAUSE_R64: int = 2036
 """
 ``TPAUSE r64, <edx>, <eax>``
 
 ``66 o64 0F AE /6``
 
 ``WAITPKG``
 
 ``64-bit``
 """
-CLRSSBSY_M64: Code = 2037 # type: ignore
+CLRSSBSY_M64: int = 2037
 """
 ``CLRSSBSY m64``
 
 ``F3 0F AE /6``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-UMONITOR_R16: Code = 2038 # type: ignore
+UMONITOR_R16: int = 2038
 """
 ``UMONITOR r16``
 
 ``a16 F3 0F AE /6``
 
 ``WAITPKG``
 
 ``16/32-bit``
 """
-UMONITOR_R32: Code = 2039 # type: ignore
+UMONITOR_R32: int = 2039
 """
 ``UMONITOR r32``
 
 ``a32 F3 0F AE /6``
 
 ``WAITPKG``
 
 ``16/32/64-bit``
 """
-UMONITOR_R64: Code = 2040 # type: ignore
+UMONITOR_R64: int = 2040
 """
 ``UMONITOR r64``
 
 ``a64 F3 0F AE /6``
 
 ``WAITPKG``
 
 ``64-bit``
 """
-UMWAIT_R32: Code = 2041 # type: ignore
+UMWAIT_R32: int = 2041
 """
 ``UMWAIT r32, <edx>, <eax>``
 
 ``F2 0F AE /6``
 
 ``WAITPKG``
 
 ``16/32/64-bit``
 """
-UMWAIT_R64: Code = 2042 # type: ignore
+UMWAIT_R64: int = 2042
 """
 ``UMWAIT r64, <edx>, <eax>``
 
 ``F2 o64 0F AE /6``
 
 ``WAITPKG``
 
 ``64-bit``
 """
-CLFLUSH_M8: Code = 2043 # type: ignore
+CLFLUSH_M8: int = 2043
 """
 ``CLFLUSH m8``
 
 ``NP 0F AE /7``
 
 ``CLFSH``
 
 ``16/32/64-bit``
 """
-CLFLUSHOPT_M8: Code = 2044 # type: ignore
+CLFLUSHOPT_M8: int = 2044
 """
 ``CLFLUSHOPT m8``
 
 ``66 0F AE /7``
 
 ``CLFLUSHOPT``
 
 ``16/32/64-bit``
 """
-LFENCE: Code = 2045 # type: ignore
+LFENCE: int = 2045
 """
 ``LFENCE``
 
 ``NP 0F AE E8``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_E9: Code = 2046 # type: ignore
+LFENCE_E9: int = 2046
 """
 ``LFENCE``
 
 ``NP 0F AE E9``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_EA: Code = 2047 # type: ignore
+LFENCE_EA: int = 2047
 """
 ``LFENCE``
 
 ``NP 0F AE EA``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_EB: Code = 2048 # type: ignore
+LFENCE_EB: int = 2048
 """
 ``LFENCE``
 
 ``NP 0F AE EB``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_EC: Code = 2049 # type: ignore
+LFENCE_EC: int = 2049
 """
 ``LFENCE``
 
 ``NP 0F AE EC``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_ED: Code = 2050 # type: ignore
+LFENCE_ED: int = 2050
 """
 ``LFENCE``
 
 ``NP 0F AE ED``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_EE: Code = 2051 # type: ignore
+LFENCE_EE: int = 2051
 """
 ``LFENCE``
 
 ``NP 0F AE EE``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-LFENCE_EF: Code = 2052 # type: ignore
+LFENCE_EF: int = 2052
 """
 ``LFENCE``
 
 ``NP 0F AE EF``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE: Code = 2053 # type: ignore
+MFENCE: int = 2053
 """
 ``MFENCE``
 
 ``NP 0F AE F0``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F1: Code = 2054 # type: ignore
+MFENCE_F1: int = 2054
 """
 ``MFENCE``
 
 ``NP 0F AE F1``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F2: Code = 2055 # type: ignore
+MFENCE_F2: int = 2055
 """
 ``MFENCE``
 
 ``NP 0F AE F2``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F3: Code = 2056 # type: ignore
+MFENCE_F3: int = 2056
 """
 ``MFENCE``
 
 ``NP 0F AE F3``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F4: Code = 2057 # type: ignore
+MFENCE_F4: int = 2057
 """
 ``MFENCE``
 
 ``NP 0F AE F4``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F5: Code = 2058 # type: ignore
+MFENCE_F5: int = 2058
 """
 ``MFENCE``
 
 ``NP 0F AE F5``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F6: Code = 2059 # type: ignore
+MFENCE_F6: int = 2059
 """
 ``MFENCE``
 
 ``NP 0F AE F6``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MFENCE_F7: Code = 2060 # type: ignore
+MFENCE_F7: int = 2060
 """
 ``MFENCE``
 
 ``NP 0F AE F7``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-SFENCE: Code = 2061 # type: ignore
+SFENCE: int = 2061
 """
 ``SFENCE``
 
 ``NP 0F AE F8``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_F9: Code = 2062 # type: ignore
+SFENCE_F9: int = 2062
 """
 ``SFENCE``
 
 ``NP 0F AE F9``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FA: Code = 2063 # type: ignore
+SFENCE_FA: int = 2063
 """
 ``SFENCE``
 
 ``NP 0F AE FA``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FB: Code = 2064 # type: ignore
+SFENCE_FB: int = 2064
 """
 ``SFENCE``
 
 ``NP 0F AE FB``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FC: Code = 2065 # type: ignore
+SFENCE_FC: int = 2065
 """
 ``SFENCE``
 
 ``NP 0F AE FC``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FD: Code = 2066 # type: ignore
+SFENCE_FD: int = 2066
 """
 ``SFENCE``
 
 ``NP 0F AE FD``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FE: Code = 2067 # type: ignore
+SFENCE_FE: int = 2067
 """
 ``SFENCE``
 
 ``NP 0F AE FE``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-SFENCE_FF: Code = 2068 # type: ignore
+SFENCE_FF: int = 2068
 """
 ``SFENCE``
 
 ``NP 0F AE FF``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PCOMMIT: Code = 2069 # type: ignore
+PCOMMIT: int = 2069
 """
 ``PCOMMIT``
 
 ``66 0F AE F8``
 
 ``PCOMMIT``
 
 ``16/32/64-bit``
 """
-IMUL_R16_RM16: Code = 2070 # type: ignore
+IMUL_R16_RM16: int = 2070
 """
 ``IMUL r16, r/m16``
 
 ``o16 0F AF /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IMUL_R32_RM32: Code = 2071 # type: ignore
+IMUL_R32_RM32: int = 2071
 """
 ``IMUL r32, r/m32``
 
 ``o32 0F AF /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-IMUL_R64_RM64: Code = 2072 # type: ignore
+IMUL_R64_RM64: int = 2072
 """
 ``IMUL r64, r/m64``
 
 ``o64 0F AF /r``
 
 ``X64``
 
 ``64-bit``
 """
-CMPXCHG_RM8_R8: Code = 2073 # type: ignore
+CMPXCHG_RM8_R8: int = 2073
 """
 ``CMPXCHG r/m8, r8``
 
 ``0F B0 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-CMPXCHG_RM16_R16: Code = 2074 # type: ignore
+CMPXCHG_RM16_R16: int = 2074
 """
 ``CMPXCHG r/m16, r16``
 
 ``o16 0F B1 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-CMPXCHG_RM32_R32: Code = 2075 # type: ignore
+CMPXCHG_RM32_R32: int = 2075
 """
 ``CMPXCHG r/m32, r32``
 
 ``o32 0F B1 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-CMPXCHG_RM64_R64: Code = 2076 # type: ignore
+CMPXCHG_RM64_R64: int = 2076
 """
 ``CMPXCHG r/m64, r64``
 
 ``o64 0F B1 /r``
 
 ``X64``
 
 ``64-bit``
 """
-LSS_R16_M1616: Code = 2077 # type: ignore
+LSS_R16_M1616: int = 2077
 """
 ``LSS r16, m16:16``
 
 ``o16 0F B2 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LSS_R32_M1632: Code = 2078 # type: ignore
+LSS_R32_M1632: int = 2078
 """
 ``LSS r32, m16:32``
 
 ``o32 0F B2 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LSS_R64_M1664: Code = 2079 # type: ignore
+LSS_R64_M1664: int = 2079
 """
 ``LSS r64, m16:64``
 
 ``o64 0F B2 /r``
 
 ``X64``
 
 ``64-bit``
 """
-BTR_RM16_R16: Code = 2080 # type: ignore
+BTR_RM16_R16: int = 2080
 """
 ``BTR r/m16, r16``
 
 ``o16 0F B3 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTR_RM32_R32: Code = 2081 # type: ignore
+BTR_RM32_R32: int = 2081
 """
 ``BTR r/m32, r32``
 
 ``o32 0F B3 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTR_RM64_R64: Code = 2082 # type: ignore
+BTR_RM64_R64: int = 2082
 """
 ``BTR r/m64, r64``
 
 ``o64 0F B3 /r``
 
 ``X64``
 
 ``64-bit``
 """
-LFS_R16_M1616: Code = 2083 # type: ignore
+LFS_R16_M1616: int = 2083
 """
 ``LFS r16, m16:16``
 
 ``o16 0F B4 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LFS_R32_M1632: Code = 2084 # type: ignore
+LFS_R32_M1632: int = 2084
 """
 ``LFS r32, m16:32``
 
 ``o32 0F B4 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LFS_R64_M1664: Code = 2085 # type: ignore
+LFS_R64_M1664: int = 2085
 """
 ``LFS r64, m16:64``
 
 ``o64 0F B4 /r``
 
 ``X64``
 
 ``64-bit``
 """
-LGS_R16_M1616: Code = 2086 # type: ignore
+LGS_R16_M1616: int = 2086
 """
 ``LGS r16, m16:16``
 
 ``o16 0F B5 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LGS_R32_M1632: Code = 2087 # type: ignore
+LGS_R32_M1632: int = 2087
 """
 ``LGS r32, m16:32``
 
 ``o32 0F B5 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-LGS_R64_M1664: Code = 2088 # type: ignore
+LGS_R64_M1664: int = 2088
 """
 ``LGS r64, m16:64``
 
 ``o64 0F B5 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOVZX_R16_RM8: Code = 2089 # type: ignore
+MOVZX_R16_RM8: int = 2089
 """
 ``MOVZX r16, r/m8``
 
 ``o16 0F B6 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVZX_R32_RM8: Code = 2090 # type: ignore
+MOVZX_R32_RM8: int = 2090
 """
 ``MOVZX r32, r/m8``
 
 ``o32 0F B6 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVZX_R64_RM8: Code = 2091 # type: ignore
+MOVZX_R64_RM8: int = 2091
 """
 ``MOVZX r64, r/m8``
 
 ``o64 0F B6 /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOVZX_R16_RM16: Code = 2092 # type: ignore
+MOVZX_R16_RM16: int = 2092
 """
 ``MOVZX r16, r/m16``
 
 ``o16 0F B7 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVZX_R32_RM16: Code = 2093 # type: ignore
+MOVZX_R32_RM16: int = 2093
 """
 ``MOVZX r32, r/m16``
 
 ``o32 0F B7 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVZX_R64_RM16: Code = 2094 # type: ignore
+MOVZX_R64_RM16: int = 2094
 """
 ``MOVZX r64, r/m16``
 
 ``o64 0F B7 /r``
 
 ``X64``
 
 ``64-bit``
 """
-JMPE_DISP16: Code = 2095 # type: ignore
+JMPE_DISP16: int = 2095
 """
 ``JMPE disp16``
 
 ``o16 0F B8 cw``
 
 ``IA-64``
 
 ``16/32-bit``
 """
-JMPE_DISP32: Code = 2096 # type: ignore
+JMPE_DISP32: int = 2096
 """
 ``JMPE disp32``
 
 ``o32 0F B8 cd``
 
 ``IA-64``
 
 ``16/32-bit``
 """
-POPCNT_R16_RM16: Code = 2097 # type: ignore
+POPCNT_R16_RM16: int = 2097
 """
 ``POPCNT r16, r/m16``
 
 ``o16 F3 0F B8 /r``
 
 ``POPCNT``
 
 ``16/32/64-bit``
 """
-POPCNT_R32_RM32: Code = 2098 # type: ignore
+POPCNT_R32_RM32: int = 2098
 """
 ``POPCNT r32, r/m32``
 
 ``o32 F3 0F B8 /r``
 
 ``POPCNT``
 
 ``16/32/64-bit``
 """
-POPCNT_R64_RM64: Code = 2099 # type: ignore
+POPCNT_R64_RM64: int = 2099
 """
 ``POPCNT r64, r/m64``
 
 ``F3 o64 0F B8 /r``
 
 ``POPCNT``
 
 ``64-bit``
 """
-UD1_R16_RM16: Code = 2100 # type: ignore
+UD1_R16_RM16: int = 2100
 """
 ``UD1 r16, r/m16``
 
 ``o16 0F B9 /r``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-UD1_R32_RM32: Code = 2101 # type: ignore
+UD1_R32_RM32: int = 2101
 """
 ``UD1 r32, r/m32``
 
 ``o32 0F B9 /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-UD1_R64_RM64: Code = 2102 # type: ignore
+UD1_R64_RM64: int = 2102
 """
 ``UD1 r64, r/m64``
 
 ``o64 0F B9 /r``
 
 ``X64``
 
 ``64-bit``
 """
-BT_RM16_IMM8: Code = 2103 # type: ignore
+BT_RM16_IMM8: int = 2103
 """
 ``BT r/m16, imm8``
 
 ``o16 0F BA /4 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BT_RM32_IMM8: Code = 2104 # type: ignore
+BT_RM32_IMM8: int = 2104
 """
 ``BT r/m32, imm8``
 
 ``o32 0F BA /4 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BT_RM64_IMM8: Code = 2105 # type: ignore
+BT_RM64_IMM8: int = 2105
 """
 ``BT r/m64, imm8``
 
 ``o64 0F BA /4 ib``
 
 ``X64``
 
 ``64-bit``
 """
-BTS_RM16_IMM8: Code = 2106 # type: ignore
+BTS_RM16_IMM8: int = 2106
 """
 ``BTS r/m16, imm8``
 
 ``o16 0F BA /5 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTS_RM32_IMM8: Code = 2107 # type: ignore
+BTS_RM32_IMM8: int = 2107
 """
 ``BTS r/m32, imm8``
 
 ``o32 0F BA /5 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTS_RM64_IMM8: Code = 2108 # type: ignore
+BTS_RM64_IMM8: int = 2108
 """
 ``BTS r/m64, imm8``
 
 ``o64 0F BA /5 ib``
 
 ``X64``
 
 ``64-bit``
 """
-BTR_RM16_IMM8: Code = 2109 # type: ignore
+BTR_RM16_IMM8: int = 2109
 """
 ``BTR r/m16, imm8``
 
 ``o16 0F BA /6 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTR_RM32_IMM8: Code = 2110 # type: ignore
+BTR_RM32_IMM8: int = 2110
 """
 ``BTR r/m32, imm8``
 
 ``o32 0F BA /6 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTR_RM64_IMM8: Code = 2111 # type: ignore
+BTR_RM64_IMM8: int = 2111
 """
 ``BTR r/m64, imm8``
 
 ``o64 0F BA /6 ib``
 
 ``X64``
 
 ``64-bit``
 """
-BTC_RM16_IMM8: Code = 2112 # type: ignore
+BTC_RM16_IMM8: int = 2112
 """
 ``BTC r/m16, imm8``
 
 ``o16 0F BA /7 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTC_RM32_IMM8: Code = 2113 # type: ignore
+BTC_RM32_IMM8: int = 2113
 """
 ``BTC r/m32, imm8``
 
 ``o32 0F BA /7 ib``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTC_RM64_IMM8: Code = 2114 # type: ignore
+BTC_RM64_IMM8: int = 2114
 """
 ``BTC r/m64, imm8``
 
 ``o64 0F BA /7 ib``
 
 ``X64``
 
 ``64-bit``
 """
-BTC_RM16_R16: Code = 2115 # type: ignore
+BTC_RM16_R16: int = 2115
 """
 ``BTC r/m16, r16``
 
 ``o16 0F BB /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTC_RM32_R32: Code = 2116 # type: ignore
+BTC_RM32_R32: int = 2116
 """
 ``BTC r/m32, r32``
 
 ``o32 0F BB /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BTC_RM64_R64: Code = 2117 # type: ignore
+BTC_RM64_R64: int = 2117
 """
 ``BTC r/m64, r64``
 
 ``o64 0F BB /r``
 
 ``X64``
 
 ``64-bit``
 """
-BSF_R16_RM16: Code = 2118 # type: ignore
+BSF_R16_RM16: int = 2118
 """
 ``BSF r16, r/m16``
 
 ``o16 0F BC /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BSF_R32_RM32: Code = 2119 # type: ignore
+BSF_R32_RM32: int = 2119
 """
 ``BSF r32, r/m32``
 
 ``o32 0F BC /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BSF_R64_RM64: Code = 2120 # type: ignore
+BSF_R64_RM64: int = 2120
 """
 ``BSF r64, r/m64``
 
 ``o64 0F BC /r``
 
 ``X64``
 
 ``64-bit``
 """
-TZCNT_R16_RM16: Code = 2121 # type: ignore
+TZCNT_R16_RM16: int = 2121
 """
 ``TZCNT r16, r/m16``
 
 ``o16 F3 0F BC /r``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-TZCNT_R32_RM32: Code = 2122 # type: ignore
+TZCNT_R32_RM32: int = 2122
 """
 ``TZCNT r32, r/m32``
 
 ``o32 F3 0F BC /r``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-TZCNT_R64_RM64: Code = 2123 # type: ignore
+TZCNT_R64_RM64: int = 2123
 """
 ``TZCNT r64, r/m64``
 
 ``F3 o64 0F BC /r``
 
 ``BMI1``
 
 ``64-bit``
 """
-BSR_R16_RM16: Code = 2124 # type: ignore
+BSR_R16_RM16: int = 2124
 """
 ``BSR r16, r/m16``
 
 ``o16 0F BD /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BSR_R32_RM32: Code = 2125 # type: ignore
+BSR_R32_RM32: int = 2125
 """
 ``BSR r32, r/m32``
 
 ``o32 0F BD /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-BSR_R64_RM64: Code = 2126 # type: ignore
+BSR_R64_RM64: int = 2126
 """
 ``BSR r64, r/m64``
 
 ``o64 0F BD /r``
 
 ``X64``
 
 ``64-bit``
 """
-LZCNT_R16_RM16: Code = 2127 # type: ignore
+LZCNT_R16_RM16: int = 2127
 """
 ``LZCNT r16, r/m16``
 
 ``o16 F3 0F BD /r``
 
 ``LZCNT``
 
 ``16/32/64-bit``
 """
-LZCNT_R32_RM32: Code = 2128 # type: ignore
+LZCNT_R32_RM32: int = 2128
 """
 ``LZCNT r32, r/m32``
 
 ``o32 F3 0F BD /r``
 
 ``LZCNT``
 
 ``16/32/64-bit``
 """
-LZCNT_R64_RM64: Code = 2129 # type: ignore
+LZCNT_R64_RM64: int = 2129
 """
 ``LZCNT r64, r/m64``
 
 ``F3 o64 0F BD /r``
 
 ``LZCNT``
 
 ``64-bit``
 """
-MOVSX_R16_RM8: Code = 2130 # type: ignore
+MOVSX_R16_RM8: int = 2130
 """
 ``MOVSX r16, r/m8``
 
 ``o16 0F BE /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVSX_R32_RM8: Code = 2131 # type: ignore
+MOVSX_R32_RM8: int = 2131
 """
 ``MOVSX r32, r/m8``
 
 ``o32 0F BE /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVSX_R64_RM8: Code = 2132 # type: ignore
+MOVSX_R64_RM8: int = 2132
 """
 ``MOVSX r64, r/m8``
 
 ``o64 0F BE /r``
 
 ``X64``
 
 ``64-bit``
 """
-MOVSX_R16_RM16: Code = 2133 # type: ignore
+MOVSX_R16_RM16: int = 2133
 """
 ``MOVSX r16, r/m16``
 
 ``o16 0F BF /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVSX_R32_RM16: Code = 2134 # type: ignore
+MOVSX_R32_RM16: int = 2134
 """
 ``MOVSX r32, r/m16``
 
 ``o32 0F BF /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-MOVSX_R64_RM16: Code = 2135 # type: ignore
+MOVSX_R64_RM16: int = 2135
 """
 ``MOVSX r64, r/m16``
 
 ``o64 0F BF /r``
 
 ``X64``
 
 ``64-bit``
 """
-XADD_RM8_R8: Code = 2136 # type: ignore
+XADD_RM8_R8: int = 2136
 """
 ``XADD r/m8, r8``
 
 ``0F C0 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-XADD_RM16_R16: Code = 2137 # type: ignore
+XADD_RM16_R16: int = 2137
 """
 ``XADD r/m16, r16``
 
 ``o16 0F C1 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-XADD_RM32_R32: Code = 2138 # type: ignore
+XADD_RM32_R32: int = 2138
 """
 ``XADD r/m32, r32``
 
 ``o32 0F C1 /r``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-XADD_RM64_R64: Code = 2139 # type: ignore
+XADD_RM64_R64: int = 2139
 """
 ``XADD r/m64, r64``
 
 ``o64 0F C1 /r``
 
 ``X64``
 
 ``64-bit``
 """
-CMPPS_XMM_XMMM128_IMM8: Code = 2140 # type: ignore
+CMPPS_XMM_XMMM128_IMM8: int = 2140
 """
 ``CMPPS xmm1, xmm2/m128, imm8``
 
 ``NP 0F C2 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VCMPPS_XMM_XMM_XMMM128_IMM8: Code = 2141 # type: ignore
+VEX_VCMPPS_XMM_XMM_XMMM128_IMM8: int = 2141
 """
 ``VCMPPS xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCMPPS_YMM_YMM_YMMM256_IMM8: Code = 2142 # type: ignore
+VEX_VCMPPS_YMM_YMM_YMMM256_IMM8: int = 2142
 """
 ``VCMPPS ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPS_KR_K1_XMM_XMMM128B32_IMM8: Code = 2143 # type: ignore
+EVEX_VCMPPS_KR_K1_XMM_XMMM128B32_IMM8: int = 2143
 """
 ``VCMPPS k1 {k2}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.0F.W0 C2 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPS_KR_K1_YMM_YMMM256B32_IMM8: Code = 2144 # type: ignore
+EVEX_VCMPPS_KR_K1_YMM_YMMM256B32_IMM8: int = 2144
 """
 ``VCMPPS k1 {k2}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.0F.W0 C2 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPS_KR_K1_ZMM_ZMMM512B32_IMM8_SAE: Code = 2145 # type: ignore
+EVEX_VCMPPS_KR_K1_ZMM_ZMMM512B32_IMM8_SAE: int = 2145
 """
 ``VCMPPS k1 {k2}, zmm2, zmm3/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.0F.W0 C2 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CMPPD_XMM_XMMM128_IMM8: Code = 2146 # type: ignore
+CMPPD_XMM_XMMM128_IMM8: int = 2146
 """
 ``CMPPD xmm1, xmm2/m128, imm8``
 
 ``66 0F C2 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCMPPD_XMM_XMM_XMMM128_IMM8: Code = 2147 # type: ignore
+VEX_VCMPPD_XMM_XMM_XMMM128_IMM8: int = 2147
 """
 ``VCMPPD xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCMPPD_YMM_YMM_YMMM256_IMM8: Code = 2148 # type: ignore
+VEX_VCMPPD_YMM_YMM_YMMM256_IMM8: int = 2148
 """
 ``VCMPPD ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPD_KR_K1_XMM_XMMM128B64_IMM8: Code = 2149 # type: ignore
+EVEX_VCMPPD_KR_K1_XMM_XMMM128B64_IMM8: int = 2149
 """
 ``VCMPPD k1 {k2}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 C2 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPD_KR_K1_YMM_YMMM256B64_IMM8: Code = 2150 # type: ignore
+EVEX_VCMPPD_KR_K1_YMM_YMMM256B64_IMM8: int = 2150
 """
 ``VCMPPD k1 {k2}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 C2 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPPD_KR_K1_ZMM_ZMMM512B64_IMM8_SAE: Code = 2151 # type: ignore
+EVEX_VCMPPD_KR_K1_ZMM_ZMMM512B64_IMM8_SAE: int = 2151
 """
 ``VCMPPD k1 {k2}, zmm2, zmm3/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F.W1 C2 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CMPSS_XMM_XMMM32_IMM8: Code = 2152 # type: ignore
+CMPSS_XMM_XMMM32_IMM8: int = 2152
 """
 ``CMPSS xmm1, xmm2/m32, imm8``
 
 ``F3 0F C2 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VCMPSS_XMM_XMM_XMMM32_IMM8: Code = 2153 # type: ignore
+VEX_VCMPSS_XMM_XMM_XMMM32_IMM8: int = 2153
 """
 ``VCMPSS xmm1, xmm2, xmm3/m32, imm8``
 
 ``VEX.LIG.F3.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPSS_KR_K1_XMM_XMMM32_IMM8_SAE: Code = 2154 # type: ignore
+EVEX_VCMPSS_KR_K1_XMM_XMMM32_IMM8_SAE: int = 2154
 """
 ``VCMPSS k1 {k2}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.F3.0F.W0 C2 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CMPSD_XMM_XMMM64_IMM8: Code = 2155 # type: ignore
+CMPSD_XMM_XMMM64_IMM8: int = 2155
 """
 ``CMPSD xmm1, xmm2/m64, imm8``
 
 ``F2 0F C2 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCMPSD_XMM_XMM_XMMM64_IMM8: Code = 2156 # type: ignore
+VEX_VCMPSD_XMM_XMM_XMMM64_IMM8: int = 2156
 """
 ``VCMPSD xmm1, xmm2, xmm3/m64, imm8``
 
 ``VEX.LIG.F2.0F.WIG C2 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCMPSD_KR_K1_XMM_XMMM64_IMM8_SAE: Code = 2157 # type: ignore
+EVEX_VCMPSD_KR_K1_XMM_XMMM64_IMM8_SAE: int = 2157
 """
 ``VCMPSD k1 {k2}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.F2.0F.W1 C2 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVNTI_M32_R32: Code = 2158 # type: ignore
+MOVNTI_M32_R32: int = 2158
 """
 ``MOVNTI m32, r32``
 
 ``NP 0F C3 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MOVNTI_M64_R64: Code = 2159 # type: ignore
+MOVNTI_M64_R64: int = 2159
 """
 ``MOVNTI m64, r64``
 
 ``NP o64 0F C3 /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-PINSRW_MM_R32M16_IMM8: Code = 2160 # type: ignore
+PINSRW_MM_R32M16_IMM8: int = 2160
 """
 ``PINSRW mm, r32/m16, imm8``
 
 ``NP 0F C4 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PINSRW_MM_R64M16_IMM8: Code = 2161 # type: ignore
+PINSRW_MM_R64M16_IMM8: int = 2161
 """
 ``PINSRW mm, r64/m16, imm8``
 
 ``NP o64 0F C4 /r ib``
 
 ``SSE``
 
 ``64-bit``
 """
-PINSRW_XMM_R32M16_IMM8: Code = 2162 # type: ignore
+PINSRW_XMM_R32M16_IMM8: int = 2162
 """
 ``PINSRW xmm, r32/m16, imm8``
 
 ``66 0F C4 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PINSRW_XMM_R64M16_IMM8: Code = 2163 # type: ignore
+PINSRW_XMM_R64M16_IMM8: int = 2163
 """
 ``PINSRW xmm, r64/m16, imm8``
 
 ``66 o64 0F C4 /r ib``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VPINSRW_XMM_XMM_R32M16_IMM8: Code = 2164 # type: ignore
+VEX_VPINSRW_XMM_XMM_R32M16_IMM8: int = 2164
 """
 ``VPINSRW xmm1, xmm2, r32/m16, imm8``
 
 ``VEX.128.66.0F.W0 C4 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPINSRW_XMM_XMM_R64M16_IMM8: Code = 2165 # type: ignore
+VEX_VPINSRW_XMM_XMM_R64M16_IMM8: int = 2165
 """
 ``VPINSRW xmm1, xmm2, r64/m16, imm8``
 
 ``VEX.128.66.0F.W1 C4 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPINSRW_XMM_XMM_R32M16_IMM8: Code = 2166 # type: ignore
+EVEX_VPINSRW_XMM_XMM_R32M16_IMM8: int = 2166
 """
 ``VPINSRW xmm1, xmm2, r32/m16, imm8``
 
 ``EVEX.128.66.0F.W0 C4 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPINSRW_XMM_XMM_R64M16_IMM8: Code = 2167 # type: ignore
+EVEX_VPINSRW_XMM_XMM_R64M16_IMM8: int = 2167
 """
 ``VPINSRW xmm1, xmm2, r64/m16, imm8``
 
 ``EVEX.128.66.0F.W1 C4 /r ib``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-PEXTRW_R32_MM_IMM8: Code = 2168 # type: ignore
+PEXTRW_R32_MM_IMM8: int = 2168
 """
 ``PEXTRW r32, mm, imm8``
 
 ``NP 0F C5 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PEXTRW_R64_MM_IMM8: Code = 2169 # type: ignore
+PEXTRW_R64_MM_IMM8: int = 2169
 """
 ``PEXTRW r64, mm, imm8``
 
 ``NP o64 0F C5 /r ib``
 
 ``SSE``
 
 ``64-bit``
 """
-PEXTRW_R32_XMM_IMM8: Code = 2170 # type: ignore
+PEXTRW_R32_XMM_IMM8: int = 2170
 """
 ``PEXTRW r32, xmm, imm8``
 
 ``66 0F C5 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PEXTRW_R64_XMM_IMM8: Code = 2171 # type: ignore
+PEXTRW_R64_XMM_IMM8: int = 2171
 """
 ``PEXTRW r64, xmm, imm8``
 
 ``66 o64 0F C5 /r ib``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VPEXTRW_R32_XMM_IMM8: Code = 2172 # type: ignore
+VEX_VPEXTRW_R32_XMM_IMM8: int = 2172
 """
 ``VPEXTRW r32, xmm1, imm8``
 
 ``VEX.128.66.0F.W0 C5 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPEXTRW_R64_XMM_IMM8: Code = 2173 # type: ignore
+VEX_VPEXTRW_R64_XMM_IMM8: int = 2173
 """
 ``VPEXTRW r64, xmm1, imm8``
 
 ``VEX.128.66.0F.W1 C5 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPEXTRW_R32_XMM_IMM8: Code = 2174 # type: ignore
+EVEX_VPEXTRW_R32_XMM_IMM8: int = 2174
 """
 ``VPEXTRW r32, xmm1, imm8``
 
 ``EVEX.128.66.0F.W0 C5 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXTRW_R64_XMM_IMM8: Code = 2175 # type: ignore
+EVEX_VPEXTRW_R64_XMM_IMM8: int = 2175
 """
 ``VPEXTRW r64, xmm1, imm8``
 
 ``EVEX.128.66.0F.W1 C5 /r ib``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-SHUFPS_XMM_XMMM128_IMM8: Code = 2176 # type: ignore
+SHUFPS_XMM_XMMM128_IMM8: int = 2176
 """
 ``SHUFPS xmm1, xmm2/m128, imm8``
 
 ``NP 0F C6 /r ib``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-VEX_VSHUFPS_XMM_XMM_XMMM128_IMM8: Code = 2177 # type: ignore
+VEX_VSHUFPS_XMM_XMM_XMMM128_IMM8: int = 2177
 """
 ``VSHUFPS xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.0F.WIG C6 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSHUFPS_YMM_YMM_YMMM256_IMM8: Code = 2178 # type: ignore
+VEX_VSHUFPS_YMM_YMM_YMMM256_IMM8: int = 2178
 """
 ``VSHUFPS ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.0F.WIG C6 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPS_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 2179 # type: ignore
+EVEX_VSHUFPS_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 2179
 """
 ``VSHUFPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.0F.W0 C6 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPS_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 2180 # type: ignore
+EVEX_VSHUFPS_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 2180
 """
 ``VSHUFPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.0F.W0 C6 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 2181 # type: ignore
+EVEX_VSHUFPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 2181
 """
 ``VSHUFPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.0F.W0 C6 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-SHUFPD_XMM_XMMM128_IMM8: Code = 2182 # type: ignore
+SHUFPD_XMM_XMMM128_IMM8: int = 2182
 """
 ``SHUFPD xmm1, xmm2/m128, imm8``
 
 ``66 0F C6 /r ib``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VSHUFPD_XMM_XMM_XMMM128_IMM8: Code = 2183 # type: ignore
+VEX_VSHUFPD_XMM_XMM_XMMM128_IMM8: int = 2183
 """
 ``VSHUFPD xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F.WIG C6 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VSHUFPD_YMM_YMM_YMMM256_IMM8: Code = 2184 # type: ignore
+VEX_VSHUFPD_YMM_YMM_YMMM256_IMM8: int = 2184
 """
 ``VSHUFPD ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F.WIG C6 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPD_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 2185 # type: ignore
+EVEX_VSHUFPD_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 2185
 """
 ``VSHUFPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F.W1 C6 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPD_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 2186 # type: ignore
+EVEX_VSHUFPD_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 2186
 """
 ``VSHUFPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F.W1 C6 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 2187 # type: ignore
+EVEX_VSHUFPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 2187
 """
 ``VSHUFPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F.W1 C6 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CMPXCHG8B_M64: Code = 2188 # type: ignore
+CMPXCHG8B_M64: int = 2188
 """
 ``CMPXCHG8B m64``
 
 ``0F C7 /1``
 
 ``CX8``
 
 ``16/32/64-bit``
 """
-CMPXCHG16B_M128: Code = 2189 # type: ignore
+CMPXCHG16B_M128: int = 2189
 """
 ``CMPXCHG16B m128``
 
 ``o64 0F C7 /1``
 
 ``CMPXCHG16B``
 
 ``64-bit``
 """
-XRSTORS_MEM: Code = 2190 # type: ignore
+XRSTORS_MEM: int = 2190
 """
 ``XRSTORS mem``
 
 ``NP 0F C7 /3``
 
 ``XSAVES``
 
 ``16/32/64-bit``
 """
-XRSTORS64_MEM: Code = 2191 # type: ignore
+XRSTORS64_MEM: int = 2191
 """
 ``XRSTORS64 mem``
 
 ``NP o64 0F C7 /3``
 
 ``XSAVES``
 
 ``64-bit``
 """
-XSAVEC_MEM: Code = 2192 # type: ignore
+XSAVEC_MEM: int = 2192
 """
 ``XSAVEC mem``
 
 ``NP 0F C7 /4``
 
 ``XSAVEC``
 
 ``16/32/64-bit``
 """
-XSAVEC64_MEM: Code = 2193 # type: ignore
+XSAVEC64_MEM: int = 2193
 """
 ``XSAVEC64 mem``
 
 ``NP o64 0F C7 /4``
 
 ``XSAVEC``
 
 ``64-bit``
 """
-XSAVES_MEM: Code = 2194 # type: ignore
+XSAVES_MEM: int = 2194
 """
 ``XSAVES mem``
 
 ``NP 0F C7 /5``
 
 ``XSAVES``
 
 ``16/32/64-bit``
 """
-XSAVES64_MEM: Code = 2195 # type: ignore
+XSAVES64_MEM: int = 2195
 """
 ``XSAVES64 mem``
 
 ``NP o64 0F C7 /5``
 
 ``XSAVES``
 
 ``64-bit``
 """
-VMPTRLD_M64: Code = 2196 # type: ignore
+VMPTRLD_M64: int = 2196
 """
 ``VMPTRLD m64``
 
 ``NP 0F C7 /6``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-VMCLEAR_M64: Code = 2197 # type: ignore
+VMCLEAR_M64: int = 2197
 """
 ``VMCLEAR m64``
 
 ``66 0F C7 /6``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-VMXON_M64: Code = 2198 # type: ignore
+VMXON_M64: int = 2198
 """
 ``VMXON m64``
 
 ``F3 0F C7 /6``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-RDRAND_R16: Code = 2199 # type: ignore
+RDRAND_R16: int = 2199
 """
 ``RDRAND r16``
 
 ``o16 0F C7 /6``
 
 ``RDRAND``
 
 ``16/32/64-bit``
 """
-RDRAND_R32: Code = 2200 # type: ignore
+RDRAND_R32: int = 2200
 """
 ``RDRAND r32``
 
 ``o32 0F C7 /6``
 
 ``RDRAND``
 
 ``16/32/64-bit``
 """
-RDRAND_R64: Code = 2201 # type: ignore
+RDRAND_R64: int = 2201
 """
 ``RDRAND r64``
 
 ``o64 0F C7 /6``
 
 ``RDRAND``
 
 ``64-bit``
 """
-VMPTRST_M64: Code = 2202 # type: ignore
+VMPTRST_M64: int = 2202
 """
 ``VMPTRST m64``
 
 ``NP 0F C7 /7``
 
 ``VMX``
 
 ``16/32/64-bit``
 """
-RDSEED_R16: Code = 2203 # type: ignore
+RDSEED_R16: int = 2203
 """
 ``RDSEED r16``
 
 ``o16 0F C7 /7``
 
 ``RDSEED``
 
 ``16/32/64-bit``
 """
-RDSEED_R32: Code = 2204 # type: ignore
+RDSEED_R32: int = 2204
 """
 ``RDSEED r32``
 
 ``o32 0F C7 /7``
 
 ``RDSEED``
 
 ``16/32/64-bit``
 """
-RDSEED_R64: Code = 2205 # type: ignore
+RDSEED_R64: int = 2205
 """
 ``RDSEED r64``
 
 ``o64 0F C7 /7``
 
 ``RDSEED``
 
 ``64-bit``
 """
-RDPID_R32: Code = 2206 # type: ignore
+RDPID_R32: int = 2206
 """
 ``RDPID r32``
 
 ``F3 0F C7 /7``
 
 ``RDPID``
 
 ``16/32-bit``
 """
-RDPID_R64: Code = 2207 # type: ignore
+RDPID_R64: int = 2207
 """
 ``RDPID r64``
 
 ``F3 0F C7 /7``
 
 ``RDPID``
 
 ``64-bit``
 """
-BSWAP_R16: Code = 2208 # type: ignore
+BSWAP_R16: int = 2208
 """
 ``BSWAP r16``
 
 ``o16 0F C8+rw``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-BSWAP_R32: Code = 2209 # type: ignore
+BSWAP_R32: int = 2209
 """
 ``BSWAP r32``
 
 ``o32 0F C8+rd``
 
 ``486+``
 
 ``16/32/64-bit``
 """
-BSWAP_R64: Code = 2210 # type: ignore
+BSWAP_R64: int = 2210
 """
 ``BSWAP r64``
 
 ``o64 0F C8+ro``
 
 ``X64``
 
 ``64-bit``
 """
-ADDSUBPD_XMM_XMMM128: Code = 2211 # type: ignore
+ADDSUBPD_XMM_XMMM128: int = 2211
 """
 ``ADDSUBPD xmm1, xmm2/m128``
 
 ``66 0F D0 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VADDSUBPD_XMM_XMM_XMMM128: Code = 2212 # type: ignore
+VEX_VADDSUBPD_XMM_XMM_XMMM128: int = 2212
 """
 ``VADDSUBPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VADDSUBPD_YMM_YMM_YMMM256: Code = 2213 # type: ignore
+VEX_VADDSUBPD_YMM_YMM_YMMM256: int = 2213
 """
 ``VADDSUBPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG D0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-ADDSUBPS_XMM_XMMM128: Code = 2214 # type: ignore
+ADDSUBPS_XMM_XMMM128: int = 2214
 """
 ``ADDSUBPS xmm1, xmm2/m128``
 
 ``F2 0F D0 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VADDSUBPS_XMM_XMM_XMMM128: Code = 2215 # type: ignore
+VEX_VADDSUBPS_XMM_XMM_XMMM128: int = 2215
 """
 ``VADDSUBPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.F2.0F.WIG D0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VADDSUBPS_YMM_YMM_YMMM256: Code = 2216 # type: ignore
+VEX_VADDSUBPS_YMM_YMM_YMMM256: int = 2216
 """
 ``VADDSUBPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.F2.0F.WIG D0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PSRLW_MM_MMM64: Code = 2217 # type: ignore
+PSRLW_MM_MMM64: int = 2217
 """
 ``PSRLW mm, mm/m64``
 
 ``NP 0F D1 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLW_XMM_XMMM128: Code = 2218 # type: ignore
+PSRLW_XMM_XMMM128: int = 2218
 """
 ``PSRLW xmm1, xmm2/m128``
 
 ``66 0F D1 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLW_XMM_XMM_XMMM128: Code = 2219 # type: ignore
+VEX_VPSRLW_XMM_XMM_XMMM128: int = 2219
 """
 ``VPSRLW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D1 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLW_YMM_YMM_XMMM128: Code = 2220 # type: ignore
+VEX_VPSRLW_YMM_YMM_XMMM128: int = 2220
 """
 ``VPSRLW ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG D1 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_XMM_K1Z_XMM_XMMM128: Code = 2221 # type: ignore
+EVEX_VPSRLW_XMM_K1Z_XMM_XMMM128: int = 2221
 """
 ``VPSRLW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG D1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_YMM_K1Z_YMM_XMMM128: Code = 2222 # type: ignore
+EVEX_VPSRLW_YMM_K1Z_YMM_XMMM128: int = 2222
 """
 ``VPSRLW ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.WIG D1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLW_ZMM_K1Z_ZMM_XMMM128: Code = 2223 # type: ignore
+EVEX_VPSRLW_ZMM_K1Z_ZMM_XMMM128: int = 2223
 """
 ``VPSRLW zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.WIG D1 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSRLD_MM_MMM64: Code = 2224 # type: ignore
+PSRLD_MM_MMM64: int = 2224
 """
 ``PSRLD mm, mm/m64``
 
 ``NP 0F D2 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLD_XMM_XMMM128: Code = 2225 # type: ignore
+PSRLD_XMM_XMMM128: int = 2225
 """
 ``PSRLD xmm1, xmm2/m128``
 
 ``66 0F D2 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLD_XMM_XMM_XMMM128: Code = 2226 # type: ignore
+VEX_VPSRLD_XMM_XMM_XMMM128: int = 2226
 """
 ``VPSRLD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D2 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLD_YMM_YMM_XMMM128: Code = 2227 # type: ignore
+VEX_VPSRLD_YMM_YMM_XMMM128: int = 2227
 """
 ``VPSRLD ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG D2 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_XMM_K1Z_XMM_XMMM128: Code = 2228 # type: ignore
+EVEX_VPSRLD_XMM_K1Z_XMM_XMMM128: int = 2228
 """
 ``VPSRLD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W0 D2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_YMM_K1Z_YMM_XMMM128: Code = 2229 # type: ignore
+EVEX_VPSRLD_YMM_K1Z_YMM_XMMM128: int = 2229
 """
 ``VPSRLD ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W0 D2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLD_ZMM_K1Z_ZMM_XMMM128: Code = 2230 # type: ignore
+EVEX_VPSRLD_ZMM_K1Z_ZMM_XMMM128: int = 2230
 """
 ``VPSRLD zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W0 D2 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSRLQ_MM_MMM64: Code = 2231 # type: ignore
+PSRLQ_MM_MMM64: int = 2231
 """
 ``PSRLQ mm, mm/m64``
 
 ``NP 0F D3 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRLQ_XMM_XMMM128: Code = 2232 # type: ignore
+PSRLQ_XMM_XMMM128: int = 2232
 """
 ``PSRLQ xmm1, xmm2/m128``
 
 ``66 0F D3 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLQ_XMM_XMM_XMMM128: Code = 2233 # type: ignore
+VEX_VPSRLQ_XMM_XMM_XMMM128: int = 2233
 """
 ``VPSRLQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D3 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLQ_YMM_YMM_XMMM128: Code = 2234 # type: ignore
+VEX_VPSRLQ_YMM_YMM_XMMM128: int = 2234
 """
 ``VPSRLQ ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG D3 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_XMM_K1Z_XMM_XMMM128: Code = 2235 # type: ignore
+EVEX_VPSRLQ_XMM_K1Z_XMM_XMMM128: int = 2235
 """
 ``VPSRLQ xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W1 D3 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_YMM_K1Z_YMM_XMMM128: Code = 2236 # type: ignore
+EVEX_VPSRLQ_YMM_K1Z_YMM_XMMM128: int = 2236
 """
 ``VPSRLQ ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W1 D3 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLQ_ZMM_K1Z_ZMM_XMMM128: Code = 2237 # type: ignore
+EVEX_VPSRLQ_ZMM_K1Z_ZMM_XMMM128: int = 2237
 """
 ``VPSRLQ zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W1 D3 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PADDQ_MM_MMM64: Code = 2238 # type: ignore
+PADDQ_MM_MMM64: int = 2238
 """
 ``PADDQ mm, mm/m64``
 
 ``NP 0F D4 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDQ_XMM_XMMM128: Code = 2239 # type: ignore
+PADDQ_XMM_XMMM128: int = 2239
 """
 ``PADDQ xmm1, xmm2/m128``
 
 ``66 0F D4 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDQ_XMM_XMM_XMMM128: Code = 2240 # type: ignore
+VEX_VPADDQ_XMM_XMM_XMMM128: int = 2240
 """
 ``VPADDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D4 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDQ_YMM_YMM_YMMM256: Code = 2241 # type: ignore
+VEX_VPADDQ_YMM_YMM_YMMM256: int = 2241
 """
 ``VPADDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG D4 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDQ_XMM_K1Z_XMM_XMMM128B64: Code = 2242 # type: ignore
+EVEX_VPADDQ_XMM_K1Z_XMM_XMMM128B64: int = 2242
 """
 ``VPADDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 D4 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDQ_YMM_K1Z_YMM_YMMM256B64: Code = 2243 # type: ignore
+EVEX_VPADDQ_YMM_K1Z_YMM_YMMM256B64: int = 2243
 """
 ``VPADDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 D4 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2244 # type: ignore
+EVEX_VPADDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2244
 """
 ``VPADDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 D4 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMULLW_MM_MMM64: Code = 2245 # type: ignore
+PMULLW_MM_MMM64: int = 2245
 """
 ``PMULLW mm, mm/m64``
 
 ``NP 0F D5 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PMULLW_XMM_XMMM128: Code = 2246 # type: ignore
+PMULLW_XMM_XMMM128: int = 2246
 """
 ``PMULLW xmm1, xmm2/m128``
 
 ``66 0F D5 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMULLW_XMM_XMM_XMMM128: Code = 2247 # type: ignore
+VEX_VPMULLW_XMM_XMM_XMMM128: int = 2247
 """
 ``VPMULLW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D5 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULLW_YMM_YMM_YMMM256: Code = 2248 # type: ignore
+VEX_VPMULLW_YMM_YMM_YMMM256: int = 2248
 """
 ``VPMULLW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG D5 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLW_XMM_K1Z_XMM_XMMM128: Code = 2249 # type: ignore
+EVEX_VPMULLW_XMM_K1Z_XMM_XMMM128: int = 2249
 """
 ``VPMULLW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG D5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLW_YMM_K1Z_YMM_YMMM256: Code = 2250 # type: ignore
+EVEX_VPMULLW_YMM_K1Z_YMM_YMMM256: int = 2250
 """
 ``VPMULLW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG D5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLW_ZMM_K1Z_ZMM_ZMMM512: Code = 2251 # type: ignore
+EVEX_VPMULLW_ZMM_K1Z_ZMM_ZMMM512: int = 2251
 """
 ``VPMULLW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG D5 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-MOVQ_XMMM64_XMM: Code = 2252 # type: ignore
+MOVQ_XMMM64_XMM: int = 2252
 """
 ``MOVQ xmm2/m64, xmm1``
 
 ``66 0F D6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVQ_XMMM64_XMM: Code = 2253 # type: ignore
+VEX_VMOVQ_XMMM64_XMM: int = 2253
 """
 ``VMOVQ xmm1/m64, xmm2``
 
 ``VEX.128.66.0F.WIG D6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVQ_XMMM64_XMM: Code = 2254 # type: ignore
+EVEX_VMOVQ_XMMM64_XMM: int = 2254
 """
 ``VMOVQ xmm1/m64, xmm2``
 
 ``EVEX.128.66.0F.W1 D6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVQ2DQ_XMM_MM: Code = 2255 # type: ignore
+MOVQ2DQ_XMM_MM: int = 2255
 """
 ``MOVQ2DQ xmm, mm``
 
 ``F3 0F D6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-MOVDQ2Q_MM_XMM: Code = 2256 # type: ignore
+MOVDQ2Q_MM_XMM: int = 2256
 """
 ``MOVDQ2Q mm, xmm``
 
 ``F2 0F D6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PMOVMSKB_R32_MM: Code = 2257 # type: ignore
+PMOVMSKB_R32_MM: int = 2257
 """
 ``PMOVMSKB r32, mm``
 
 ``NP 0F D7 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMOVMSKB_R64_MM: Code = 2258 # type: ignore
+PMOVMSKB_R64_MM: int = 2258
 """
 ``PMOVMSKB r64, mm``
 
 ``NP o64 0F D7 /r``
 
 ``SSE``
 
 ``64-bit``
 """
-PMOVMSKB_R32_XMM: Code = 2259 # type: ignore
+PMOVMSKB_R32_XMM: int = 2259
 """
 ``PMOVMSKB r32, xmm``
 
 ``66 0F D7 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PMOVMSKB_R64_XMM: Code = 2260 # type: ignore
+PMOVMSKB_R64_XMM: int = 2260
 """
 ``PMOVMSKB r64, xmm``
 
 ``66 o64 0F D7 /r``
 
 ``SSE2``
 
 ``64-bit``
 """
-VEX_VPMOVMSKB_R32_XMM: Code = 2261 # type: ignore
+VEX_VPMOVMSKB_R32_XMM: int = 2261
 """
 ``VPMOVMSKB r32, xmm1``
 
 ``VEX.128.66.0F.W0 D7 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVMSKB_R64_XMM: Code = 2262 # type: ignore
+VEX_VPMOVMSKB_R64_XMM: int = 2262
 """
 ``VPMOVMSKB r64, xmm1``
 
 ``VEX.128.66.0F.W1 D7 /r``
 
 ``AVX``
 
 ``64-bit``
 """
-VEX_VPMOVMSKB_R32_YMM: Code = 2263 # type: ignore
+VEX_VPMOVMSKB_R32_YMM: int = 2263
 """
 ``VPMOVMSKB r32, ymm1``
 
 ``VEX.256.66.0F.W0 D7 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVMSKB_R64_YMM: Code = 2264 # type: ignore
+VEX_VPMOVMSKB_R64_YMM: int = 2264
 """
 ``VPMOVMSKB r64, ymm1``
 
 ``VEX.256.66.0F.W1 D7 /r``
 
 ``AVX2``
 
 ``64-bit``
 """
-PSUBUSB_MM_MMM64: Code = 2265 # type: ignore
+PSUBUSB_MM_MMM64: int = 2265
 """
 ``PSUBUSB mm, mm/m64``
 
 ``NP 0F D8 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBUSB_XMM_XMMM128: Code = 2266 # type: ignore
+PSUBUSB_XMM_XMMM128: int = 2266
 """
 ``PSUBUSB xmm1, xmm2/m128``
 
 ``66 0F D8 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBUSB_XMM_XMM_XMMM128: Code = 2267 # type: ignore
+VEX_VPSUBUSB_XMM_XMM_XMMM128: int = 2267
 """
 ``VPSUBUSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D8 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBUSB_YMM_YMM_YMMM256: Code = 2268 # type: ignore
+VEX_VPSUBUSB_YMM_YMM_YMMM256: int = 2268
 """
 ``VPSUBUSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG D8 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSB_XMM_K1Z_XMM_XMMM128: Code = 2269 # type: ignore
+EVEX_VPSUBUSB_XMM_K1Z_XMM_XMMM128: int = 2269
 """
 ``VPSUBUSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG D8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSB_YMM_K1Z_YMM_YMMM256: Code = 2270 # type: ignore
+EVEX_VPSUBUSB_YMM_K1Z_YMM_YMMM256: int = 2270
 """
 ``VPSUBUSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG D8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2271 # type: ignore
+EVEX_VPSUBUSB_ZMM_K1Z_ZMM_ZMMM512: int = 2271
 """
 ``VPSUBUSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG D8 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSUBUSW_MM_MMM64: Code = 2272 # type: ignore
+PSUBUSW_MM_MMM64: int = 2272
 """
 ``PSUBUSW mm, mm/m64``
 
 ``NP 0F D9 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBUSW_XMM_XMMM128: Code = 2273 # type: ignore
+PSUBUSW_XMM_XMMM128: int = 2273
 """
 ``PSUBUSW xmm1, xmm2/m128``
 
 ``66 0F D9 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBUSW_XMM_XMM_XMMM128: Code = 2274 # type: ignore
+VEX_VPSUBUSW_XMM_XMM_XMMM128: int = 2274
 """
 ``VPSUBUSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG D9 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBUSW_YMM_YMM_YMMM256: Code = 2275 # type: ignore
+VEX_VPSUBUSW_YMM_YMM_YMMM256: int = 2275
 """
 ``VPSUBUSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG D9 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSW_XMM_K1Z_XMM_XMMM128: Code = 2276 # type: ignore
+EVEX_VPSUBUSW_XMM_K1Z_XMM_XMMM128: int = 2276
 """
 ``VPSUBUSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG D9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSW_YMM_K1Z_YMM_YMMM256: Code = 2277 # type: ignore
+EVEX_VPSUBUSW_YMM_K1Z_YMM_YMMM256: int = 2277
 """
 ``VPSUBUSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG D9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBUSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2278 # type: ignore
+EVEX_VPSUBUSW_ZMM_K1Z_ZMM_ZMMM512: int = 2278
 """
 ``VPSUBUSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG D9 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMINUB_MM_MMM64: Code = 2279 # type: ignore
+PMINUB_MM_MMM64: int = 2279
 """
 ``PMINUB mm1, mm2/m64``
 
 ``NP 0F DA /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMINUB_XMM_XMMM128: Code = 2280 # type: ignore
+PMINUB_XMM_XMMM128: int = 2280
 """
 ``PMINUB xmm1, xmm2/m128``
 
 ``66 0F DA /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUB_XMM_XMM_XMMM128: Code = 2281 # type: ignore
+VEX_VPMINUB_XMM_XMM_XMMM128: int = 2281
 """
 ``VPMINUB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DA /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUB_YMM_YMM_YMMM256: Code = 2282 # type: ignore
+VEX_VPMINUB_YMM_YMM_YMMM256: int = 2282
 """
 ``VPMINUB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DA /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUB_XMM_K1Z_XMM_XMMM128: Code = 2283 # type: ignore
+EVEX_VPMINUB_XMM_K1Z_XMM_XMMM128: int = 2283
 """
 ``VPMINUB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG DA /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUB_YMM_K1Z_YMM_YMMM256: Code = 2284 # type: ignore
+EVEX_VPMINUB_YMM_K1Z_YMM_YMMM256: int = 2284
 """
 ``VPMINUB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG DA /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUB_ZMM_K1Z_ZMM_ZMMM512: Code = 2285 # type: ignore
+EVEX_VPMINUB_ZMM_K1Z_ZMM_ZMMM512: int = 2285
 """
 ``VPMINUB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG DA /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PAND_MM_MMM64: Code = 2286 # type: ignore
+PAND_MM_MMM64: int = 2286
 """
 ``PAND mm, mm/m64``
 
 ``NP 0F DB /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PAND_XMM_XMMM128: Code = 2287 # type: ignore
+PAND_XMM_XMMM128: int = 2287
 """
 ``PAND xmm1, xmm2/m128``
 
 ``66 0F DB /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPAND_XMM_XMM_XMMM128: Code = 2288 # type: ignore
+VEX_VPAND_XMM_XMM_XMMM128: int = 2288
 """
 ``VPAND xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DB /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPAND_YMM_YMM_YMMM256: Code = 2289 # type: ignore
+VEX_VPAND_YMM_YMM_YMMM256: int = 2289
 """
 ``VPAND ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DB /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDD_XMM_K1Z_XMM_XMMM128B32: Code = 2290 # type: ignore
+EVEX_VPANDD_XMM_K1Z_XMM_XMMM128B32: int = 2290
 """
 ``VPANDD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 DB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDD_YMM_K1Z_YMM_YMMM256B32: Code = 2291 # type: ignore
+EVEX_VPANDD_YMM_K1Z_YMM_YMMM256B32: int = 2291
 """
 ``VPANDD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 DB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2292 # type: ignore
+EVEX_VPANDD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2292
 """
 ``VPANDD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 DB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDQ_XMM_K1Z_XMM_XMMM128B64: Code = 2293 # type: ignore
+EVEX_VPANDQ_XMM_K1Z_XMM_XMMM128B64: int = 2293
 """
 ``VPANDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 DB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDQ_YMM_K1Z_YMM_YMMM256B64: Code = 2294 # type: ignore
+EVEX_VPANDQ_YMM_K1Z_YMM_YMMM256B64: int = 2294
 """
 ``VPANDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 DB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2295 # type: ignore
+EVEX_VPANDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2295
 """
 ``VPANDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 DB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PADDUSB_MM_MMM64: Code = 2296 # type: ignore
+PADDUSB_MM_MMM64: int = 2296
 """
 ``PADDUSB mm, mm/m64``
 
 ``NP 0F DC /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDUSB_XMM_XMMM128: Code = 2297 # type: ignore
+PADDUSB_XMM_XMMM128: int = 2297
 """
 ``PADDUSB xmm1, xmm2/m128``
 
 ``66 0F DC /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDUSB_XMM_XMM_XMMM128: Code = 2298 # type: ignore
+VEX_VPADDUSB_XMM_XMM_XMMM128: int = 2298
 """
 ``VPADDUSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DC /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDUSB_YMM_YMM_YMMM256: Code = 2299 # type: ignore
+VEX_VPADDUSB_YMM_YMM_YMMM256: int = 2299
 """
 ``VPADDUSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DC /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSB_XMM_K1Z_XMM_XMMM128: Code = 2300 # type: ignore
+EVEX_VPADDUSB_XMM_K1Z_XMM_XMMM128: int = 2300
 """
 ``VPADDUSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG DC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSB_YMM_K1Z_YMM_YMMM256: Code = 2301 # type: ignore
+EVEX_VPADDUSB_YMM_K1Z_YMM_YMMM256: int = 2301
 """
 ``VPADDUSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG DC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2302 # type: ignore
+EVEX_VPADDUSB_ZMM_K1Z_ZMM_ZMMM512: int = 2302
 """
 ``VPADDUSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG DC /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PADDUSW_MM_MMM64: Code = 2303 # type: ignore
+PADDUSW_MM_MMM64: int = 2303
 """
 ``PADDUSW mm, mm/m64``
 
 ``NP 0F DD /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDUSW_XMM_XMMM128: Code = 2304 # type: ignore
+PADDUSW_XMM_XMMM128: int = 2304
 """
 ``PADDUSW xmm1, xmm2/m128``
 
 ``66 0F DD /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDUSW_XMM_XMM_XMMM128: Code = 2305 # type: ignore
+VEX_VPADDUSW_XMM_XMM_XMMM128: int = 2305
 """
 ``VPADDUSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DD /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDUSW_YMM_YMM_YMMM256: Code = 2306 # type: ignore
+VEX_VPADDUSW_YMM_YMM_YMMM256: int = 2306
 """
 ``VPADDUSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DD /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSW_XMM_K1Z_XMM_XMMM128: Code = 2307 # type: ignore
+EVEX_VPADDUSW_XMM_K1Z_XMM_XMMM128: int = 2307
 """
 ``VPADDUSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG DD /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSW_YMM_K1Z_YMM_YMMM256: Code = 2308 # type: ignore
+EVEX_VPADDUSW_YMM_K1Z_YMM_YMMM256: int = 2308
 """
 ``VPADDUSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG DD /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDUSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2309 # type: ignore
+EVEX_VPADDUSW_ZMM_K1Z_ZMM_ZMMM512: int = 2309
 """
 ``VPADDUSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG DD /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMAXUB_MM_MMM64: Code = 2310 # type: ignore
+PMAXUB_MM_MMM64: int = 2310
 """
 ``PMAXUB mm1, mm2/m64``
 
 ``NP 0F DE /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMAXUB_XMM_XMMM128: Code = 2311 # type: ignore
+PMAXUB_XMM_XMMM128: int = 2311
 """
 ``PMAXUB xmm1, xmm2/m128``
 
 ``66 0F DE /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUB_XMM_XMM_XMMM128: Code = 2312 # type: ignore
+VEX_VPMAXUB_XMM_XMM_XMMM128: int = 2312
 """
 ``VPMAXUB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DE /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUB_YMM_YMM_YMMM256: Code = 2313 # type: ignore
+VEX_VPMAXUB_YMM_YMM_YMMM256: int = 2313
 """
 ``VPMAXUB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DE /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUB_XMM_K1Z_XMM_XMMM128: Code = 2314 # type: ignore
+EVEX_VPMAXUB_XMM_K1Z_XMM_XMMM128: int = 2314
 """
 ``VPMAXUB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG DE /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUB_YMM_K1Z_YMM_YMMM256: Code = 2315 # type: ignore
+EVEX_VPMAXUB_YMM_K1Z_YMM_YMMM256: int = 2315
 """
 ``VPMAXUB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG DE /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUB_ZMM_K1Z_ZMM_ZMMM512: Code = 2316 # type: ignore
+EVEX_VPMAXUB_ZMM_K1Z_ZMM_ZMMM512: int = 2316
 """
 ``VPMAXUB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG DE /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PANDN_MM_MMM64: Code = 2317 # type: ignore
+PANDN_MM_MMM64: int = 2317
 """
 ``PANDN mm, mm/m64``
 
 ``NP 0F DF /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PANDN_XMM_XMMM128: Code = 2318 # type: ignore
+PANDN_XMM_XMMM128: int = 2318
 """
 ``PANDN xmm1, xmm2/m128``
 
 ``66 0F DF /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPANDN_XMM_XMM_XMMM128: Code = 2319 # type: ignore
+VEX_VPANDN_XMM_XMM_XMMM128: int = 2319
 """
 ``VPANDN xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG DF /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPANDN_YMM_YMM_YMMM256: Code = 2320 # type: ignore
+VEX_VPANDN_YMM_YMM_YMMM256: int = 2320
 """
 ``VPANDN ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG DF /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDND_XMM_K1Z_XMM_XMMM128B32: Code = 2321 # type: ignore
+EVEX_VPANDND_XMM_K1Z_XMM_XMMM128B32: int = 2321
 """
 ``VPANDND xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 DF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDND_YMM_K1Z_YMM_YMMM256B32: Code = 2322 # type: ignore
+EVEX_VPANDND_YMM_K1Z_YMM_YMMM256B32: int = 2322
 """
 ``VPANDND ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 DF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDND_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2323 # type: ignore
+EVEX_VPANDND_ZMM_K1Z_ZMM_ZMMM512B32: int = 2323
 """
 ``VPANDND zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 DF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDNQ_XMM_K1Z_XMM_XMMM128B64: Code = 2324 # type: ignore
+EVEX_VPANDNQ_XMM_K1Z_XMM_XMMM128B64: int = 2324
 """
 ``VPANDNQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 DF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDNQ_YMM_K1Z_YMM_YMMM256B64: Code = 2325 # type: ignore
+EVEX_VPANDNQ_YMM_K1Z_YMM_YMMM256B64: int = 2325
 """
 ``VPANDNQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 DF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPANDNQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2326 # type: ignore
+EVEX_VPANDNQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2326
 """
 ``VPANDNQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 DF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PAVGB_MM_MMM64: Code = 2327 # type: ignore
+PAVGB_MM_MMM64: int = 2327
 """
 ``PAVGB mm1, mm2/m64``
 
 ``NP 0F E0 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PAVGB_XMM_XMMM128: Code = 2328 # type: ignore
+PAVGB_XMM_XMMM128: int = 2328
 """
 ``PAVGB xmm1, xmm2/m128``
 
 ``66 0F E0 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPAVGB_XMM_XMM_XMMM128: Code = 2329 # type: ignore
+VEX_VPAVGB_XMM_XMM_XMMM128: int = 2329
 """
 ``VPAVGB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPAVGB_YMM_YMM_YMMM256: Code = 2330 # type: ignore
+VEX_VPAVGB_YMM_YMM_YMMM256: int = 2330
 """
 ``VPAVGB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E0 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGB_XMM_K1Z_XMM_XMMM128: Code = 2331 # type: ignore
+EVEX_VPAVGB_XMM_K1Z_XMM_XMMM128: int = 2331
 """
 ``VPAVGB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E0 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGB_YMM_K1Z_YMM_YMMM256: Code = 2332 # type: ignore
+EVEX_VPAVGB_YMM_K1Z_YMM_YMMM256: int = 2332
 """
 ``VPAVGB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E0 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGB_ZMM_K1Z_ZMM_ZMMM512: Code = 2333 # type: ignore
+EVEX_VPAVGB_ZMM_K1Z_ZMM_ZMMM512: int = 2333
 """
 ``VPAVGB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E0 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSRAW_MM_MMM64: Code = 2334 # type: ignore
+PSRAW_MM_MMM64: int = 2334
 """
 ``PSRAW mm, mm/m64``
 
 ``NP 0F E1 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRAW_XMM_XMMM128: Code = 2335 # type: ignore
+PSRAW_XMM_XMMM128: int = 2335
 """
 ``PSRAW xmm1, xmm2/m128``
 
 ``66 0F E1 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAW_XMM_XMM_XMMM128: Code = 2336 # type: ignore
+VEX_VPSRAW_XMM_XMM_XMMM128: int = 2336
 """
 ``VPSRAW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E1 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAW_YMM_YMM_XMMM128: Code = 2337 # type: ignore
+VEX_VPSRAW_YMM_YMM_XMMM128: int = 2337
 """
 ``VPSRAW ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG E1 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_XMM_K1Z_XMM_XMMM128: Code = 2338 # type: ignore
+EVEX_VPSRAW_XMM_K1Z_XMM_XMMM128: int = 2338
 """
 ``VPSRAW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_YMM_K1Z_YMM_XMMM128: Code = 2339 # type: ignore
+EVEX_VPSRAW_YMM_K1Z_YMM_XMMM128: int = 2339
 """
 ``VPSRAW ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.WIG E1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAW_ZMM_K1Z_ZMM_XMMM128: Code = 2340 # type: ignore
+EVEX_VPSRAW_ZMM_K1Z_ZMM_XMMM128: int = 2340
 """
 ``VPSRAW zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.WIG E1 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSRAD_MM_MMM64: Code = 2341 # type: ignore
+PSRAD_MM_MMM64: int = 2341
 """
 ``PSRAD mm, mm/m64``
 
 ``NP 0F E2 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSRAD_XMM_XMMM128: Code = 2342 # type: ignore
+PSRAD_XMM_XMMM128: int = 2342
 """
 ``PSRAD xmm1, xmm2/m128``
 
 ``66 0F E2 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAD_XMM_XMM_XMMM128: Code = 2343 # type: ignore
+VEX_VPSRAD_XMM_XMM_XMMM128: int = 2343
 """
 ``VPSRAD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E2 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAD_YMM_YMM_XMMM128: Code = 2344 # type: ignore
+VEX_VPSRAD_YMM_YMM_XMMM128: int = 2344
 """
 ``VPSRAD ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG E2 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_XMM_K1Z_XMM_XMMM128: Code = 2345 # type: ignore
+EVEX_VPSRAD_XMM_K1Z_XMM_XMMM128: int = 2345
 """
 ``VPSRAD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W0 E2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_YMM_K1Z_YMM_XMMM128: Code = 2346 # type: ignore
+EVEX_VPSRAD_YMM_K1Z_YMM_XMMM128: int = 2346
 """
 ``VPSRAD ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W0 E2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAD_ZMM_K1Z_ZMM_XMMM128: Code = 2347 # type: ignore
+EVEX_VPSRAD_ZMM_K1Z_ZMM_XMMM128: int = 2347
 """
 ``VPSRAD zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W0 E2 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_XMM_K1Z_XMM_XMMM128: Code = 2348 # type: ignore
+EVEX_VPSRAQ_XMM_K1Z_XMM_XMMM128: int = 2348
 """
 ``VPSRAQ xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W1 E2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_YMM_K1Z_YMM_XMMM128: Code = 2349 # type: ignore
+EVEX_VPSRAQ_YMM_K1Z_YMM_XMMM128: int = 2349
 """
 ``VPSRAQ ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W1 E2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAQ_ZMM_K1Z_ZMM_XMMM128: Code = 2350 # type: ignore
+EVEX_VPSRAQ_ZMM_K1Z_ZMM_XMMM128: int = 2350
 """
 ``VPSRAQ zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W1 E2 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PAVGW_MM_MMM64: Code = 2351 # type: ignore
+PAVGW_MM_MMM64: int = 2351
 """
 ``PAVGW mm1, mm2/m64``
 
 ``NP 0F E3 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PAVGW_XMM_XMMM128: Code = 2352 # type: ignore
+PAVGW_XMM_XMMM128: int = 2352
 """
 ``PAVGW xmm1, xmm2/m128``
 
 ``66 0F E3 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPAVGW_XMM_XMM_XMMM128: Code = 2353 # type: ignore
+VEX_VPAVGW_XMM_XMM_XMMM128: int = 2353
 """
 ``VPAVGW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E3 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPAVGW_YMM_YMM_YMMM256: Code = 2354 # type: ignore
+VEX_VPAVGW_YMM_YMM_YMMM256: int = 2354
 """
 ``VPAVGW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E3 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGW_XMM_K1Z_XMM_XMMM128: Code = 2355 # type: ignore
+EVEX_VPAVGW_XMM_K1Z_XMM_XMMM128: int = 2355
 """
 ``VPAVGW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E3 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGW_YMM_K1Z_YMM_YMMM256: Code = 2356 # type: ignore
+EVEX_VPAVGW_YMM_K1Z_YMM_YMMM256: int = 2356
 """
 ``VPAVGW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E3 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPAVGW_ZMM_K1Z_ZMM_ZMMM512: Code = 2357 # type: ignore
+EVEX_VPAVGW_ZMM_K1Z_ZMM_ZMMM512: int = 2357
 """
 ``VPAVGW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E3 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMULHUW_MM_MMM64: Code = 2358 # type: ignore
+PMULHUW_MM_MMM64: int = 2358
 """
 ``PMULHUW mm1, mm2/m64``
 
 ``NP 0F E4 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMULHUW_XMM_XMMM128: Code = 2359 # type: ignore
+PMULHUW_XMM_XMMM128: int = 2359
 """
 ``PMULHUW xmm1, xmm2/m128``
 
 ``66 0F E4 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHUW_XMM_XMM_XMMM128: Code = 2360 # type: ignore
+VEX_VPMULHUW_XMM_XMM_XMMM128: int = 2360
 """
 ``VPMULHUW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E4 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHUW_YMM_YMM_YMMM256: Code = 2361 # type: ignore
+VEX_VPMULHUW_YMM_YMM_YMMM256: int = 2361
 """
 ``VPMULHUW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E4 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHUW_XMM_K1Z_XMM_XMMM128: Code = 2362 # type: ignore
+EVEX_VPMULHUW_XMM_K1Z_XMM_XMMM128: int = 2362
 """
 ``VPMULHUW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E4 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHUW_YMM_K1Z_YMM_YMMM256: Code = 2363 # type: ignore
+EVEX_VPMULHUW_YMM_K1Z_YMM_YMMM256: int = 2363
 """
 ``VPMULHUW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E4 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHUW_ZMM_K1Z_ZMM_ZMMM512: Code = 2364 # type: ignore
+EVEX_VPMULHUW_ZMM_K1Z_ZMM_ZMMM512: int = 2364
 """
 ``VPMULHUW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E4 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMULHW_MM_MMM64: Code = 2365 # type: ignore
+PMULHW_MM_MMM64: int = 2365
 """
 ``PMULHW mm, mm/m64``
 
 ``NP 0F E5 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PMULHW_XMM_XMMM128: Code = 2366 # type: ignore
+PMULHW_XMM_XMMM128: int = 2366
 """
 ``PMULHW xmm1, xmm2/m128``
 
 ``66 0F E5 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHW_XMM_XMM_XMMM128: Code = 2367 # type: ignore
+VEX_VPMULHW_XMM_XMM_XMMM128: int = 2367
 """
 ``VPMULHW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E5 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHW_YMM_YMM_YMMM256: Code = 2368 # type: ignore
+VEX_VPMULHW_YMM_YMM_YMMM256: int = 2368
 """
 ``VPMULHW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E5 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHW_XMM_K1Z_XMM_XMMM128: Code = 2369 # type: ignore
+EVEX_VPMULHW_XMM_K1Z_XMM_XMMM128: int = 2369
 """
 ``VPMULHW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHW_YMM_K1Z_YMM_YMMM256: Code = 2370 # type: ignore
+EVEX_VPMULHW_YMM_K1Z_YMM_YMMM256: int = 2370
 """
 ``VPMULHW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHW_ZMM_K1Z_ZMM_ZMMM512: Code = 2371 # type: ignore
+EVEX_VPMULHW_ZMM_K1Z_ZMM_ZMMM512: int = 2371
 """
 ``VPMULHW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E5 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-CVTTPD2DQ_XMM_XMMM128: Code = 2372 # type: ignore
+CVTTPD2DQ_XMM_XMMM128: int = 2372
 """
 ``CVTTPD2DQ xmm1, xmm2/m128``
 
 ``66 0F E6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTPD2DQ_XMM_XMMM128: Code = 2373 # type: ignore
+VEX_VCVTTPD2DQ_XMM_XMMM128: int = 2373
 """
 ``VCVTTPD2DQ xmm1, xmm2/m128``
 
 ``VEX.128.66.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTTPD2DQ_XMM_YMMM256: Code = 2374 # type: ignore
+VEX_VCVTTPD2DQ_XMM_YMMM256: int = 2374
 """
 ``VCVTTPD2DQ xmm1, ymm2/m256``
 
 ``VEX.256.66.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2DQ_XMM_K1Z_XMMM128B64: Code = 2375 # type: ignore
+EVEX_VCVTTPD2DQ_XMM_K1Z_XMMM128B64: int = 2375
 """
 ``VCVTTPD2DQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2DQ_XMM_K1Z_YMMM256B64: Code = 2376 # type: ignore
+EVEX_VCVTTPD2DQ_XMM_K1Z_YMMM256B64: int = 2376
 """
 ``VCVTTPD2DQ xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTTPD2DQ_YMM_K1Z_ZMMM512B64_SAE: Code = 2377 # type: ignore
+EVEX_VCVTTPD2DQ_YMM_K1Z_ZMMM512B64_SAE: int = 2377
 """
 ``VCVTTPD2DQ ymm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F.W1 E6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-CVTDQ2PD_XMM_XMMM64: Code = 2378 # type: ignore
+CVTDQ2PD_XMM_XMMM64: int = 2378
 """
 ``CVTDQ2PD xmm1, xmm2/m64``
 
 ``F3 0F E6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTDQ2PD_XMM_XMMM64: Code = 2379 # type: ignore
+VEX_VCVTDQ2PD_XMM_XMMM64: int = 2379
 """
 ``VCVTDQ2PD xmm1, xmm2/m64``
 
 ``VEX.128.F3.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTDQ2PD_YMM_XMMM128: Code = 2380 # type: ignore
+VEX_VCVTDQ2PD_YMM_XMMM128: int = 2380
 """
 ``VCVTDQ2PD ymm1, xmm2/m128``
 
 ``VEX.256.F3.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PD_XMM_K1Z_XMMM64B32: Code = 2381 # type: ignore
+EVEX_VCVTDQ2PD_XMM_K1Z_XMMM64B32: int = 2381
 """
 ``VCVTDQ2PD xmm1 {k1}{z}, xmm2/m64/m32bcst``
 
 ``EVEX.128.F3.0F.W0 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PD_YMM_K1Z_XMMM128B32: Code = 2382 # type: ignore
+EVEX_VCVTDQ2PD_YMM_K1Z_XMMM128B32: int = 2382
 """
 ``VCVTDQ2PD ymm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.256.F3.0F.W0 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTDQ2PD_ZMM_K1Z_YMMM256B32_ER: Code = 2383 # type: ignore
+EVEX_VCVTDQ2PD_ZMM_K1Z_YMMM256B32_ER: int = 2383
 """
 ``VCVTDQ2PD zmm1 {k1}{z}, ymm2/m256/m32bcst{er}``
 
 ``EVEX.512.F3.0F.W0 E6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PD_XMM_K1Z_XMMM128B64: Code = 2384 # type: ignore
+EVEX_VCVTQQ2PD_XMM_K1Z_XMMM128B64: int = 2384
 """
 ``VCVTQQ2PD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.F3.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PD_YMM_K1Z_YMMM256B64: Code = 2385 # type: ignore
+EVEX_VCVTQQ2PD_YMM_K1Z_YMMM256B64: int = 2385
 """
 ``VCVTQQ2PD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.F3.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTQQ2PD_ZMM_K1Z_ZMMM512B64_ER: Code = 2386 # type: ignore
+EVEX_VCVTQQ2PD_ZMM_K1Z_ZMMM512B64_ER: int = 2386
 """
 ``VCVTQQ2PD zmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.F3.0F.W1 E6 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-CVTPD2DQ_XMM_XMMM128: Code = 2387 # type: ignore
+CVTPD2DQ_XMM_XMMM128: int = 2387
 """
 ``CVTPD2DQ xmm1, xmm2/m128``
 
 ``F2 0F E6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPD2DQ_XMM_XMMM128: Code = 2388 # type: ignore
+VEX_VCVTPD2DQ_XMM_XMMM128: int = 2388
 """
 ``VCVTPD2DQ xmm1, xmm2/m128``
 
 ``VEX.128.F2.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPD2DQ_XMM_YMMM256: Code = 2389 # type: ignore
+VEX_VCVTPD2DQ_XMM_YMMM256: int = 2389
 """
 ``VCVTPD2DQ xmm1, ymm2/m256``
 
 ``VEX.256.F2.0F.WIG E6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2DQ_XMM_K1Z_XMMM128B64: Code = 2390 # type: ignore
+EVEX_VCVTPD2DQ_XMM_K1Z_XMMM128B64: int = 2390
 """
 ``VCVTPD2DQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.F2.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2DQ_XMM_K1Z_YMMM256B64: Code = 2391 # type: ignore
+EVEX_VCVTPD2DQ_XMM_K1Z_YMMM256B64: int = 2391
 """
 ``VCVTPD2DQ xmm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.F2.0F.W1 E6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPD2DQ_YMM_K1Z_ZMMM512B64_ER: Code = 2392 # type: ignore
+EVEX_VCVTPD2DQ_YMM_K1Z_ZMMM512B64_ER: int = 2392
 """
 ``VCVTPD2DQ ymm1 {k1}{z}, zmm2/m512/m64bcst{er}``
 
 ``EVEX.512.F2.0F.W1 E6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-MOVNTQ_M64_MM: Code = 2393 # type: ignore
+MOVNTQ_M64_MM: int = 2393
 """
 ``MOVNTQ m64, mm``
 
 ``NP 0F E7 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-MOVNTDQ_M128_XMM: Code = 2394 # type: ignore
+MOVNTDQ_M128_XMM: int = 2394
 """
 ``MOVNTDQ m128, xmm1``
 
 ``66 0F E7 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTDQ_M128_XMM: Code = 2395 # type: ignore
+VEX_VMOVNTDQ_M128_XMM: int = 2395
 """
 ``VMOVNTDQ m128, xmm1``
 
 ``VEX.128.66.0F.WIG E7 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTDQ_M256_YMM: Code = 2396 # type: ignore
+VEX_VMOVNTDQ_M256_YMM: int = 2396
 """
 ``VMOVNTDQ m256, ymm1``
 
 ``VEX.256.66.0F.WIG E7 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQ_M128_XMM: Code = 2397 # type: ignore
+EVEX_VMOVNTDQ_M128_XMM: int = 2397
 """
 ``VMOVNTDQ m128, xmm1``
 
 ``EVEX.128.66.0F.W0 E7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQ_M256_YMM: Code = 2398 # type: ignore
+EVEX_VMOVNTDQ_M256_YMM: int = 2398
 """
 ``VMOVNTDQ m256, ymm1``
 
 ``EVEX.256.66.0F.W0 E7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQ_M512_ZMM: Code = 2399 # type: ignore
+EVEX_VMOVNTDQ_M512_ZMM: int = 2399
 """
 ``VMOVNTDQ m512, zmm1``
 
 ``EVEX.512.66.0F.W0 E7 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSUBSB_MM_MMM64: Code = 2400 # type: ignore
+PSUBSB_MM_MMM64: int = 2400
 """
 ``PSUBSB mm, mm/m64``
 
 ``NP 0F E8 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBSB_XMM_XMMM128: Code = 2401 # type: ignore
+PSUBSB_XMM_XMMM128: int = 2401
 """
 ``PSUBSB xmm1, xmm2/m128``
 
 ``66 0F E8 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBSB_XMM_XMM_XMMM128: Code = 2402 # type: ignore
+VEX_VPSUBSB_XMM_XMM_XMMM128: int = 2402
 """
 ``VPSUBSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E8 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBSB_YMM_YMM_YMMM256: Code = 2403 # type: ignore
+VEX_VPSUBSB_YMM_YMM_YMMM256: int = 2403
 """
 ``VPSUBSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E8 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSB_XMM_K1Z_XMM_XMMM128: Code = 2404 # type: ignore
+EVEX_VPSUBSB_XMM_K1Z_XMM_XMMM128: int = 2404
 """
 ``VPSUBSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSB_YMM_K1Z_YMM_YMMM256: Code = 2405 # type: ignore
+EVEX_VPSUBSB_YMM_K1Z_YMM_YMMM256: int = 2405
 """
 ``VPSUBSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2406 # type: ignore
+EVEX_VPSUBSB_ZMM_K1Z_ZMM_ZMMM512: int = 2406
 """
 ``VPSUBSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E8 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSUBSW_MM_MMM64: Code = 2407 # type: ignore
+PSUBSW_MM_MMM64: int = 2407
 """
 ``PSUBSW mm, mm/m64``
 
 ``NP 0F E9 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBSW_XMM_XMMM128: Code = 2408 # type: ignore
+PSUBSW_XMM_XMMM128: int = 2408
 """
 ``PSUBSW xmm1, xmm2/m128``
 
 ``66 0F E9 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBSW_XMM_XMM_XMMM128: Code = 2409 # type: ignore
+VEX_VPSUBSW_XMM_XMM_XMMM128: int = 2409
 """
 ``VPSUBSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG E9 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBSW_YMM_YMM_YMMM256: Code = 2410 # type: ignore
+VEX_VPSUBSW_YMM_YMM_YMMM256: int = 2410
 """
 ``VPSUBSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG E9 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSW_XMM_K1Z_XMM_XMMM128: Code = 2411 # type: ignore
+EVEX_VPSUBSW_XMM_K1Z_XMM_XMMM128: int = 2411
 """
 ``VPSUBSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG E9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSW_YMM_K1Z_YMM_YMMM256: Code = 2412 # type: ignore
+EVEX_VPSUBSW_YMM_K1Z_YMM_YMMM256: int = 2412
 """
 ``VPSUBSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG E9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2413 # type: ignore
+EVEX_VPSUBSW_ZMM_K1Z_ZMM_ZMMM512: int = 2413
 """
 ``VPSUBSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG E9 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMINSW_MM_MMM64: Code = 2414 # type: ignore
+PMINSW_MM_MMM64: int = 2414
 """
 ``PMINSW mm1, mm2/m64``
 
 ``NP 0F EA /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMINSW_XMM_XMMM128: Code = 2415 # type: ignore
+PMINSW_XMM_XMMM128: int = 2415
 """
 ``PMINSW xmm1, xmm2/m128``
 
 ``66 0F EA /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSW_XMM_XMM_XMMM128: Code = 2416 # type: ignore
+VEX_VPMINSW_XMM_XMM_XMMM128: int = 2416
 """
 ``VPMINSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG EA /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSW_YMM_YMM_YMMM256: Code = 2417 # type: ignore
+VEX_VPMINSW_YMM_YMM_YMMM256: int = 2417
 """
 ``VPMINSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG EA /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSW_XMM_K1Z_XMM_XMMM128: Code = 2418 # type: ignore
+EVEX_VPMINSW_XMM_K1Z_XMM_XMMM128: int = 2418
 """
 ``VPMINSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG EA /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSW_YMM_K1Z_YMM_YMMM256: Code = 2419 # type: ignore
+EVEX_VPMINSW_YMM_K1Z_YMM_YMMM256: int = 2419
 """
 ``VPMINSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG EA /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2420 # type: ignore
+EVEX_VPMINSW_ZMM_K1Z_ZMM_ZMMM512: int = 2420
 """
 ``VPMINSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG EA /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-POR_MM_MMM64: Code = 2421 # type: ignore
+POR_MM_MMM64: int = 2421
 """
 ``POR mm, mm/m64``
 
 ``NP 0F EB /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-POR_XMM_XMMM128: Code = 2422 # type: ignore
+POR_XMM_XMMM128: int = 2422
 """
 ``POR xmm1, xmm2/m128``
 
 ``66 0F EB /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPOR_XMM_XMM_XMMM128: Code = 2423 # type: ignore
+VEX_VPOR_XMM_XMM_XMMM128: int = 2423
 """
 ``VPOR xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG EB /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPOR_YMM_YMM_YMMM256: Code = 2424 # type: ignore
+VEX_VPOR_YMM_YMM_YMMM256: int = 2424
 """
 ``VPOR ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG EB /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPORD_XMM_K1Z_XMM_XMMM128B32: Code = 2425 # type: ignore
+EVEX_VPORD_XMM_K1Z_XMM_XMMM128B32: int = 2425
 """
 ``VPORD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 EB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPORD_YMM_K1Z_YMM_YMMM256B32: Code = 2426 # type: ignore
+EVEX_VPORD_YMM_K1Z_YMM_YMMM256B32: int = 2426
 """
 ``VPORD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 EB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPORD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2427 # type: ignore
+EVEX_VPORD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2427
 """
 ``VPORD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 EB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPORQ_XMM_K1Z_XMM_XMMM128B64: Code = 2428 # type: ignore
+EVEX_VPORQ_XMM_K1Z_XMM_XMMM128B64: int = 2428
 """
 ``VPORQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 EB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPORQ_YMM_K1Z_YMM_YMMM256B64: Code = 2429 # type: ignore
+EVEX_VPORQ_YMM_K1Z_YMM_YMMM256B64: int = 2429
 """
 ``VPORQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 EB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPORQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2430 # type: ignore
+EVEX_VPORQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2430
 """
 ``VPORQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 EB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PADDSB_MM_MMM64: Code = 2431 # type: ignore
+PADDSB_MM_MMM64: int = 2431
 """
 ``PADDSB mm, mm/m64``
 
 ``NP 0F EC /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDSB_XMM_XMMM128: Code = 2432 # type: ignore
+PADDSB_XMM_XMMM128: int = 2432
 """
 ``PADDSB xmm1, xmm2/m128``
 
 ``66 0F EC /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDSB_XMM_XMM_XMMM128: Code = 2433 # type: ignore
+VEX_VPADDSB_XMM_XMM_XMMM128: int = 2433
 """
 ``VPADDSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG EC /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDSB_YMM_YMM_YMMM256: Code = 2434 # type: ignore
+VEX_VPADDSB_YMM_YMM_YMMM256: int = 2434
 """
 ``VPADDSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG EC /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSB_XMM_K1Z_XMM_XMMM128: Code = 2435 # type: ignore
+EVEX_VPADDSB_XMM_K1Z_XMM_XMMM128: int = 2435
 """
 ``VPADDSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG EC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSB_YMM_K1Z_YMM_YMMM256: Code = 2436 # type: ignore
+EVEX_VPADDSB_YMM_K1Z_YMM_YMMM256: int = 2436
 """
 ``VPADDSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG EC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2437 # type: ignore
+EVEX_VPADDSB_ZMM_K1Z_ZMM_ZMMM512: int = 2437
 """
 ``VPADDSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG EC /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PADDSW_MM_MMM64: Code = 2438 # type: ignore
+PADDSW_MM_MMM64: int = 2438
 """
 ``PADDSW mm, mm/m64``
 
 ``NP 0F ED /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDSW_XMM_XMMM128: Code = 2439 # type: ignore
+PADDSW_XMM_XMMM128: int = 2439
 """
 ``PADDSW xmm1, xmm2/m128``
 
 ``66 0F ED /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDSW_XMM_XMM_XMMM128: Code = 2440 # type: ignore
+VEX_VPADDSW_XMM_XMM_XMMM128: int = 2440
 """
 ``VPADDSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG ED /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDSW_YMM_YMM_YMMM256: Code = 2441 # type: ignore
+VEX_VPADDSW_YMM_YMM_YMMM256: int = 2441
 """
 ``VPADDSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG ED /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSW_XMM_K1Z_XMM_XMMM128: Code = 2442 # type: ignore
+EVEX_VPADDSW_XMM_K1Z_XMM_XMMM128: int = 2442
 """
 ``VPADDSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG ED /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSW_YMM_K1Z_YMM_YMMM256: Code = 2443 # type: ignore
+EVEX_VPADDSW_YMM_K1Z_YMM_YMMM256: int = 2443
 """
 ``VPADDSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG ED /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2444 # type: ignore
+EVEX_VPADDSW_ZMM_K1Z_ZMM_ZMMM512: int = 2444
 """
 ``VPADDSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG ED /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMAXSW_MM_MMM64: Code = 2445 # type: ignore
+PMAXSW_MM_MMM64: int = 2445
 """
 ``PMAXSW mm1, mm2/m64``
 
 ``NP 0F EE /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PMAXSW_XMM_XMMM128: Code = 2446 # type: ignore
+PMAXSW_XMM_XMMM128: int = 2446
 """
 ``PMAXSW xmm1, xmm2/m128``
 
 ``66 0F EE /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSW_XMM_XMM_XMMM128: Code = 2447 # type: ignore
+VEX_VPMAXSW_XMM_XMM_XMMM128: int = 2447
 """
 ``VPMAXSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG EE /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSW_YMM_YMM_YMMM256: Code = 2448 # type: ignore
+VEX_VPMAXSW_YMM_YMM_YMMM256: int = 2448
 """
 ``VPMAXSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG EE /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSW_XMM_K1Z_XMM_XMMM128: Code = 2449 # type: ignore
+EVEX_VPMAXSW_XMM_K1Z_XMM_XMMM128: int = 2449
 """
 ``VPMAXSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG EE /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSW_YMM_K1Z_YMM_YMMM256: Code = 2450 # type: ignore
+EVEX_VPMAXSW_YMM_K1Z_YMM_YMMM256: int = 2450
 """
 ``VPMAXSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG EE /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2451 # type: ignore
+EVEX_VPMAXSW_ZMM_K1Z_ZMM_ZMMM512: int = 2451
 """
 ``VPMAXSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG EE /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PXOR_MM_MMM64: Code = 2452 # type: ignore
+PXOR_MM_MMM64: int = 2452
 """
 ``PXOR mm, mm/m64``
 
 ``NP 0F EF /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PXOR_XMM_XMMM128: Code = 2453 # type: ignore
+PXOR_XMM_XMMM128: int = 2453
 """
 ``PXOR xmm1, xmm2/m128``
 
 ``66 0F EF /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPXOR_XMM_XMM_XMMM128: Code = 2454 # type: ignore
+VEX_VPXOR_XMM_XMM_XMMM128: int = 2454
 """
 ``VPXOR xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG EF /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPXOR_YMM_YMM_YMMM256: Code = 2455 # type: ignore
+VEX_VPXOR_YMM_YMM_YMMM256: int = 2455
 """
 ``VPXOR ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG EF /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORD_XMM_K1Z_XMM_XMMM128B32: Code = 2456 # type: ignore
+EVEX_VPXORD_XMM_K1Z_XMM_XMMM128B32: int = 2456
 """
 ``VPXORD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 EF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORD_YMM_K1Z_YMM_YMMM256B32: Code = 2457 # type: ignore
+EVEX_VPXORD_YMM_K1Z_YMM_YMMM256B32: int = 2457
 """
 ``VPXORD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 EF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2458 # type: ignore
+EVEX_VPXORD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2458
 """
 ``VPXORD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 EF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORQ_XMM_K1Z_XMM_XMMM128B64: Code = 2459 # type: ignore
+EVEX_VPXORQ_XMM_K1Z_XMM_XMMM128B64: int = 2459
 """
 ``VPXORQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 EF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORQ_YMM_K1Z_YMM_YMMM256B64: Code = 2460 # type: ignore
+EVEX_VPXORQ_YMM_K1Z_YMM_YMMM256B64: int = 2460
 """
 ``VPXORQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 EF /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPXORQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2461 # type: ignore
+EVEX_VPXORQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2461
 """
 ``VPXORQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 EF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-LDDQU_XMM_M128: Code = 2462 # type: ignore
+LDDQU_XMM_M128: int = 2462
 """
 ``LDDQU xmm1, m128``
 
 ``F2 0F F0 /r``
 
 ``SSE3``
 
 ``16/32/64-bit``
 """
-VEX_VLDDQU_XMM_M128: Code = 2463 # type: ignore
+VEX_VLDDQU_XMM_M128: int = 2463
 """
 ``VLDDQU xmm1, m128``
 
 ``VEX.128.F2.0F.WIG F0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VLDDQU_YMM_M256: Code = 2464 # type: ignore
+VEX_VLDDQU_YMM_M256: int = 2464
 """
 ``VLDDQU ymm1, m256``
 
 ``VEX.256.F2.0F.WIG F0 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PSLLW_MM_MMM64: Code = 2465 # type: ignore
+PSLLW_MM_MMM64: int = 2465
 """
 ``PSLLW mm, mm/m64``
 
 ``NP 0F F1 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLW_XMM_XMMM128: Code = 2466 # type: ignore
+PSLLW_XMM_XMMM128: int = 2466
 """
 ``PSLLW xmm1, xmm2/m128``
 
 ``66 0F F1 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLW_XMM_XMM_XMMM128: Code = 2467 # type: ignore
+VEX_VPSLLW_XMM_XMM_XMMM128: int = 2467
 """
 ``VPSLLW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F1 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLW_YMM_YMM_XMMM128: Code = 2468 # type: ignore
+VEX_VPSLLW_YMM_YMM_XMMM128: int = 2468
 """
 ``VPSLLW ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG F1 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_XMM_K1Z_XMM_XMMM128: Code = 2469 # type: ignore
+EVEX_VPSLLW_XMM_K1Z_XMM_XMMM128: int = 2469
 """
 ``VPSLLW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG F1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_YMM_K1Z_YMM_XMMM128: Code = 2470 # type: ignore
+EVEX_VPSLLW_YMM_K1Z_YMM_XMMM128: int = 2470
 """
 ``VPSLLW ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.WIG F1 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLW_ZMM_K1Z_ZMM_XMMM128: Code = 2471 # type: ignore
+EVEX_VPSLLW_ZMM_K1Z_ZMM_XMMM128: int = 2471
 """
 ``VPSLLW zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.WIG F1 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSLLD_MM_MMM64: Code = 2472 # type: ignore
+PSLLD_MM_MMM64: int = 2472
 """
 ``PSLLD mm, mm/m64``
 
 ``NP 0F F2 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLD_XMM_XMMM128: Code = 2473 # type: ignore
+PSLLD_XMM_XMMM128: int = 2473
 """
 ``PSLLD xmm1, xmm2/m128``
 
 ``66 0F F2 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLD_XMM_XMM_XMMM128: Code = 2474 # type: ignore
+VEX_VPSLLD_XMM_XMM_XMMM128: int = 2474
 """
 ``VPSLLD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F2 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLD_YMM_YMM_XMMM128: Code = 2475 # type: ignore
+VEX_VPSLLD_YMM_YMM_XMMM128: int = 2475
 """
 ``VPSLLD ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG F2 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_XMM_K1Z_XMM_XMMM128: Code = 2476 # type: ignore
+EVEX_VPSLLD_XMM_K1Z_XMM_XMMM128: int = 2476
 """
 ``VPSLLD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W0 F2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_YMM_K1Z_YMM_XMMM128: Code = 2477 # type: ignore
+EVEX_VPSLLD_YMM_K1Z_YMM_XMMM128: int = 2477
 """
 ``VPSLLD ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W0 F2 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLD_ZMM_K1Z_ZMM_XMMM128: Code = 2478 # type: ignore
+EVEX_VPSLLD_ZMM_K1Z_ZMM_XMMM128: int = 2478
 """
 ``VPSLLD zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W0 F2 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSLLQ_MM_MMM64: Code = 2479 # type: ignore
+PSLLQ_MM_MMM64: int = 2479
 """
 ``PSLLQ mm, mm/m64``
 
 ``NP 0F F3 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSLLQ_XMM_XMMM128: Code = 2480 # type: ignore
+PSLLQ_XMM_XMMM128: int = 2480
 """
 ``PSLLQ xmm1, xmm2/m128``
 
 ``66 0F F3 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLQ_XMM_XMM_XMMM128: Code = 2481 # type: ignore
+VEX_VPSLLQ_XMM_XMM_XMMM128: int = 2481
 """
 ``VPSLLQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F3 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLQ_YMM_YMM_XMMM128: Code = 2482 # type: ignore
+VEX_VPSLLQ_YMM_YMM_XMMM128: int = 2482
 """
 ``VPSLLQ ymm1, ymm2, xmm3/m128``
 
 ``VEX.256.66.0F.WIG F3 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_XMM_K1Z_XMM_XMMM128: Code = 2483 # type: ignore
+EVEX_VPSLLQ_XMM_K1Z_XMM_XMMM128: int = 2483
 """
 ``VPSLLQ xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.W1 F3 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_YMM_K1Z_YMM_XMMM128: Code = 2484 # type: ignore
+EVEX_VPSLLQ_YMM_K1Z_YMM_XMMM128: int = 2484
 """
 ``VPSLLQ ymm1 {k1}{z}, ymm2, xmm3/m128``
 
 ``EVEX.256.66.0F.W1 F3 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLQ_ZMM_K1Z_ZMM_XMMM128: Code = 2485 # type: ignore
+EVEX_VPSLLQ_ZMM_K1Z_ZMM_XMMM128: int = 2485
 """
 ``VPSLLQ zmm1 {k1}{z}, zmm2, xmm3/m128``
 
 ``EVEX.512.66.0F.W1 F3 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMULUDQ_MM_MMM64: Code = 2486 # type: ignore
+PMULUDQ_MM_MMM64: int = 2486
 """
 ``PMULUDQ mm1, mm2/m64``
 
 ``NP 0F F4 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PMULUDQ_XMM_XMMM128: Code = 2487 # type: ignore
+PMULUDQ_XMM_XMMM128: int = 2487
 """
 ``PMULUDQ xmm1, xmm2/m128``
 
 ``66 0F F4 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMULUDQ_XMM_XMM_XMMM128: Code = 2488 # type: ignore
+VEX_VPMULUDQ_XMM_XMM_XMMM128: int = 2488
 """
 ``VPMULUDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F4 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULUDQ_YMM_YMM_YMMM256: Code = 2489 # type: ignore
+VEX_VPMULUDQ_YMM_YMM_YMMM256: int = 2489
 """
 ``VPMULUDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG F4 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULUDQ_XMM_K1Z_XMM_XMMM128B64: Code = 2490 # type: ignore
+EVEX_VPMULUDQ_XMM_K1Z_XMM_XMMM128B64: int = 2490
 """
 ``VPMULUDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 F4 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULUDQ_YMM_K1Z_YMM_YMMM256B64: Code = 2491 # type: ignore
+EVEX_VPMULUDQ_YMM_K1Z_YMM_YMMM256B64: int = 2491
 """
 ``VPMULUDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 F4 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULUDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2492 # type: ignore
+EVEX_VPMULUDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2492
 """
 ``VPMULUDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 F4 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMADDWD_MM_MMM64: Code = 2493 # type: ignore
+PMADDWD_MM_MMM64: int = 2493
 """
 ``PMADDWD mm, mm/m64``
 
 ``NP 0F F5 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PMADDWD_XMM_XMMM128: Code = 2494 # type: ignore
+PMADDWD_XMM_XMMM128: int = 2494
 """
 ``PMADDWD xmm1, xmm2/m128``
 
 ``66 0F F5 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPMADDWD_XMM_XMM_XMMM128: Code = 2495 # type: ignore
+VEX_VPMADDWD_XMM_XMM_XMMM128: int = 2495
 """
 ``VPMADDWD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F5 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMADDWD_YMM_YMM_YMMM256: Code = 2496 # type: ignore
+VEX_VPMADDWD_YMM_YMM_YMMM256: int = 2496
 """
 ``VPMADDWD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG F5 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDWD_XMM_K1Z_XMM_XMMM128: Code = 2497 # type: ignore
+EVEX_VPMADDWD_XMM_K1Z_XMM_XMMM128: int = 2497
 """
 ``VPMADDWD xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG F5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDWD_YMM_K1Z_YMM_YMMM256: Code = 2498 # type: ignore
+EVEX_VPMADDWD_YMM_K1Z_YMM_YMMM256: int = 2498
 """
 ``VPMADDWD ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG F5 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDWD_ZMM_K1Z_ZMM_ZMMM512: Code = 2499 # type: ignore
+EVEX_VPMADDWD_ZMM_K1Z_ZMM_ZMMM512: int = 2499
 """
 ``VPMADDWD zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG F5 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSADBW_MM_MMM64: Code = 2500 # type: ignore
+PSADBW_MM_MMM64: int = 2500
 """
 ``PSADBW mm1, mm2/m64``
 
 ``NP 0F F6 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-PSADBW_XMM_XMMM128: Code = 2501 # type: ignore
+PSADBW_XMM_XMMM128: int = 2501
 """
 ``PSADBW xmm1, xmm2/m128``
 
 ``66 0F F6 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSADBW_XMM_XMM_XMMM128: Code = 2502 # type: ignore
+VEX_VPSADBW_XMM_XMM_XMMM128: int = 2502
 """
 ``VPSADBW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F6 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSADBW_YMM_YMM_YMMM256: Code = 2503 # type: ignore
+VEX_VPSADBW_YMM_YMM_YMMM256: int = 2503
 """
 ``VPSADBW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG F6 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSADBW_XMM_XMM_XMMM128: Code = 2504 # type: ignore
+EVEX_VPSADBW_XMM_XMM_XMMM128: int = 2504
 """
 ``VPSADBW xmm1, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG F6 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSADBW_YMM_YMM_YMMM256: Code = 2505 # type: ignore
+EVEX_VPSADBW_YMM_YMM_YMMM256: int = 2505
 """
 ``VPSADBW ymm1, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG F6 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSADBW_ZMM_ZMM_ZMMM512: Code = 2506 # type: ignore
+EVEX_VPSADBW_ZMM_ZMM_ZMMM512: int = 2506
 """
 ``VPSADBW zmm1, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG F6 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-MASKMOVQ_RDI_MM_MM: Code = 2507 # type: ignore
+MASKMOVQ_RDI_MM_MM: int = 2507
 """
 ``MASKMOVQ mm1, mm2``
 
 ``NP 0F F7 /r``
 
 ``SSE``
 
 ``16/32/64-bit``
 """
-MASKMOVDQU_RDI_XMM_XMM: Code = 2508 # type: ignore
+MASKMOVDQU_RDI_XMM_XMM: int = 2508
 """
 ``MASKMOVDQU xmm1, xmm2``
 
 ``66 0F F7 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVDQU_RDI_XMM_XMM: Code = 2509 # type: ignore
+VEX_VMASKMOVDQU_RDI_XMM_XMM: int = 2509
 """
 ``VMASKMOVDQU xmm1, xmm2``
 
 ``VEX.128.66.0F.WIG F7 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PSUBB_MM_MMM64: Code = 2510 # type: ignore
+PSUBB_MM_MMM64: int = 2510
 """
 ``PSUBB mm, mm/m64``
 
 ``NP 0F F8 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBB_XMM_XMMM128: Code = 2511 # type: ignore
+PSUBB_XMM_XMMM128: int = 2511
 """
 ``PSUBB xmm1, xmm2/m128``
 
 ``66 0F F8 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBB_XMM_XMM_XMMM128: Code = 2512 # type: ignore
+VEX_VPSUBB_XMM_XMM_XMMM128: int = 2512
 """
 ``VPSUBB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F8 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBB_YMM_YMM_YMMM256: Code = 2513 # type: ignore
+VEX_VPSUBB_YMM_YMM_YMMM256: int = 2513
 """
 ``VPSUBB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG F8 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBB_XMM_K1Z_XMM_XMMM128: Code = 2514 # type: ignore
+EVEX_VPSUBB_XMM_K1Z_XMM_XMMM128: int = 2514
 """
 ``VPSUBB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG F8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBB_YMM_K1Z_YMM_YMMM256: Code = 2515 # type: ignore
+EVEX_VPSUBB_YMM_K1Z_YMM_YMMM256: int = 2515
 """
 ``VPSUBB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG F8 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBB_ZMM_K1Z_ZMM_ZMMM512: Code = 2516 # type: ignore
+EVEX_VPSUBB_ZMM_K1Z_ZMM_ZMMM512: int = 2516
 """
 ``VPSUBB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG F8 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSUBW_MM_MMM64: Code = 2517 # type: ignore
+PSUBW_MM_MMM64: int = 2517
 """
 ``PSUBW mm, mm/m64``
 
 ``NP 0F F9 /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBW_XMM_XMMM128: Code = 2518 # type: ignore
+PSUBW_XMM_XMMM128: int = 2518
 """
 ``PSUBW xmm1, xmm2/m128``
 
 ``66 0F F9 /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBW_XMM_XMM_XMMM128: Code = 2519 # type: ignore
+VEX_VPSUBW_XMM_XMM_XMMM128: int = 2519
 """
 ``VPSUBW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG F9 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBW_YMM_YMM_YMMM256: Code = 2520 # type: ignore
+VEX_VPSUBW_YMM_YMM_YMMM256: int = 2520
 """
 ``VPSUBW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG F9 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBW_XMM_K1Z_XMM_XMMM128: Code = 2521 # type: ignore
+EVEX_VPSUBW_XMM_K1Z_XMM_XMMM128: int = 2521
 """
 ``VPSUBW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG F9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBW_YMM_K1Z_YMM_YMMM256: Code = 2522 # type: ignore
+EVEX_VPSUBW_YMM_K1Z_YMM_YMMM256: int = 2522
 """
 ``VPSUBW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG F9 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBW_ZMM_K1Z_ZMM_ZMMM512: Code = 2523 # type: ignore
+EVEX_VPSUBW_ZMM_K1Z_ZMM_ZMMM512: int = 2523
 """
 ``VPSUBW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG F9 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PSUBD_MM_MMM64: Code = 2524 # type: ignore
+PSUBD_MM_MMM64: int = 2524
 """
 ``PSUBD mm, mm/m64``
 
 ``NP 0F FA /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PSUBD_XMM_XMMM128: Code = 2525 # type: ignore
+PSUBD_XMM_XMMM128: int = 2525
 """
 ``PSUBD xmm1, xmm2/m128``
 
 ``66 0F FA /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBD_XMM_XMM_XMMM128: Code = 2526 # type: ignore
+VEX_VPSUBD_XMM_XMM_XMMM128: int = 2526
 """
 ``VPSUBD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG FA /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBD_YMM_YMM_YMMM256: Code = 2527 # type: ignore
+VEX_VPSUBD_YMM_YMM_YMMM256: int = 2527
 """
 ``VPSUBD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG FA /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBD_XMM_K1Z_XMM_XMMM128B32: Code = 2528 # type: ignore
+EVEX_VPSUBD_XMM_K1Z_XMM_XMMM128B32: int = 2528
 """
 ``VPSUBD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 FA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBD_YMM_K1Z_YMM_YMMM256B32: Code = 2529 # type: ignore
+EVEX_VPSUBD_YMM_K1Z_YMM_YMMM256B32: int = 2529
 """
 ``VPSUBD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 FA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2530 # type: ignore
+EVEX_VPSUBD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2530
 """
 ``VPSUBD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 FA /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PSUBQ_MM_MMM64: Code = 2531 # type: ignore
+PSUBQ_MM_MMM64: int = 2531
 """
 ``PSUBQ mm1, mm2/m64``
 
 ``NP 0F FB /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-PSUBQ_XMM_XMMM128: Code = 2532 # type: ignore
+PSUBQ_XMM_XMMM128: int = 2532
 """
 ``PSUBQ xmm1, xmm2/m128``
 
 ``66 0F FB /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBQ_XMM_XMM_XMMM128: Code = 2533 # type: ignore
+VEX_VPSUBQ_XMM_XMM_XMMM128: int = 2533
 """
 ``VPSUBQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG FB /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSUBQ_YMM_YMM_YMMM256: Code = 2534 # type: ignore
+VEX_VPSUBQ_YMM_YMM_YMMM256: int = 2534
 """
 ``VPSUBQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG FB /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBQ_XMM_K1Z_XMM_XMMM128B64: Code = 2535 # type: ignore
+EVEX_VPSUBQ_XMM_K1Z_XMM_XMMM128B64: int = 2535
 """
 ``VPSUBQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F.W1 FB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBQ_YMM_K1Z_YMM_YMMM256B64: Code = 2536 # type: ignore
+EVEX_VPSUBQ_YMM_K1Z_YMM_YMMM256B64: int = 2536
 """
 ``VPSUBQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F.W1 FB /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSUBQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2537 # type: ignore
+EVEX_VPSUBQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2537
 """
 ``VPSUBQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F.W1 FB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PADDB_MM_MMM64: Code = 2538 # type: ignore
+PADDB_MM_MMM64: int = 2538
 """
 ``PADDB mm, mm/m64``
 
 ``NP 0F FC /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDB_XMM_XMMM128: Code = 2539 # type: ignore
+PADDB_XMM_XMMM128: int = 2539
 """
 ``PADDB xmm1, xmm2/m128``
 
 ``66 0F FC /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDB_XMM_XMM_XMMM128: Code = 2540 # type: ignore
+VEX_VPADDB_XMM_XMM_XMMM128: int = 2540
 """
 ``VPADDB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG FC /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDB_YMM_YMM_YMMM256: Code = 2541 # type: ignore
+VEX_VPADDB_YMM_YMM_YMMM256: int = 2541
 """
 ``VPADDB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG FC /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDB_XMM_K1Z_XMM_XMMM128: Code = 2542 # type: ignore
+EVEX_VPADDB_XMM_K1Z_XMM_XMMM128: int = 2542
 """
 ``VPADDB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG FC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDB_YMM_K1Z_YMM_YMMM256: Code = 2543 # type: ignore
+EVEX_VPADDB_YMM_K1Z_YMM_YMMM256: int = 2543
 """
 ``VPADDB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG FC /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDB_ZMM_K1Z_ZMM_ZMMM512: Code = 2544 # type: ignore
+EVEX_VPADDB_ZMM_K1Z_ZMM_ZMMM512: int = 2544
 """
 ``VPADDB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG FC /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PADDW_MM_MMM64: Code = 2545 # type: ignore
+PADDW_MM_MMM64: int = 2545
 """
 ``PADDW mm, mm/m64``
 
 ``NP 0F FD /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDW_XMM_XMMM128: Code = 2546 # type: ignore
+PADDW_XMM_XMMM128: int = 2546
 """
 ``PADDW xmm1, xmm2/m128``
 
 ``66 0F FD /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDW_XMM_XMM_XMMM128: Code = 2547 # type: ignore
+VEX_VPADDW_XMM_XMM_XMMM128: int = 2547
 """
 ``VPADDW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG FD /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDW_YMM_YMM_YMMM256: Code = 2548 # type: ignore
+VEX_VPADDW_YMM_YMM_YMMM256: int = 2548
 """
 ``VPADDW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG FD /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDW_XMM_K1Z_XMM_XMMM128: Code = 2549 # type: ignore
+EVEX_VPADDW_XMM_K1Z_XMM_XMMM128: int = 2549
 """
 ``VPADDW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F.WIG FD /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDW_YMM_K1Z_YMM_YMMM256: Code = 2550 # type: ignore
+EVEX_VPADDW_YMM_K1Z_YMM_YMMM256: int = 2550
 """
 ``VPADDW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F.WIG FD /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDW_ZMM_K1Z_ZMM_ZMMM512: Code = 2551 # type: ignore
+EVEX_VPADDW_ZMM_K1Z_ZMM_ZMMM512: int = 2551
 """
 ``VPADDW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F.WIG FD /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PADDD_MM_MMM64: Code = 2552 # type: ignore
+PADDD_MM_MMM64: int = 2552
 """
 ``PADDD mm, mm/m64``
 
 ``NP 0F FE /r``
 
 ``MMX``
 
 ``16/32/64-bit``
 """
-PADDD_XMM_XMMM128: Code = 2553 # type: ignore
+PADDD_XMM_XMMM128: int = 2553
 """
 ``PADDD xmm1, xmm2/m128``
 
 ``66 0F FE /r``
 
 ``SSE2``
 
 ``16/32/64-bit``
 """
-VEX_VPADDD_XMM_XMM_XMMM128: Code = 2554 # type: ignore
+VEX_VPADDD_XMM_XMM_XMMM128: int = 2554
 """
 ``VPADDD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F.WIG FE /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPADDD_YMM_YMM_YMMM256: Code = 2555 # type: ignore
+VEX_VPADDD_YMM_YMM_YMMM256: int = 2555
 """
 ``VPADDD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F.WIG FE /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDD_XMM_K1Z_XMM_XMMM128B32: Code = 2556 # type: ignore
+EVEX_VPADDD_XMM_K1Z_XMM_XMMM128B32: int = 2556
 """
 ``VPADDD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F.W0 FE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDD_YMM_K1Z_YMM_YMMM256B32: Code = 2557 # type: ignore
+EVEX_VPADDD_YMM_K1Z_YMM_YMMM256B32: int = 2557
 """
 ``VPADDD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F.W0 FE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPADDD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2558 # type: ignore
+EVEX_VPADDD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2558
 """
 ``VPADDD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F.W0 FE /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-UD0_R16_RM16: Code = 2559 # type: ignore
+UD0_R16_RM16: int = 2559
 """
 ``UD0 r16, r/m16``
 
 ``o16 0F FF /r``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-UD0_R32_RM32: Code = 2560 # type: ignore
+UD0_R32_RM32: int = 2560
 """
 ``UD0 r32, r/m32``
 
 ``o32 0F FF /r``
 
 ``386+``
 
 ``16/32/64-bit``
 """
-UD0_R64_RM64: Code = 2561 # type: ignore
+UD0_R64_RM64: int = 2561
 """
 ``UD0 r64, r/m64``
 
 ``o64 0F FF /r``
 
 ``X64``
 
 ``64-bit``
 """
-PSHUFB_MM_MMM64: Code = 2562 # type: ignore
+PSHUFB_MM_MMM64: int = 2562
 """
 ``PSHUFB mm1, mm2/m64``
 
 ``NP 0F 38 00 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PSHUFB_XMM_XMMM128: Code = 2563 # type: ignore
+PSHUFB_XMM_XMMM128: int = 2563
 """
 ``PSHUFB xmm1, xmm2/m128``
 
 ``66 0F 38 00 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFB_XMM_XMM_XMMM128: Code = 2564 # type: ignore
+VEX_VPSHUFB_XMM_XMM_XMMM128: int = 2564
 """
 ``VPSHUFB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 00 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSHUFB_YMM_YMM_YMMM256: Code = 2565 # type: ignore
+VEX_VPSHUFB_YMM_YMM_YMMM256: int = 2565
 """
 ``VPSHUFB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 00 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFB_XMM_K1Z_XMM_XMMM128: Code = 2566 # type: ignore
+EVEX_VPSHUFB_XMM_K1Z_XMM_XMMM128: int = 2566
 """
 ``VPSHUFB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 00 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFB_YMM_K1Z_YMM_YMMM256: Code = 2567 # type: ignore
+EVEX_VPSHUFB_YMM_K1Z_YMM_YMMM256: int = 2567
 """
 ``VPSHUFB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 00 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFB_ZMM_K1Z_ZMM_ZMMM512: Code = 2568 # type: ignore
+EVEX_VPSHUFB_ZMM_K1Z_ZMM_ZMMM512: int = 2568
 """
 ``VPSHUFB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 00 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PHADDW_MM_MMM64: Code = 2569 # type: ignore
+PHADDW_MM_MMM64: int = 2569
 """
 ``PHADDW mm1, mm2/m64``
 
 ``NP 0F 38 01 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHADDW_XMM_XMMM128: Code = 2570 # type: ignore
+PHADDW_XMM_XMMM128: int = 2570
 """
 ``PHADDW xmm1, xmm2/m128``
 
 ``66 0F 38 01 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDW_XMM_XMM_XMMM128: Code = 2571 # type: ignore
+VEX_VPHADDW_XMM_XMM_XMMM128: int = 2571
 """
 ``VPHADDW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 01 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDW_YMM_YMM_YMMM256: Code = 2572 # type: ignore
+VEX_VPHADDW_YMM_YMM_YMMM256: int = 2572
 """
 ``VPHADDW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 01 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PHADDD_MM_MMM64: Code = 2573 # type: ignore
+PHADDD_MM_MMM64: int = 2573
 """
 ``PHADDD mm1, mm2/m64``
 
 ``NP 0F 38 02 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHADDD_XMM_XMMM128: Code = 2574 # type: ignore
+PHADDD_XMM_XMMM128: int = 2574
 """
 ``PHADDD xmm1, xmm2/m128``
 
 ``66 0F 38 02 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDD_XMM_XMM_XMMM128: Code = 2575 # type: ignore
+VEX_VPHADDD_XMM_XMM_XMMM128: int = 2575
 """
 ``VPHADDD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 02 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDD_YMM_YMM_YMMM256: Code = 2576 # type: ignore
+VEX_VPHADDD_YMM_YMM_YMMM256: int = 2576
 """
 ``VPHADDD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 02 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PHADDSW_MM_MMM64: Code = 2577 # type: ignore
+PHADDSW_MM_MMM64: int = 2577
 """
 ``PHADDSW mm1, mm2/m64``
 
 ``NP 0F 38 03 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHADDSW_XMM_XMMM128: Code = 2578 # type: ignore
+PHADDSW_XMM_XMMM128: int = 2578
 """
 ``PHADDSW xmm1, xmm2/m128``
 
 ``66 0F 38 03 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDSW_XMM_XMM_XMMM128: Code = 2579 # type: ignore
+VEX_VPHADDSW_XMM_XMM_XMMM128: int = 2579
 """
 ``VPHADDSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 03 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHADDSW_YMM_YMM_YMMM256: Code = 2580 # type: ignore
+VEX_VPHADDSW_YMM_YMM_YMMM256: int = 2580
 """
 ``VPHADDSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 03 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PMADDUBSW_MM_MMM64: Code = 2581 # type: ignore
+PMADDUBSW_MM_MMM64: int = 2581
 """
 ``PMADDUBSW mm1, mm2/m64``
 
 ``NP 0F 38 04 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PMADDUBSW_XMM_XMMM128: Code = 2582 # type: ignore
+PMADDUBSW_XMM_XMMM128: int = 2582
 """
 ``PMADDUBSW xmm1, xmm2/m128``
 
 ``66 0F 38 04 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPMADDUBSW_XMM_XMM_XMMM128: Code = 2583 # type: ignore
+VEX_VPMADDUBSW_XMM_XMM_XMMM128: int = 2583
 """
 ``VPMADDUBSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 04 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMADDUBSW_YMM_YMM_YMMM256: Code = 2584 # type: ignore
+VEX_VPMADDUBSW_YMM_YMM_YMMM256: int = 2584
 """
 ``VPMADDUBSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 04 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDUBSW_XMM_K1Z_XMM_XMMM128: Code = 2585 # type: ignore
+EVEX_VPMADDUBSW_XMM_K1Z_XMM_XMMM128: int = 2585
 """
 ``VPMADDUBSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 04 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDUBSW_YMM_K1Z_YMM_YMMM256: Code = 2586 # type: ignore
+EVEX_VPMADDUBSW_YMM_K1Z_YMM_YMMM256: int = 2586
 """
 ``VPMADDUBSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 04 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADDUBSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2587 # type: ignore
+EVEX_VPMADDUBSW_ZMM_K1Z_ZMM_ZMMM512: int = 2587
 """
 ``VPMADDUBSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 04 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PHSUBW_MM_MMM64: Code = 2588 # type: ignore
+PHSUBW_MM_MMM64: int = 2588
 """
 ``PHSUBW mm1, mm2/m64``
 
 ``NP 0F 38 05 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHSUBW_XMM_XMMM128: Code = 2589 # type: ignore
+PHSUBW_XMM_XMMM128: int = 2589
 """
 ``PHSUBW xmm1, xmm2/m128``
 
 ``66 0F 38 05 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBW_XMM_XMM_XMMM128: Code = 2590 # type: ignore
+VEX_VPHSUBW_XMM_XMM_XMMM128: int = 2590
 """
 ``VPHSUBW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 05 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBW_YMM_YMM_YMMM256: Code = 2591 # type: ignore
+VEX_VPHSUBW_YMM_YMM_YMMM256: int = 2591
 """
 ``VPHSUBW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 05 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PHSUBD_MM_MMM64: Code = 2592 # type: ignore
+PHSUBD_MM_MMM64: int = 2592
 """
 ``PHSUBD mm1, mm2/m64``
 
 ``NP 0F 38 06 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHSUBD_XMM_XMMM128: Code = 2593 # type: ignore
+PHSUBD_XMM_XMMM128: int = 2593
 """
 ``PHSUBD xmm1, xmm2/m128``
 
 ``66 0F 38 06 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBD_XMM_XMM_XMMM128: Code = 2594 # type: ignore
+VEX_VPHSUBD_XMM_XMM_XMMM128: int = 2594
 """
 ``VPHSUBD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 06 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBD_YMM_YMM_YMMM256: Code = 2595 # type: ignore
+VEX_VPHSUBD_YMM_YMM_YMMM256: int = 2595
 """
 ``VPHSUBD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 06 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PHSUBSW_MM_MMM64: Code = 2596 # type: ignore
+PHSUBSW_MM_MMM64: int = 2596
 """
 ``PHSUBSW mm1, mm2/m64``
 
 ``NP 0F 38 07 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PHSUBSW_XMM_XMMM128: Code = 2597 # type: ignore
+PHSUBSW_XMM_XMMM128: int = 2597
 """
 ``PHSUBSW xmm1, xmm2/m128``
 
 ``66 0F 38 07 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBSW_XMM_XMM_XMMM128: Code = 2598 # type: ignore
+VEX_VPHSUBSW_XMM_XMM_XMMM128: int = 2598
 """
 ``VPHSUBSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 07 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPHSUBSW_YMM_YMM_YMMM256: Code = 2599 # type: ignore
+VEX_VPHSUBSW_YMM_YMM_YMMM256: int = 2599
 """
 ``VPHSUBSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 07 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PSIGNB_MM_MMM64: Code = 2600 # type: ignore
+PSIGNB_MM_MMM64: int = 2600
 """
 ``PSIGNB mm1, mm2/m64``
 
 ``NP 0F 38 08 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PSIGNB_XMM_XMMM128: Code = 2601 # type: ignore
+PSIGNB_XMM_XMMM128: int = 2601
 """
 ``PSIGNB xmm1, xmm2/m128``
 
 ``66 0F 38 08 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGNB_XMM_XMM_XMMM128: Code = 2602 # type: ignore
+VEX_VPSIGNB_XMM_XMM_XMMM128: int = 2602
 """
 ``VPSIGNB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 08 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGNB_YMM_YMM_YMMM256: Code = 2603 # type: ignore
+VEX_VPSIGNB_YMM_YMM_YMMM256: int = 2603
 """
 ``VPSIGNB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 08 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PSIGNW_MM_MMM64: Code = 2604 # type: ignore
+PSIGNW_MM_MMM64: int = 2604
 """
 ``PSIGNW mm1, mm2/m64``
 
 ``NP 0F 38 09 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PSIGNW_XMM_XMMM128: Code = 2605 # type: ignore
+PSIGNW_XMM_XMMM128: int = 2605
 """
 ``PSIGNW xmm1, xmm2/m128``
 
 ``66 0F 38 09 /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGNW_XMM_XMM_XMMM128: Code = 2606 # type: ignore
+VEX_VPSIGNW_XMM_XMM_XMMM128: int = 2606
 """
 ``VPSIGNW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 09 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGNW_YMM_YMM_YMMM256: Code = 2607 # type: ignore
+VEX_VPSIGNW_YMM_YMM_YMMM256: int = 2607
 """
 ``VPSIGNW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 09 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PSIGND_MM_MMM64: Code = 2608 # type: ignore
+PSIGND_MM_MMM64: int = 2608
 """
 ``PSIGND mm1, mm2/m64``
 
 ``NP 0F 38 0A /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PSIGND_XMM_XMMM128: Code = 2609 # type: ignore
+PSIGND_XMM_XMMM128: int = 2609
 """
 ``PSIGND xmm1, xmm2/m128``
 
 ``66 0F 38 0A /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGND_XMM_XMM_XMMM128: Code = 2610 # type: ignore
+VEX_VPSIGND_XMM_XMM_XMMM128: int = 2610
 """
 ``VPSIGND xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 0A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPSIGND_YMM_YMM_YMMM256: Code = 2611 # type: ignore
+VEX_VPSIGND_YMM_YMM_YMMM256: int = 2611
 """
 ``VPSIGND ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 0A /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PMULHRSW_MM_MMM64: Code = 2612 # type: ignore
+PMULHRSW_MM_MMM64: int = 2612
 """
 ``PMULHRSW mm1, mm2/m64``
 
 ``NP 0F 38 0B /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PMULHRSW_XMM_XMMM128: Code = 2613 # type: ignore
+PMULHRSW_XMM_XMMM128: int = 2613
 """
 ``PMULHRSW xmm1, xmm2/m128``
 
 ``66 0F 38 0B /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHRSW_XMM_XMM_XMMM128: Code = 2614 # type: ignore
+VEX_VPMULHRSW_XMM_XMM_XMMM128: int = 2614
 """
 ``VPMULHRSW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 0B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULHRSW_YMM_YMM_YMMM256: Code = 2615 # type: ignore
+VEX_VPMULHRSW_YMM_YMM_YMMM256: int = 2615
 """
 ``VPMULHRSW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 0B /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHRSW_XMM_K1Z_XMM_XMMM128: Code = 2616 # type: ignore
+EVEX_VPMULHRSW_XMM_K1Z_XMM_XMMM128: int = 2616
 """
 ``VPMULHRSW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 0B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHRSW_YMM_K1Z_YMM_YMMM256: Code = 2617 # type: ignore
+EVEX_VPMULHRSW_YMM_K1Z_YMM_YMMM256: int = 2617
 """
 ``VPMULHRSW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 0B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULHRSW_ZMM_K1Z_ZMM_ZMMM512: Code = 2618 # type: ignore
+EVEX_VPMULHRSW_ZMM_K1Z_ZMM_ZMMM512: int = 2618
 """
 ``VPMULHRSW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 0B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPS_XMM_XMM_XMMM128: Code = 2619 # type: ignore
+VEX_VPERMILPS_XMM_XMM_XMMM128: int = 2619
 """
 ``VPERMILPS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 0C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPS_YMM_YMM_YMMM256: Code = 2620 # type: ignore
+VEX_VPERMILPS_YMM_YMM_YMMM256: int = 2620
 """
 ``VPERMILPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 0C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_XMM_K1Z_XMM_XMMM128B32: Code = 2621 # type: ignore
+EVEX_VPERMILPS_XMM_K1Z_XMM_XMMM128B32: int = 2621
 """
 ``VPERMILPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 0C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_YMM_K1Z_YMM_YMMM256B32: Code = 2622 # type: ignore
+EVEX_VPERMILPS_YMM_K1Z_YMM_YMMM256B32: int = 2622
 """
 ``VPERMILPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 0C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2623 # type: ignore
+EVEX_VPERMILPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 2623
 """
 ``VPERMILPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 0C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPD_XMM_XMM_XMMM128: Code = 2624 # type: ignore
+VEX_VPERMILPD_XMM_XMM_XMMM128: int = 2624
 """
 ``VPERMILPD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 0D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPD_YMM_YMM_YMMM256: Code = 2625 # type: ignore
+VEX_VPERMILPD_YMM_YMM_YMMM256: int = 2625
 """
 ``VPERMILPD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 0D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_XMM_K1Z_XMM_XMMM128B64: Code = 2626 # type: ignore
+EVEX_VPERMILPD_XMM_K1Z_XMM_XMMM128B64: int = 2626
 """
 ``VPERMILPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 0D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_YMM_K1Z_YMM_YMMM256B64: Code = 2627 # type: ignore
+EVEX_VPERMILPD_YMM_K1Z_YMM_YMMM256B64: int = 2627
 """
 ``VPERMILPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 0D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2628 # type: ignore
+EVEX_VPERMILPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 2628
 """
 ``VPERMILPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 0D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VTESTPS_XMM_XMMM128: Code = 2629 # type: ignore
+VEX_VTESTPS_XMM_XMMM128: int = 2629
 """
 ``VTESTPS xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.W0 0E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VTESTPS_YMM_YMMM256: Code = 2630 # type: ignore
+VEX_VTESTPS_YMM_YMMM256: int = 2630
 """
 ``VTESTPS ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.W0 0E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VTESTPD_XMM_XMMM128: Code = 2631 # type: ignore
+VEX_VTESTPD_XMM_XMMM128: int = 2631
 """
 ``VTESTPD xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.W0 0F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VTESTPD_YMM_YMMM256: Code = 2632 # type: ignore
+VEX_VTESTPD_YMM_YMMM256: int = 2632
 """
 ``VTESTPD ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.W0 0F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PBLENDVB_XMM_XMMM128: Code = 2633 # type: ignore
+PBLENDVB_XMM_XMMM128: int = 2633
 """
 ``PBLENDVB xmm1, xmm2/m128, <XMM0>``
 
 ``66 0F 38 10 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVW_XMM_K1Z_XMM_XMMM128: Code = 2634 # type: ignore
+EVEX_VPSRLVW_XMM_K1Z_XMM_XMMM128: int = 2634
 """
 ``VPSRLVW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 10 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVW_YMM_K1Z_YMM_YMMM256: Code = 2635 # type: ignore
+EVEX_VPSRLVW_YMM_K1Z_YMM_YMMM256: int = 2635
 """
 ``VPSRLVW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 10 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVW_ZMM_K1Z_ZMM_ZMMM512: Code = 2636 # type: ignore
+EVEX_VPSRLVW_ZMM_K1Z_ZMM_ZMMM512: int = 2636
 """
 ``VPSRLVW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 10 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSWB_XMMM64_K1Z_XMM: Code = 2637 # type: ignore
+EVEX_VPMOVUSWB_XMMM64_K1Z_XMM: int = 2637
 """
 ``VPMOVUSWB xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 10 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSWB_XMMM128_K1Z_YMM: Code = 2638 # type: ignore
+EVEX_VPMOVUSWB_XMMM128_K1Z_YMM: int = 2638
 """
 ``VPMOVUSWB xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 10 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSWB_YMMM256_K1Z_ZMM: Code = 2639 # type: ignore
+EVEX_VPMOVUSWB_YMMM256_K1Z_ZMM: int = 2639
 """
 ``VPMOVUSWB ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 10 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVW_XMM_K1Z_XMM_XMMM128: Code = 2640 # type: ignore
+EVEX_VPSRAVW_XMM_K1Z_XMM_XMMM128: int = 2640
 """
 ``VPSRAVW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 11 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVW_YMM_K1Z_YMM_YMMM256: Code = 2641 # type: ignore
+EVEX_VPSRAVW_YMM_K1Z_YMM_YMMM256: int = 2641
 """
 ``VPSRAVW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 11 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVW_ZMM_K1Z_ZMM_ZMMM512: Code = 2642 # type: ignore
+EVEX_VPSRAVW_ZMM_K1Z_ZMM_ZMMM512: int = 2642
 """
 ``VPSRAVW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 11 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDB_XMMM32_K1Z_XMM: Code = 2643 # type: ignore
+EVEX_VPMOVUSDB_XMMM32_K1Z_XMM: int = 2643
 """
 ``VPMOVUSDB xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDB_XMMM64_K1Z_YMM: Code = 2644 # type: ignore
+EVEX_VPMOVUSDB_XMMM64_K1Z_YMM: int = 2644
 """
 ``VPMOVUSDB xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 11 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDB_XMMM128_K1Z_ZMM: Code = 2645 # type: ignore
+EVEX_VPMOVUSDB_XMMM128_K1Z_ZMM: int = 2645
 """
 ``VPMOVUSDB xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 11 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVW_XMM_K1Z_XMM_XMMM128: Code = 2646 # type: ignore
+EVEX_VPSLLVW_XMM_K1Z_XMM_XMMM128: int = 2646
 """
 ``VPSLLVW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 12 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVW_YMM_K1Z_YMM_YMMM256: Code = 2647 # type: ignore
+EVEX_VPSLLVW_YMM_K1Z_YMM_YMMM256: int = 2647
 """
 ``VPSLLVW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 12 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVW_ZMM_K1Z_ZMM_ZMMM512: Code = 2648 # type: ignore
+EVEX_VPSLLVW_ZMM_K1Z_ZMM_ZMMM512: int = 2648
 """
 ``VPSLLVW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 12 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQB_XMMM16_K1Z_XMM: Code = 2649 # type: ignore
+EVEX_VPMOVUSQB_XMMM16_K1Z_XMM: int = 2649
 """
 ``VPMOVUSQB xmm1/m16 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQB_XMMM32_K1Z_YMM: Code = 2650 # type: ignore
+EVEX_VPMOVUSQB_XMMM32_K1Z_YMM: int = 2650
 """
 ``VPMOVUSQB xmm1/m32 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 12 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQB_XMMM64_K1Z_ZMM: Code = 2651 # type: ignore
+EVEX_VPMOVUSQB_XMMM64_K1Z_ZMM: int = 2651
 """
 ``VPMOVUSQB xmm1/m64 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 12 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPH2PS_XMM_XMMM64: Code = 2652 # type: ignore
+VEX_VCVTPH2PS_XMM_XMMM64: int = 2652
 """
 ``VCVTPH2PS xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.W0 13 /r``
 
 ``F16C``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPH2PS_YMM_XMMM128: Code = 2653 # type: ignore
+VEX_VCVTPH2PS_YMM_XMMM128: int = 2653
 """
 ``VCVTPH2PS ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.W0 13 /r``
 
 ``F16C``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPH2PS_XMM_K1Z_XMMM64: Code = 2654 # type: ignore
+EVEX_VCVTPH2PS_XMM_K1Z_XMMM64: int = 2654
 """
 ``VCVTPH2PS xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.W0 13 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPH2PS_YMM_K1Z_XMMM128: Code = 2655 # type: ignore
+EVEX_VCVTPH2PS_YMM_K1Z_XMMM128: int = 2655
 """
 ``VCVTPH2PS ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.W0 13 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPH2PS_ZMM_K1Z_YMMM256_SAE: Code = 2656 # type: ignore
+EVEX_VCVTPH2PS_ZMM_K1Z_YMMM256_SAE: int = 2656
 """
 ``VCVTPH2PS zmm1 {k1}{z}, ymm2/m256{sae}``
 
 ``EVEX.512.66.0F38.W0 13 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDW_XMMM64_K1Z_XMM: Code = 2657 # type: ignore
+EVEX_VPMOVUSDW_XMMM64_K1Z_XMM: int = 2657
 """
 ``VPMOVUSDW xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 13 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDW_XMMM128_K1Z_YMM: Code = 2658 # type: ignore
+EVEX_VPMOVUSDW_XMMM128_K1Z_YMM: int = 2658
 """
 ``VPMOVUSDW xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 13 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSDW_YMMM256_K1Z_ZMM: Code = 2659 # type: ignore
+EVEX_VPMOVUSDW_YMMM256_K1Z_ZMM: int = 2659
 """
 ``VPMOVUSDW ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 13 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-BLENDVPS_XMM_XMMM128: Code = 2660 # type: ignore
+BLENDVPS_XMM_XMMM128: int = 2660
 """
 ``BLENDVPS xmm1, xmm2/m128, <XMM0>``
 
 ``66 0F 38 14 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVD_XMM_K1Z_XMM_XMMM128B32: Code = 2661 # type: ignore
+EVEX_VPRORVD_XMM_K1Z_XMM_XMMM128B32: int = 2661
 """
 ``VPRORVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVD_YMM_K1Z_YMM_YMMM256B32: Code = 2662 # type: ignore
+EVEX_VPRORVD_YMM_K1Z_YMM_YMMM256B32: int = 2662
 """
 ``VPRORVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2663 # type: ignore
+EVEX_VPRORVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2663
 """
 ``VPRORVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 14 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVQ_XMM_K1Z_XMM_XMMM128B64: Code = 2664 # type: ignore
+EVEX_VPRORVQ_XMM_K1Z_XMM_XMMM128B64: int = 2664
 """
 ``VPRORVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVQ_YMM_K1Z_YMM_YMMM256B64: Code = 2665 # type: ignore
+EVEX_VPRORVQ_YMM_K1Z_YMM_YMMM256B64: int = 2665
 """
 ``VPRORVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPRORVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2666 # type: ignore
+EVEX_VPRORVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2666
 """
 ``VPRORVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 14 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQW_XMMM32_K1Z_XMM: Code = 2667 # type: ignore
+EVEX_VPMOVUSQW_XMMM32_K1Z_XMM: int = 2667
 """
 ``VPMOVUSQW xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQW_XMMM64_K1Z_YMM: Code = 2668 # type: ignore
+EVEX_VPMOVUSQW_XMMM64_K1Z_YMM: int = 2668
 """
 ``VPMOVUSQW xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 14 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQW_XMMM128_K1Z_ZMM: Code = 2669 # type: ignore
+EVEX_VPMOVUSQW_XMMM128_K1Z_ZMM: int = 2669
 """
 ``VPMOVUSQW xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 14 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-BLENDVPD_XMM_XMMM128: Code = 2670 # type: ignore
+BLENDVPD_XMM_XMMM128: int = 2670
 """
 ``BLENDVPD xmm1, xmm2/m128, <XMM0>``
 
 ``66 0F 38 15 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVD_XMM_K1Z_XMM_XMMM128B32: Code = 2671 # type: ignore
+EVEX_VPROLVD_XMM_K1Z_XMM_XMMM128B32: int = 2671
 """
 ``VPROLVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVD_YMM_K1Z_YMM_YMMM256B32: Code = 2672 # type: ignore
+EVEX_VPROLVD_YMM_K1Z_YMM_YMMM256B32: int = 2672
 """
 ``VPROLVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2673 # type: ignore
+EVEX_VPROLVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2673
 """
 ``VPROLVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 15 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVQ_XMM_K1Z_XMM_XMMM128B64: Code = 2674 # type: ignore
+EVEX_VPROLVQ_XMM_K1Z_XMM_XMMM128B64: int = 2674
 """
 ``VPROLVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVQ_YMM_K1Z_YMM_YMMM256B64: Code = 2675 # type: ignore
+EVEX_VPROLVQ_YMM_K1Z_YMM_YMMM256B64: int = 2675
 """
 ``VPROLVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPROLVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2676 # type: ignore
+EVEX_VPROLVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2676
 """
 ``VPROLVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 15 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQD_XMMM64_K1Z_XMM: Code = 2677 # type: ignore
+EVEX_VPMOVUSQD_XMMM64_K1Z_XMM: int = 2677
 """
 ``VPMOVUSQD xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQD_XMMM128_K1Z_YMM: Code = 2678 # type: ignore
+EVEX_VPMOVUSQD_XMMM128_K1Z_YMM: int = 2678
 """
 ``VPMOVUSQD xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 15 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVUSQD_YMMM256_K1Z_ZMM: Code = 2679 # type: ignore
+EVEX_VPMOVUSQD_YMMM256_K1Z_ZMM: int = 2679
 """
 ``VPMOVUSQD ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 15 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMPS_YMM_YMM_YMMM256: Code = 2680 # type: ignore
+VEX_VPERMPS_YMM_YMM_YMMM256: int = 2680
 """
 ``VPERMPS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 16 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPS_YMM_K1Z_YMM_YMMM256B32: Code = 2681 # type: ignore
+EVEX_VPERMPS_YMM_K1Z_YMM_YMMM256B32: int = 2681
 """
 ``VPERMPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 16 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2682 # type: ignore
+EVEX_VPERMPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 2682
 """
 ``VPERMPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPD_YMM_K1Z_YMM_YMMM256B64: Code = 2683 # type: ignore
+EVEX_VPERMPD_YMM_K1Z_YMM_YMMM256B64: int = 2683
 """
 ``VPERMPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 16 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2684 # type: ignore
+EVEX_VPERMPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 2684
 """
 ``VPERMPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 16 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PTEST_XMM_XMMM128: Code = 2685 # type: ignore
+PTEST_XMM_XMMM128: int = 2685
 """
 ``PTEST xmm1, xmm2/m128``
 
 ``66 0F 38 17 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPTEST_XMM_XMMM128: Code = 2686 # type: ignore
+VEX_VPTEST_XMM_XMMM128: int = 2686
 """
 ``VPTEST xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG 17 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPTEST_YMM_YMMM256: Code = 2687 # type: ignore
+VEX_VPTEST_YMM_YMMM256: int = 2687
 """
 ``VPTEST ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.WIG 17 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSS_XMM_M32: Code = 2688 # type: ignore
+VEX_VBROADCASTSS_XMM_M32: int = 2688
 """
 ``VBROADCASTSS xmm1, m32``
 
 ``VEX.128.66.0F38.W0 18 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSS_YMM_M32: Code = 2689 # type: ignore
+VEX_VBROADCASTSS_YMM_M32: int = 2689
 """
 ``VBROADCASTSS ymm1, m32``
 
 ``VEX.256.66.0F38.W0 18 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTSS_XMM_K1Z_XMMM32: Code = 2690 # type: ignore
+EVEX_VBROADCASTSS_XMM_K1Z_XMMM32: int = 2690
 """
 ``VBROADCASTSS xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.W0 18 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTSS_YMM_K1Z_XMMM32: Code = 2691 # type: ignore
+EVEX_VBROADCASTSS_YMM_K1Z_XMMM32: int = 2691
 """
 ``VBROADCASTSS ymm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.256.66.0F38.W0 18 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTSS_ZMM_K1Z_XMMM32: Code = 2692 # type: ignore
+EVEX_VBROADCASTSS_ZMM_K1Z_XMMM32: int = 2692
 """
 ``VBROADCASTSS zmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.512.66.0F38.W0 18 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSD_YMM_M64: Code = 2693 # type: ignore
+VEX_VBROADCASTSD_YMM_M64: int = 2693
 """
 ``VBROADCASTSD ymm1, m64``
 
 ``VEX.256.66.0F38.W0 19 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF32X2_YMM_K1Z_XMMM64: Code = 2694 # type: ignore
+EVEX_VBROADCASTF32X2_YMM_K1Z_XMMM64: int = 2694
 """
 ``VBROADCASTF32X2 ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.W0 19 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF32X2_ZMM_K1Z_XMMM64: Code = 2695 # type: ignore
+EVEX_VBROADCASTF32X2_ZMM_K1Z_XMMM64: int = 2695
 """
 ``VBROADCASTF32X2 zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.W0 19 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTSD_YMM_K1Z_XMMM64: Code = 2696 # type: ignore
+EVEX_VBROADCASTSD_YMM_K1Z_XMMM64: int = 2696
 """
 ``VBROADCASTSD ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.W1 19 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTSD_ZMM_K1Z_XMMM64: Code = 2697 # type: ignore
+EVEX_VBROADCASTSD_ZMM_K1Z_XMMM64: int = 2697
 """
 ``VBROADCASTSD zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.W1 19 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTF128_YMM_M128: Code = 2698 # type: ignore
+VEX_VBROADCASTF128_YMM_M128: int = 2698
 """
 ``VBROADCASTF128 ymm1, m128``
 
 ``VEX.256.66.0F38.W0 1A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF32X4_YMM_K1Z_M128: Code = 2699 # type: ignore
+EVEX_VBROADCASTF32X4_YMM_K1Z_M128: int = 2699
 """
 ``VBROADCASTF32X4 ymm1 {k1}{z}, m128``
 
 ``EVEX.256.66.0F38.W0 1A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF32X4_ZMM_K1Z_M128: Code = 2700 # type: ignore
+EVEX_VBROADCASTF32X4_ZMM_K1Z_M128: int = 2700
 """
 ``VBROADCASTF32X4 zmm1 {k1}{z}, m128``
 
 ``EVEX.512.66.0F38.W0 1A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF64X2_YMM_K1Z_M128: Code = 2701 # type: ignore
+EVEX_VBROADCASTF64X2_YMM_K1Z_M128: int = 2701
 """
 ``VBROADCASTF64X2 ymm1 {k1}{z}, m128``
 
 ``EVEX.256.66.0F38.W1 1A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF64X2_ZMM_K1Z_M128: Code = 2702 # type: ignore
+EVEX_VBROADCASTF64X2_ZMM_K1Z_M128: int = 2702
 """
 ``VBROADCASTF64X2 zmm1 {k1}{z}, m128``
 
 ``EVEX.512.66.0F38.W1 1A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF32X8_ZMM_K1Z_M256: Code = 2703 # type: ignore
+EVEX_VBROADCASTF32X8_ZMM_K1Z_M256: int = 2703
 """
 ``VBROADCASTF32X8 zmm1 {k1}{z}, m256``
 
 ``EVEX.512.66.0F38.W0 1B /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTF64X4_ZMM_K1Z_M256: Code = 2704 # type: ignore
+EVEX_VBROADCASTF64X4_ZMM_K1Z_M256: int = 2704
 """
 ``VBROADCASTF64X4 zmm1 {k1}{z}, m256``
 
 ``EVEX.512.66.0F38.W1 1B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PABSB_MM_MMM64: Code = 2705 # type: ignore
+PABSB_MM_MMM64: int = 2705
 """
 ``PABSB mm1, mm2/m64``
 
 ``NP 0F 38 1C /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PABSB_XMM_XMMM128: Code = 2706 # type: ignore
+PABSB_XMM_XMMM128: int = 2706
 """
 ``PABSB xmm1, xmm2/m128``
 
 ``66 0F 38 1C /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPABSB_XMM_XMMM128: Code = 2707 # type: ignore
+VEX_VPABSB_XMM_XMMM128: int = 2707
 """
 ``VPABSB xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG 1C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPABSB_YMM_YMMM256: Code = 2708 # type: ignore
+VEX_VPABSB_YMM_YMMM256: int = 2708
 """
 ``VPABSB ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.WIG 1C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSB_XMM_K1Z_XMMM128: Code = 2709 # type: ignore
+EVEX_VPABSB_XMM_K1Z_XMMM128: int = 2709
 """
 ``VPABSB xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.WIG 1C /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSB_YMM_K1Z_YMMM256: Code = 2710 # type: ignore
+EVEX_VPABSB_YMM_K1Z_YMMM256: int = 2710
 """
 ``VPABSB ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.WIG 1C /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSB_ZMM_K1Z_ZMMM512: Code = 2711 # type: ignore
+EVEX_VPABSB_ZMM_K1Z_ZMMM512: int = 2711
 """
 ``VPABSB zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.WIG 1C /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PABSW_MM_MMM64: Code = 2712 # type: ignore
+PABSW_MM_MMM64: int = 2712
 """
 ``PABSW mm1, mm2/m64``
 
 ``NP 0F 38 1D /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PABSW_XMM_XMMM128: Code = 2713 # type: ignore
+PABSW_XMM_XMMM128: int = 2713
 """
 ``PABSW xmm1, xmm2/m128``
 
 ``66 0F 38 1D /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPABSW_XMM_XMMM128: Code = 2714 # type: ignore
+VEX_VPABSW_XMM_XMMM128: int = 2714
 """
 ``VPABSW xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG 1D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPABSW_YMM_YMMM256: Code = 2715 # type: ignore
+VEX_VPABSW_YMM_YMMM256: int = 2715
 """
 ``VPABSW ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.WIG 1D /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSW_XMM_K1Z_XMMM128: Code = 2716 # type: ignore
+EVEX_VPABSW_XMM_K1Z_XMMM128: int = 2716
 """
 ``VPABSW xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.WIG 1D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSW_YMM_K1Z_YMMM256: Code = 2717 # type: ignore
+EVEX_VPABSW_YMM_K1Z_YMMM256: int = 2717
 """
 ``VPABSW ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.WIG 1D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSW_ZMM_K1Z_ZMMM512: Code = 2718 # type: ignore
+EVEX_VPABSW_ZMM_K1Z_ZMMM512: int = 2718
 """
 ``VPABSW zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.WIG 1D /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PABSD_MM_MMM64: Code = 2719 # type: ignore
+PABSD_MM_MMM64: int = 2719
 """
 ``PABSD mm1, mm2/m64``
 
 ``NP 0F 38 1E /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PABSD_XMM_XMMM128: Code = 2720 # type: ignore
+PABSD_XMM_XMMM128: int = 2720
 """
 ``PABSD xmm1, xmm2/m128``
 
 ``66 0F 38 1E /r``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPABSD_XMM_XMMM128: Code = 2721 # type: ignore
+VEX_VPABSD_XMM_XMMM128: int = 2721
 """
 ``VPABSD xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG 1E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPABSD_YMM_YMMM256: Code = 2722 # type: ignore
+VEX_VPABSD_YMM_YMMM256: int = 2722
 """
 ``VPABSD ymm1, ymm2/m256``
 
 ``VEX.256.66.0F38.WIG 1E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSD_XMM_K1Z_XMMM128B32: Code = 2723 # type: ignore
+EVEX_VPABSD_XMM_K1Z_XMMM128B32: int = 2723
 """
 ``VPABSD xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 1E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSD_YMM_K1Z_YMMM256B32: Code = 2724 # type: ignore
+EVEX_VPABSD_YMM_K1Z_YMMM256B32: int = 2724
 """
 ``VPABSD ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 1E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSD_ZMM_K1Z_ZMMM512B32: Code = 2725 # type: ignore
+EVEX_VPABSD_ZMM_K1Z_ZMMM512B32: int = 2725
 """
 ``VPABSD zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 1E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSQ_XMM_K1Z_XMMM128B64: Code = 2726 # type: ignore
+EVEX_VPABSQ_XMM_K1Z_XMMM128B64: int = 2726
 """
 ``VPABSQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 1F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSQ_YMM_K1Z_YMMM256B64: Code = 2727 # type: ignore
+EVEX_VPABSQ_YMM_K1Z_YMMM256B64: int = 2727
 """
 ``VPABSQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 1F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPABSQ_ZMM_K1Z_ZMMM512B64: Code = 2728 # type: ignore
+EVEX_VPABSQ_ZMM_K1Z_ZMMM512B64: int = 2728
 """
 ``VPABSQ zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 1F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVSXBW_XMM_XMMM64: Code = 2729 # type: ignore
+PMOVSXBW_XMM_XMMM64: int = 2729
 """
 ``PMOVSXBW xmm1, xmm2/m64``
 
 ``66 0F 38 20 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBW_XMM_XMMM64: Code = 2730 # type: ignore
+VEX_VPMOVSXBW_XMM_XMMM64: int = 2730
 """
 ``VPMOVSXBW xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 20 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBW_YMM_XMMM128: Code = 2731 # type: ignore
+VEX_VPMOVSXBW_YMM_XMMM128: int = 2731
 """
 ``VPMOVSXBW ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 20 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBW_XMM_K1Z_XMMM64: Code = 2732 # type: ignore
+EVEX_VPMOVSXBW_XMM_K1Z_XMMM64: int = 2732
 """
 ``VPMOVSXBW xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.WIG 20 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBW_YMM_K1Z_XMMM128: Code = 2733 # type: ignore
+EVEX_VPMOVSXBW_YMM_K1Z_XMMM128: int = 2733
 """
 ``VPMOVSXBW ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.WIG 20 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBW_ZMM_K1Z_YMMM256: Code = 2734 # type: ignore
+EVEX_VPMOVSXBW_ZMM_K1Z_YMMM256: int = 2734
 """
 ``VPMOVSXBW zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.WIG 20 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSWB_XMMM64_K1Z_XMM: Code = 2735 # type: ignore
+EVEX_VPMOVSWB_XMMM64_K1Z_XMM: int = 2735
 """
 ``VPMOVSWB xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 20 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSWB_XMMM128_K1Z_YMM: Code = 2736 # type: ignore
+EVEX_VPMOVSWB_XMMM128_K1Z_YMM: int = 2736
 """
 ``VPMOVSWB xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 20 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSWB_YMMM256_K1Z_ZMM: Code = 2737 # type: ignore
+EVEX_VPMOVSWB_YMMM256_K1Z_ZMM: int = 2737
 """
 ``VPMOVSWB ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 20 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMOVSXBD_XMM_XMMM32: Code = 2738 # type: ignore
+PMOVSXBD_XMM_XMMM32: int = 2738
 """
 ``PMOVSXBD xmm1, xmm2/m32``
 
 ``66 0F 38 21 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBD_XMM_XMMM32: Code = 2739 # type: ignore
+VEX_VPMOVSXBD_XMM_XMMM32: int = 2739
 """
 ``VPMOVSXBD xmm1, xmm2/m32``
 
 ``VEX.128.66.0F38.WIG 21 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBD_YMM_XMMM64: Code = 2740 # type: ignore
+VEX_VPMOVSXBD_YMM_XMMM64: int = 2740
 """
 ``VPMOVSXBD ymm1, xmm2/m64``
 
 ``VEX.256.66.0F38.WIG 21 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBD_XMM_K1Z_XMMM32: Code = 2741 # type: ignore
+EVEX_VPMOVSXBD_XMM_K1Z_XMMM32: int = 2741
 """
 ``VPMOVSXBD xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.WIG 21 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBD_YMM_K1Z_XMMM64: Code = 2742 # type: ignore
+EVEX_VPMOVSXBD_YMM_K1Z_XMMM64: int = 2742
 """
 ``VPMOVSXBD ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.WIG 21 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBD_ZMM_K1Z_XMMM128: Code = 2743 # type: ignore
+EVEX_VPMOVSXBD_ZMM_K1Z_XMMM128: int = 2743
 """
 ``VPMOVSXBD zmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.512.66.0F38.WIG 21 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDB_XMMM32_K1Z_XMM: Code = 2744 # type: ignore
+EVEX_VPMOVSDB_XMMM32_K1Z_XMM: int = 2744
 """
 ``VPMOVSDB xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 21 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDB_XMMM64_K1Z_YMM: Code = 2745 # type: ignore
+EVEX_VPMOVSDB_XMMM64_K1Z_YMM: int = 2745
 """
 ``VPMOVSDB xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 21 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDB_XMMM128_K1Z_ZMM: Code = 2746 # type: ignore
+EVEX_VPMOVSDB_XMMM128_K1Z_ZMM: int = 2746
 """
 ``VPMOVSDB xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 21 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVSXBQ_XMM_XMMM16: Code = 2747 # type: ignore
+PMOVSXBQ_XMM_XMMM16: int = 2747
 """
 ``PMOVSXBQ xmm1, xmm2/m16``
 
 ``66 0F 38 22 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBQ_XMM_XMMM16: Code = 2748 # type: ignore
+VEX_VPMOVSXBQ_XMM_XMMM16: int = 2748
 """
 ``VPMOVSXBQ xmm1, xmm2/m16``
 
 ``VEX.128.66.0F38.WIG 22 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXBQ_YMM_XMMM32: Code = 2749 # type: ignore
+VEX_VPMOVSXBQ_YMM_XMMM32: int = 2749
 """
 ``VPMOVSXBQ ymm1, xmm2/m32``
 
 ``VEX.256.66.0F38.WIG 22 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBQ_XMM_K1Z_XMMM16: Code = 2750 # type: ignore
+EVEX_VPMOVSXBQ_XMM_K1Z_XMMM16: int = 2750
 """
 ``VPMOVSXBQ xmm1 {k1}{z}, xmm2/m16``
 
 ``EVEX.128.66.0F38.WIG 22 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBQ_YMM_K1Z_XMMM32: Code = 2751 # type: ignore
+EVEX_VPMOVSXBQ_YMM_K1Z_XMMM32: int = 2751
 """
 ``VPMOVSXBQ ymm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.256.66.0F38.WIG 22 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXBQ_ZMM_K1Z_XMMM64: Code = 2752 # type: ignore
+EVEX_VPMOVSXBQ_ZMM_K1Z_XMMM64: int = 2752
 """
 ``VPMOVSXBQ zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.WIG 22 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQB_XMMM16_K1Z_XMM: Code = 2753 # type: ignore
+EVEX_VPMOVSQB_XMMM16_K1Z_XMM: int = 2753
 """
 ``VPMOVSQB xmm1/m16 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 22 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQB_XMMM32_K1Z_YMM: Code = 2754 # type: ignore
+EVEX_VPMOVSQB_XMMM32_K1Z_YMM: int = 2754
 """
 ``VPMOVSQB xmm1/m32 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 22 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQB_XMMM64_K1Z_ZMM: Code = 2755 # type: ignore
+EVEX_VPMOVSQB_XMMM64_K1Z_ZMM: int = 2755
 """
 ``VPMOVSQB xmm1/m64 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 22 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVSXWD_XMM_XMMM64: Code = 2756 # type: ignore
+PMOVSXWD_XMM_XMMM64: int = 2756
 """
 ``PMOVSXWD xmm1, xmm2/m64``
 
 ``66 0F 38 23 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXWD_XMM_XMMM64: Code = 2757 # type: ignore
+VEX_VPMOVSXWD_XMM_XMMM64: int = 2757
 """
 ``VPMOVSXWD xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 23 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXWD_YMM_XMMM128: Code = 2758 # type: ignore
+VEX_VPMOVSXWD_YMM_XMMM128: int = 2758
 """
 ``VPMOVSXWD ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 23 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWD_XMM_K1Z_XMMM64: Code = 2759 # type: ignore
+EVEX_VPMOVSXWD_XMM_K1Z_XMMM64: int = 2759
 """
 ``VPMOVSXWD xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.WIG 23 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWD_YMM_K1Z_XMMM128: Code = 2760 # type: ignore
+EVEX_VPMOVSXWD_YMM_K1Z_XMMM128: int = 2760
 """
 ``VPMOVSXWD ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.WIG 23 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWD_ZMM_K1Z_YMMM256: Code = 2761 # type: ignore
+EVEX_VPMOVSXWD_ZMM_K1Z_YMMM256: int = 2761
 """
 ``VPMOVSXWD zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.WIG 23 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDW_XMMM64_K1Z_XMM: Code = 2762 # type: ignore
+EVEX_VPMOVSDW_XMMM64_K1Z_XMM: int = 2762
 """
 ``VPMOVSDW xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 23 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDW_XMMM128_K1Z_YMM: Code = 2763 # type: ignore
+EVEX_VPMOVSDW_XMMM128_K1Z_YMM: int = 2763
 """
 ``VPMOVSDW xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 23 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSDW_YMMM256_K1Z_ZMM: Code = 2764 # type: ignore
+EVEX_VPMOVSDW_YMMM256_K1Z_ZMM: int = 2764
 """
 ``VPMOVSDW ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 23 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVSXWQ_XMM_XMMM32: Code = 2765 # type: ignore
+PMOVSXWQ_XMM_XMMM32: int = 2765
 """
 ``PMOVSXWQ xmm1, xmm2/m32``
 
 ``66 0F 38 24 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXWQ_XMM_XMMM32: Code = 2766 # type: ignore
+VEX_VPMOVSXWQ_XMM_XMMM32: int = 2766
 """
 ``VPMOVSXWQ xmm1, xmm2/m32``
 
 ``VEX.128.66.0F38.WIG 24 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXWQ_YMM_XMMM64: Code = 2767 # type: ignore
+VEX_VPMOVSXWQ_YMM_XMMM64: int = 2767
 """
 ``VPMOVSXWQ ymm1, xmm2/m64``
 
 ``VEX.256.66.0F38.WIG 24 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWQ_XMM_K1Z_XMMM32: Code = 2768 # type: ignore
+EVEX_VPMOVSXWQ_XMM_K1Z_XMMM32: int = 2768
 """
 ``VPMOVSXWQ xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.WIG 24 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWQ_YMM_K1Z_XMMM64: Code = 2769 # type: ignore
+EVEX_VPMOVSXWQ_YMM_K1Z_XMMM64: int = 2769
 """
 ``VPMOVSXWQ ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.WIG 24 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXWQ_ZMM_K1Z_XMMM128: Code = 2770 # type: ignore
+EVEX_VPMOVSXWQ_ZMM_K1Z_XMMM128: int = 2770
 """
 ``VPMOVSXWQ zmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.512.66.0F38.WIG 24 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQW_XMMM32_K1Z_XMM: Code = 2771 # type: ignore
+EVEX_VPMOVSQW_XMMM32_K1Z_XMM: int = 2771
 """
 ``VPMOVSQW xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 24 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQW_XMMM64_K1Z_YMM: Code = 2772 # type: ignore
+EVEX_VPMOVSQW_XMMM64_K1Z_YMM: int = 2772
 """
 ``VPMOVSQW xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 24 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQW_XMMM128_K1Z_ZMM: Code = 2773 # type: ignore
+EVEX_VPMOVSQW_XMMM128_K1Z_ZMM: int = 2773
 """
 ``VPMOVSQW xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 24 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVSXDQ_XMM_XMMM64: Code = 2774 # type: ignore
+PMOVSXDQ_XMM_XMMM64: int = 2774
 """
 ``PMOVSXDQ xmm1, xmm2/m64``
 
 ``66 0F 38 25 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXDQ_XMM_XMMM64: Code = 2775 # type: ignore
+VEX_VPMOVSXDQ_XMM_XMMM64: int = 2775
 """
 ``VPMOVSXDQ xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 25 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVSXDQ_YMM_XMMM128: Code = 2776 # type: ignore
+VEX_VPMOVSXDQ_YMM_XMMM128: int = 2776
 """
 ``VPMOVSXDQ ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 25 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXDQ_XMM_K1Z_XMMM64: Code = 2777 # type: ignore
+EVEX_VPMOVSXDQ_XMM_K1Z_XMMM64: int = 2777
 """
 ``VPMOVSXDQ xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.W0 25 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXDQ_YMM_K1Z_XMMM128: Code = 2778 # type: ignore
+EVEX_VPMOVSXDQ_YMM_K1Z_XMMM128: int = 2778
 """
 ``VPMOVSXDQ ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.W0 25 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSXDQ_ZMM_K1Z_YMMM256: Code = 2779 # type: ignore
+EVEX_VPMOVSXDQ_ZMM_K1Z_YMMM256: int = 2779
 """
 ``VPMOVSXDQ zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.W0 25 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQD_XMMM64_K1Z_XMM: Code = 2780 # type: ignore
+EVEX_VPMOVSQD_XMMM64_K1Z_XMM: int = 2780
 """
 ``VPMOVSQD xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 25 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQD_XMMM128_K1Z_YMM: Code = 2781 # type: ignore
+EVEX_VPMOVSQD_XMMM128_K1Z_YMM: int = 2781
 """
 ``VPMOVSQD xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 25 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVSQD_YMMM256_K1Z_ZMM: Code = 2782 # type: ignore
+EVEX_VPMOVSQD_YMMM256_K1Z_ZMM: int = 2782
 """
 ``VPMOVSQD ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 25 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMB_KR_K1_XMM_XMMM128: Code = 2783 # type: ignore
+EVEX_VPTESTMB_KR_K1_XMM_XMMM128: int = 2783
 """
 ``VPTESTMB k2 {k1}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMB_KR_K1_YMM_YMMM256: Code = 2784 # type: ignore
+EVEX_VPTESTMB_KR_K1_YMM_YMMM256: int = 2784
 """
 ``VPTESTMB k2 {k1}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMB_KR_K1_ZMM_ZMMM512: Code = 2785 # type: ignore
+EVEX_VPTESTMB_KR_K1_ZMM_ZMMM512: int = 2785
 """
 ``VPTESTMB k2 {k1}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 26 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMW_KR_K1_XMM_XMMM128: Code = 2786 # type: ignore
+EVEX_VPTESTMW_KR_K1_XMM_XMMM128: int = 2786
 """
 ``VPTESTMW k2 {k1}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMW_KR_K1_YMM_YMMM256: Code = 2787 # type: ignore
+EVEX_VPTESTMW_KR_K1_YMM_YMMM256: int = 2787
 """
 ``VPTESTMW k2 {k1}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMW_KR_K1_ZMM_ZMMM512: Code = 2788 # type: ignore
+EVEX_VPTESTMW_KR_K1_ZMM_ZMMM512: int = 2788
 """
 ``VPTESTMW k2 {k1}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 26 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMB_KR_K1_XMM_XMMM128: Code = 2789 # type: ignore
+EVEX_VPTESTNMB_KR_K1_XMM_XMMM128: int = 2789
 """
 ``VPTESTNMB k2 {k1}, xmm2, xmm3/m128``
 
 ``EVEX.128.F3.0F38.W0 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMB_KR_K1_YMM_YMMM256: Code = 2790 # type: ignore
+EVEX_VPTESTNMB_KR_K1_YMM_YMMM256: int = 2790
 """
 ``VPTESTNMB k2 {k1}, ymm2, ymm3/m256``
 
 ``EVEX.256.F3.0F38.W0 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMB_KR_K1_ZMM_ZMMM512: Code = 2791 # type: ignore
+EVEX_VPTESTNMB_KR_K1_ZMM_ZMMM512: int = 2791
 """
 ``VPTESTNMB k2 {k1}, zmm2, zmm3/m512``
 
 ``EVEX.512.F3.0F38.W0 26 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMW_KR_K1_XMM_XMMM128: Code = 2792 # type: ignore
+EVEX_VPTESTNMW_KR_K1_XMM_XMMM128: int = 2792
 """
 ``VPTESTNMW k2 {k1}, xmm2, xmm3/m128``
 
 ``EVEX.128.F3.0F38.W1 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMW_KR_K1_YMM_YMMM256: Code = 2793 # type: ignore
+EVEX_VPTESTNMW_KR_K1_YMM_YMMM256: int = 2793
 """
 ``VPTESTNMW k2 {k1}, ymm2, ymm3/m256``
 
 ``EVEX.256.F3.0F38.W1 26 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMW_KR_K1_ZMM_ZMMM512: Code = 2794 # type: ignore
+EVEX_VPTESTNMW_KR_K1_ZMM_ZMMM512: int = 2794
 """
 ``VPTESTNMW k2 {k1}, zmm2, zmm3/m512``
 
 ``EVEX.512.F3.0F38.W1 26 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMD_KR_K1_XMM_XMMM128B32: Code = 2795 # type: ignore
+EVEX_VPTESTMD_KR_K1_XMM_XMMM128B32: int = 2795
 """
 ``VPTESTMD k2 {k1}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMD_KR_K1_YMM_YMMM256B32: Code = 2796 # type: ignore
+EVEX_VPTESTMD_KR_K1_YMM_YMMM256B32: int = 2796
 """
 ``VPTESTMD k2 {k1}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMD_KR_K1_ZMM_ZMMM512B32: Code = 2797 # type: ignore
+EVEX_VPTESTMD_KR_K1_ZMM_ZMMM512B32: int = 2797
 """
 ``VPTESTMD k2 {k1}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 27 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMQ_KR_K1_XMM_XMMM128B64: Code = 2798 # type: ignore
+EVEX_VPTESTMQ_KR_K1_XMM_XMMM128B64: int = 2798
 """
 ``VPTESTMQ k2 {k1}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMQ_KR_K1_YMM_YMMM256B64: Code = 2799 # type: ignore
+EVEX_VPTESTMQ_KR_K1_YMM_YMMM256B64: int = 2799
 """
 ``VPTESTMQ k2 {k1}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTMQ_KR_K1_ZMM_ZMMM512B64: Code = 2800 # type: ignore
+EVEX_VPTESTMQ_KR_K1_ZMM_ZMMM512B64: int = 2800
 """
 ``VPTESTMQ k2 {k1}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 27 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMD_KR_K1_XMM_XMMM128B32: Code = 2801 # type: ignore
+EVEX_VPTESTNMD_KR_K1_XMM_XMMM128B32: int = 2801
 """
 ``VPTESTNMD k2 {k1}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.F3.0F38.W0 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMD_KR_K1_YMM_YMMM256B32: Code = 2802 # type: ignore
+EVEX_VPTESTNMD_KR_K1_YMM_YMMM256B32: int = 2802
 """
 ``VPTESTNMD k2 {k1}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.F3.0F38.W0 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMD_KR_K1_ZMM_ZMMM512B32: Code = 2803 # type: ignore
+EVEX_VPTESTNMD_KR_K1_ZMM_ZMMM512B32: int = 2803
 """
 ``VPTESTNMD k2 {k1}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.F3.0F38.W0 27 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMQ_KR_K1_XMM_XMMM128B64: Code = 2804 # type: ignore
+EVEX_VPTESTNMQ_KR_K1_XMM_XMMM128B64: int = 2804
 """
 ``VPTESTNMQ k2 {k1}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.F3.0F38.W1 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMQ_KR_K1_YMM_YMMM256B64: Code = 2805 # type: ignore
+EVEX_VPTESTNMQ_KR_K1_YMM_YMMM256B64: int = 2805
 """
 ``VPTESTNMQ k2 {k1}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.F3.0F38.W1 27 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTESTNMQ_KR_K1_ZMM_ZMMM512B64: Code = 2806 # type: ignore
+EVEX_VPTESTNMQ_KR_K1_ZMM_ZMMM512B64: int = 2806
 """
 ``VPTESTNMQ k2 {k1}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.F3.0F38.W1 27 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMULDQ_XMM_XMMM128: Code = 2807 # type: ignore
+PMULDQ_XMM_XMMM128: int = 2807
 """
 ``PMULDQ xmm1, xmm2/m128``
 
 ``66 0F 38 28 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMULDQ_XMM_XMM_XMMM128: Code = 2808 # type: ignore
+VEX_VPMULDQ_XMM_XMM_XMMM128: int = 2808
 """
 ``VPMULDQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 28 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULDQ_YMM_YMM_YMMM256: Code = 2809 # type: ignore
+VEX_VPMULDQ_YMM_YMM_YMMM256: int = 2809
 """
 ``VPMULDQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 28 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULDQ_XMM_K1Z_XMM_XMMM128B64: Code = 2810 # type: ignore
+EVEX_VPMULDQ_XMM_K1Z_XMM_XMMM128B64: int = 2810
 """
 ``VPMULDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULDQ_YMM_K1Z_YMM_YMMM256B64: Code = 2811 # type: ignore
+EVEX_VPMULDQ_YMM_K1Z_YMM_YMMM256B64: int = 2811
 """
 ``VPMULDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 28 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULDQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2812 # type: ignore
+EVEX_VPMULDQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2812
 """
 ``VPMULDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 28 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2B_XMM_KR: Code = 2813 # type: ignore
+EVEX_VPMOVM2B_XMM_KR: int = 2813
 """
 ``VPMOVM2B xmm1, k1``
 
 ``EVEX.128.F3.0F38.W0 28 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2B_YMM_KR: Code = 2814 # type: ignore
+EVEX_VPMOVM2B_YMM_KR: int = 2814
 """
 ``VPMOVM2B ymm1, k1``
 
 ``EVEX.256.F3.0F38.W0 28 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2B_ZMM_KR: Code = 2815 # type: ignore
+EVEX_VPMOVM2B_ZMM_KR: int = 2815
 """
 ``VPMOVM2B zmm1, k1``
 
 ``EVEX.512.F3.0F38.W0 28 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2W_XMM_KR: Code = 2816 # type: ignore
+EVEX_VPMOVM2W_XMM_KR: int = 2816
 """
 ``VPMOVM2W xmm1, k1``
 
 ``EVEX.128.F3.0F38.W1 28 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2W_YMM_KR: Code = 2817 # type: ignore
+EVEX_VPMOVM2W_YMM_KR: int = 2817
 """
 ``VPMOVM2W ymm1, k1``
 
 ``EVEX.256.F3.0F38.W1 28 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2W_ZMM_KR: Code = 2818 # type: ignore
+EVEX_VPMOVM2W_ZMM_KR: int = 2818
 """
 ``VPMOVM2W zmm1, k1``
 
 ``EVEX.512.F3.0F38.W1 28 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PCMPEQQ_XMM_XMMM128: Code = 2819 # type: ignore
+PCMPEQQ_XMM_XMMM128: int = 2819
 """
 ``PCMPEQQ xmm1, xmm2/m128``
 
 ``66 0F 38 29 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQQ_XMM_XMM_XMMM128: Code = 2820 # type: ignore
+VEX_VPCMPEQQ_XMM_XMM_XMMM128: int = 2820
 """
 ``VPCMPEQQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 29 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPEQQ_YMM_YMM_YMMM256: Code = 2821 # type: ignore
+VEX_VPCMPEQQ_YMM_YMM_YMMM256: int = 2821
 """
 ``VPCMPEQQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 29 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQQ_KR_K1_XMM_XMMM128B64: Code = 2822 # type: ignore
+EVEX_VPCMPEQQ_KR_K1_XMM_XMMM128B64: int = 2822
 """
 ``VPCMPEQQ k1 {k2}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQQ_KR_K1_YMM_YMMM256B64: Code = 2823 # type: ignore
+EVEX_VPCMPEQQ_KR_K1_YMM_YMMM256B64: int = 2823
 """
 ``VPCMPEQQ k1 {k2}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 29 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPEQQ_KR_K1_ZMM_ZMMM512B64: Code = 2824 # type: ignore
+EVEX_VPCMPEQQ_KR_K1_ZMM_ZMMM512B64: int = 2824
 """
 ``VPCMPEQQ k1 {k2}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 29 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVB2M_KR_XMM: Code = 2825 # type: ignore
+EVEX_VPMOVB2M_KR_XMM: int = 2825
 """
 ``VPMOVB2M k1, xmm1``
 
 ``EVEX.128.F3.0F38.W0 29 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVB2M_KR_YMM: Code = 2826 # type: ignore
+EVEX_VPMOVB2M_KR_YMM: int = 2826
 """
 ``VPMOVB2M k1, ymm1``
 
 ``EVEX.256.F3.0F38.W0 29 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVB2M_KR_ZMM: Code = 2827 # type: ignore
+EVEX_VPMOVB2M_KR_ZMM: int = 2827
 """
 ``VPMOVB2M k1, zmm1``
 
 ``EVEX.512.F3.0F38.W0 29 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVW2M_KR_XMM: Code = 2828 # type: ignore
+EVEX_VPMOVW2M_KR_XMM: int = 2828
 """
 ``VPMOVW2M k1, xmm1``
 
 ``EVEX.128.F3.0F38.W1 29 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVW2M_KR_YMM: Code = 2829 # type: ignore
+EVEX_VPMOVW2M_KR_YMM: int = 2829
 """
 ``VPMOVW2M k1, ymm1``
 
 ``EVEX.256.F3.0F38.W1 29 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVW2M_KR_ZMM: Code = 2830 # type: ignore
+EVEX_VPMOVW2M_KR_ZMM: int = 2830
 """
 ``VPMOVW2M k1, zmm1``
 
 ``EVEX.512.F3.0F38.W1 29 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-MOVNTDQA_XMM_M128: Code = 2831 # type: ignore
+MOVNTDQA_XMM_M128: int = 2831
 """
 ``MOVNTDQA xmm1, m128``
 
 ``66 0F 38 2A /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTDQA_XMM_M128: Code = 2832 # type: ignore
+VEX_VMOVNTDQA_XMM_M128: int = 2832
 """
 ``VMOVNTDQA xmm1, m128``
 
 ``VEX.128.66.0F38.WIG 2A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMOVNTDQA_YMM_M256: Code = 2833 # type: ignore
+VEX_VMOVNTDQA_YMM_M256: int = 2833
 """
 ``VMOVNTDQA ymm1, m256``
 
 ``VEX.256.66.0F38.WIG 2A /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQA_XMM_M128: Code = 2834 # type: ignore
+EVEX_VMOVNTDQA_XMM_M128: int = 2834
 """
 ``VMOVNTDQA xmm1, m128``
 
 ``EVEX.128.66.0F38.W0 2A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQA_YMM_M256: Code = 2835 # type: ignore
+EVEX_VMOVNTDQA_YMM_M256: int = 2835
 """
 ``VMOVNTDQA ymm1, m256``
 
 ``EVEX.256.66.0F38.W0 2A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VMOVNTDQA_ZMM_M512: Code = 2836 # type: ignore
+EVEX_VMOVNTDQA_ZMM_M512: int = 2836
 """
 ``VMOVNTDQA zmm1, m512``
 
 ``EVEX.512.66.0F38.W0 2A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMB2Q_XMM_KR: Code = 2837 # type: ignore
+EVEX_VPBROADCASTMB2Q_XMM_KR: int = 2837
 """
 ``VPBROADCASTMB2Q xmm1, k1``
 
 ``EVEX.128.F3.0F38.W1 2A /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMB2Q_YMM_KR: Code = 2838 # type: ignore
+EVEX_VPBROADCASTMB2Q_YMM_KR: int = 2838
 """
 ``VPBROADCASTMB2Q ymm1, k1``
 
 ``EVEX.256.F3.0F38.W1 2A /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMB2Q_ZMM_KR: Code = 2839 # type: ignore
+EVEX_VPBROADCASTMB2Q_ZMM_KR: int = 2839
 """
 ``VPBROADCASTMB2Q zmm1, k1``
 
 ``EVEX.512.F3.0F38.W1 2A /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-PACKUSDW_XMM_XMMM128: Code = 2840 # type: ignore
+PACKUSDW_XMM_XMMM128: int = 2840
 """
 ``PACKUSDW xmm1, xmm2/m128``
 
 ``66 0F 38 2B /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPACKUSDW_XMM_XMM_XMMM128: Code = 2841 # type: ignore
+VEX_VPACKUSDW_XMM_XMM_XMMM128: int = 2841
 """
 ``VPACKUSDW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 2B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPACKUSDW_YMM_YMM_YMMM256: Code = 2842 # type: ignore
+VEX_VPACKUSDW_YMM_YMM_YMMM256: int = 2842
 """
 ``VPACKUSDW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 2B /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSDW_XMM_K1Z_XMM_XMMM128B32: Code = 2843 # type: ignore
+EVEX_VPACKUSDW_XMM_K1Z_XMM_XMMM128B32: int = 2843
 """
 ``VPACKUSDW xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 2B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSDW_YMM_K1Z_YMM_YMMM256B32: Code = 2844 # type: ignore
+EVEX_VPACKUSDW_YMM_K1Z_YMM_YMMM256B32: int = 2844
 """
 ``VPACKUSDW ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 2B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPACKUSDW_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2845 # type: ignore
+EVEX_VPACKUSDW_ZMM_K1Z_ZMM_ZMMM512B32: int = 2845
 """
 ``VPACKUSDW zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 2B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPS_XMM_XMM_M128: Code = 2846 # type: ignore
+VEX_VMASKMOVPS_XMM_XMM_M128: int = 2846
 """
 ``VMASKMOVPS xmm1, xmm2, m128``
 
 ``VEX.128.66.0F38.W0 2C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPS_YMM_YMM_M256: Code = 2847 # type: ignore
+VEX_VMASKMOVPS_YMM_YMM_M256: int = 2847
 """
 ``VMASKMOVPS ymm1, ymm2, m256``
 
 ``VEX.256.66.0F38.W0 2C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPS_XMM_K1Z_XMM_XMMM128B32: Code = 2848 # type: ignore
+EVEX_VSCALEFPS_XMM_K1Z_XMM_XMMM128B32: int = 2848
 """
 ``VSCALEFPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 2C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPS_YMM_K1Z_YMM_YMMM256B32: Code = 2849 # type: ignore
+EVEX_VSCALEFPS_YMM_K1Z_YMM_YMMM256B32: int = 2849
 """
 ``VSCALEFPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 2C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 2850 # type: ignore
+EVEX_VSCALEFPS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 2850
 """
 ``VSCALEFPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 2C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPD_XMM_K1Z_XMM_XMMM128B64: Code = 2851 # type: ignore
+EVEX_VSCALEFPD_XMM_K1Z_XMM_XMMM128B64: int = 2851
 """
 ``VSCALEFPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 2C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPD_YMM_K1Z_YMM_YMMM256B64: Code = 2852 # type: ignore
+EVEX_VSCALEFPD_YMM_K1Z_YMM_YMMM256B64: int = 2852
 """
 ``VSCALEFPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 2C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 2853 # type: ignore
+EVEX_VSCALEFPD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 2853
 """
 ``VSCALEFPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 2C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPD_XMM_XMM_M128: Code = 2854 # type: ignore
+VEX_VMASKMOVPD_XMM_XMM_M128: int = 2854
 """
 ``VMASKMOVPD xmm1, xmm2, m128``
 
 ``VEX.128.66.0F38.W0 2D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPD_YMM_YMM_M256: Code = 2855 # type: ignore
+VEX_VMASKMOVPD_YMM_YMM_M256: int = 2855
 """
 ``VMASKMOVPD ymm1, ymm2, m256``
 
 ``VEX.256.66.0F38.W0 2D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFSS_XMM_K1Z_XMM_XMMM32_ER: Code = 2856 # type: ignore
+EVEX_VSCALEFSS_XMM_K1Z_XMM_XMMM32_ER: int = 2856
 """
 ``VSCALEFSS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 2D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCALEFSD_XMM_K1Z_XMM_XMMM64_ER: Code = 2857 # type: ignore
+EVEX_VSCALEFSD_XMM_K1Z_XMM_XMMM64_ER: int = 2857
 """
 ``VSCALEFSD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 2D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPS_M128_XMM_XMM: Code = 2858 # type: ignore
+VEX_VMASKMOVPS_M128_XMM_XMM: int = 2858
 """
 ``VMASKMOVPS m128, xmm1, xmm2``
 
 ``VEX.128.66.0F38.W0 2E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPS_M256_YMM_YMM: Code = 2859 # type: ignore
+VEX_VMASKMOVPS_M256_YMM_YMM: int = 2859
 """
 ``VMASKMOVPS m256, ymm1, ymm2``
 
 ``VEX.256.66.0F38.W0 2E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPD_M128_XMM_XMM: Code = 2860 # type: ignore
+VEX_VMASKMOVPD_M128_XMM_XMM: int = 2860
 """
 ``VMASKMOVPD m128, xmm1, xmm2``
 
 ``VEX.128.66.0F38.W0 2F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMASKMOVPD_M256_YMM_YMM: Code = 2861 # type: ignore
+VEX_VMASKMOVPD_M256_YMM_YMM: int = 2861
 """
 ``VMASKMOVPD m256, ymm1, ymm2``
 
 ``VEX.256.66.0F38.W0 2F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PMOVZXBW_XMM_XMMM64: Code = 2862 # type: ignore
+PMOVZXBW_XMM_XMMM64: int = 2862
 """
 ``PMOVZXBW xmm1, xmm2/m64``
 
 ``66 0F 38 30 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBW_XMM_XMMM64: Code = 2863 # type: ignore
+VEX_VPMOVZXBW_XMM_XMMM64: int = 2863
 """
 ``VPMOVZXBW xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 30 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBW_YMM_XMMM128: Code = 2864 # type: ignore
+VEX_VPMOVZXBW_YMM_XMMM128: int = 2864
 """
 ``VPMOVZXBW ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 30 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBW_XMM_K1Z_XMMM64: Code = 2865 # type: ignore
+EVEX_VPMOVZXBW_XMM_K1Z_XMMM64: int = 2865
 """
 ``VPMOVZXBW xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.WIG 30 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBW_YMM_K1Z_XMMM128: Code = 2866 # type: ignore
+EVEX_VPMOVZXBW_YMM_K1Z_XMMM128: int = 2866
 """
 ``VPMOVZXBW ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.WIG 30 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBW_ZMM_K1Z_YMMM256: Code = 2867 # type: ignore
+EVEX_VPMOVZXBW_ZMM_K1Z_YMMM256: int = 2867
 """
 ``VPMOVZXBW zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.WIG 30 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVWB_XMMM64_K1Z_XMM: Code = 2868 # type: ignore
+EVEX_VPMOVWB_XMMM64_K1Z_XMM: int = 2868
 """
 ``VPMOVWB xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 30 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVWB_XMMM128_K1Z_YMM: Code = 2869 # type: ignore
+EVEX_VPMOVWB_XMMM128_K1Z_YMM: int = 2869
 """
 ``VPMOVWB xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 30 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVWB_YMMM256_K1Z_ZMM: Code = 2870 # type: ignore
+EVEX_VPMOVWB_YMMM256_K1Z_ZMM: int = 2870
 """
 ``VPMOVWB ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 30 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMOVZXBD_XMM_XMMM32: Code = 2871 # type: ignore
+PMOVZXBD_XMM_XMMM32: int = 2871
 """
 ``PMOVZXBD xmm1, xmm2/m32``
 
 ``66 0F 38 31 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBD_XMM_XMMM32: Code = 2872 # type: ignore
+VEX_VPMOVZXBD_XMM_XMMM32: int = 2872
 """
 ``VPMOVZXBD xmm1, xmm2/m32``
 
 ``VEX.128.66.0F38.WIG 31 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBD_YMM_XMMM64: Code = 2873 # type: ignore
+VEX_VPMOVZXBD_YMM_XMMM64: int = 2873
 """
 ``VPMOVZXBD ymm1, xmm2/m64``
 
 ``VEX.256.66.0F38.WIG 31 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBD_XMM_K1Z_XMMM32: Code = 2874 # type: ignore
+EVEX_VPMOVZXBD_XMM_K1Z_XMMM32: int = 2874
 """
 ``VPMOVZXBD xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.WIG 31 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBD_YMM_K1Z_XMMM64: Code = 2875 # type: ignore
+EVEX_VPMOVZXBD_YMM_K1Z_XMMM64: int = 2875
 """
 ``VPMOVZXBD ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.WIG 31 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBD_ZMM_K1Z_XMMM128: Code = 2876 # type: ignore
+EVEX_VPMOVZXBD_ZMM_K1Z_XMMM128: int = 2876
 """
 ``VPMOVZXBD zmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.512.66.0F38.WIG 31 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDB_XMMM32_K1Z_XMM: Code = 2877 # type: ignore
+EVEX_VPMOVDB_XMMM32_K1Z_XMM: int = 2877
 """
 ``VPMOVDB xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 31 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDB_XMMM64_K1Z_YMM: Code = 2878 # type: ignore
+EVEX_VPMOVDB_XMMM64_K1Z_YMM: int = 2878
 """
 ``VPMOVDB xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 31 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDB_XMMM128_K1Z_ZMM: Code = 2879 # type: ignore
+EVEX_VPMOVDB_XMMM128_K1Z_ZMM: int = 2879
 """
 ``VPMOVDB xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 31 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVZXBQ_XMM_XMMM16: Code = 2880 # type: ignore
+PMOVZXBQ_XMM_XMMM16: int = 2880
 """
 ``PMOVZXBQ xmm1, xmm2/m16``
 
 ``66 0F 38 32 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBQ_XMM_XMMM16: Code = 2881 # type: ignore
+VEX_VPMOVZXBQ_XMM_XMMM16: int = 2881
 """
 ``VPMOVZXBQ xmm1, xmm2/m16``
 
 ``VEX.128.66.0F38.WIG 32 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXBQ_YMM_XMMM32: Code = 2882 # type: ignore
+VEX_VPMOVZXBQ_YMM_XMMM32: int = 2882
 """
 ``VPMOVZXBQ ymm1, xmm2/m32``
 
 ``VEX.256.66.0F38.WIG 32 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBQ_XMM_K1Z_XMMM16: Code = 2883 # type: ignore
+EVEX_VPMOVZXBQ_XMM_K1Z_XMMM16: int = 2883
 """
 ``VPMOVZXBQ xmm1 {k1}{z}, xmm2/m16``
 
 ``EVEX.128.66.0F38.WIG 32 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBQ_YMM_K1Z_XMMM32: Code = 2884 # type: ignore
+EVEX_VPMOVZXBQ_YMM_K1Z_XMMM32: int = 2884
 """
 ``VPMOVZXBQ ymm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.256.66.0F38.WIG 32 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXBQ_ZMM_K1Z_XMMM64: Code = 2885 # type: ignore
+EVEX_VPMOVZXBQ_ZMM_K1Z_XMMM64: int = 2885
 """
 ``VPMOVZXBQ zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.WIG 32 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQB_XMMM16_K1Z_XMM: Code = 2886 # type: ignore
+EVEX_VPMOVQB_XMMM16_K1Z_XMM: int = 2886
 """
 ``VPMOVQB xmm1/m16 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 32 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQB_XMMM32_K1Z_YMM: Code = 2887 # type: ignore
+EVEX_VPMOVQB_XMMM32_K1Z_YMM: int = 2887
 """
 ``VPMOVQB xmm1/m32 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 32 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQB_XMMM64_K1Z_ZMM: Code = 2888 # type: ignore
+EVEX_VPMOVQB_XMMM64_K1Z_ZMM: int = 2888
 """
 ``VPMOVQB xmm1/m64 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 32 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVZXWD_XMM_XMMM64: Code = 2889 # type: ignore
+PMOVZXWD_XMM_XMMM64: int = 2889
 """
 ``PMOVZXWD xmm1, xmm2/m64``
 
 ``66 0F 38 33 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXWD_XMM_XMMM64: Code = 2890 # type: ignore
+VEX_VPMOVZXWD_XMM_XMMM64: int = 2890
 """
 ``VPMOVZXWD xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 33 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXWD_YMM_XMMM128: Code = 2891 # type: ignore
+VEX_VPMOVZXWD_YMM_XMMM128: int = 2891
 """
 ``VPMOVZXWD ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 33 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWD_XMM_K1Z_XMMM64: Code = 2892 # type: ignore
+EVEX_VPMOVZXWD_XMM_K1Z_XMMM64: int = 2892
 """
 ``VPMOVZXWD xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.WIG 33 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWD_YMM_K1Z_XMMM128: Code = 2893 # type: ignore
+EVEX_VPMOVZXWD_YMM_K1Z_XMMM128: int = 2893
 """
 ``VPMOVZXWD ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.WIG 33 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWD_ZMM_K1Z_YMMM256: Code = 2894 # type: ignore
+EVEX_VPMOVZXWD_ZMM_K1Z_YMMM256: int = 2894
 """
 ``VPMOVZXWD zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.WIG 33 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDW_XMMM64_K1Z_XMM: Code = 2895 # type: ignore
+EVEX_VPMOVDW_XMMM64_K1Z_XMM: int = 2895
 """
 ``VPMOVDW xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 33 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDW_XMMM128_K1Z_YMM: Code = 2896 # type: ignore
+EVEX_VPMOVDW_XMMM128_K1Z_YMM: int = 2896
 """
 ``VPMOVDW xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 33 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVDW_YMMM256_K1Z_ZMM: Code = 2897 # type: ignore
+EVEX_VPMOVDW_YMMM256_K1Z_ZMM: int = 2897
 """
 ``VPMOVDW ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 33 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVZXWQ_XMM_XMMM32: Code = 2898 # type: ignore
+PMOVZXWQ_XMM_XMMM32: int = 2898
 """
 ``PMOVZXWQ xmm1, xmm2/m32``
 
 ``66 0F 38 34 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXWQ_XMM_XMMM32: Code = 2899 # type: ignore
+VEX_VPMOVZXWQ_XMM_XMMM32: int = 2899
 """
 ``VPMOVZXWQ xmm1, xmm2/m32``
 
 ``VEX.128.66.0F38.WIG 34 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXWQ_YMM_XMMM64: Code = 2900 # type: ignore
+VEX_VPMOVZXWQ_YMM_XMMM64: int = 2900
 """
 ``VPMOVZXWQ ymm1, xmm2/m64``
 
 ``VEX.256.66.0F38.WIG 34 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWQ_XMM_K1Z_XMMM32: Code = 2901 # type: ignore
+EVEX_VPMOVZXWQ_XMM_K1Z_XMMM32: int = 2901
 """
 ``VPMOVZXWQ xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.WIG 34 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWQ_YMM_K1Z_XMMM64: Code = 2902 # type: ignore
+EVEX_VPMOVZXWQ_YMM_K1Z_XMMM64: int = 2902
 """
 ``VPMOVZXWQ ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.WIG 34 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXWQ_ZMM_K1Z_XMMM128: Code = 2903 # type: ignore
+EVEX_VPMOVZXWQ_ZMM_K1Z_XMMM128: int = 2903
 """
 ``VPMOVZXWQ zmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.512.66.0F38.WIG 34 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQW_XMMM32_K1Z_XMM: Code = 2904 # type: ignore
+EVEX_VPMOVQW_XMMM32_K1Z_XMM: int = 2904
 """
 ``VPMOVQW xmm1/m32 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 34 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQW_XMMM64_K1Z_YMM: Code = 2905 # type: ignore
+EVEX_VPMOVQW_XMMM64_K1Z_YMM: int = 2905
 """
 ``VPMOVQW xmm1/m64 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 34 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQW_XMMM128_K1Z_ZMM: Code = 2906 # type: ignore
+EVEX_VPMOVQW_XMMM128_K1Z_ZMM: int = 2906
 """
 ``VPMOVQW xmm1/m128 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 34 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMOVZXDQ_XMM_XMMM64: Code = 2907 # type: ignore
+PMOVZXDQ_XMM_XMMM64: int = 2907
 """
 ``PMOVZXDQ xmm1, xmm2/m64``
 
 ``66 0F 38 35 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXDQ_XMM_XMMM64: Code = 2908 # type: ignore
+VEX_VPMOVZXDQ_XMM_XMMM64: int = 2908
 """
 ``VPMOVZXDQ xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.WIG 35 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMOVZXDQ_YMM_XMMM128: Code = 2909 # type: ignore
+VEX_VPMOVZXDQ_YMM_XMMM128: int = 2909
 """
 ``VPMOVZXDQ ymm1, xmm2/m128``
 
 ``VEX.256.66.0F38.WIG 35 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXDQ_XMM_K1Z_XMMM64: Code = 2910 # type: ignore
+EVEX_VPMOVZXDQ_XMM_K1Z_XMMM64: int = 2910
 """
 ``VPMOVZXDQ xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.W0 35 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXDQ_YMM_K1Z_XMMM128: Code = 2911 # type: ignore
+EVEX_VPMOVZXDQ_YMM_K1Z_XMMM128: int = 2911
 """
 ``VPMOVZXDQ ymm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.256.66.0F38.W0 35 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVZXDQ_ZMM_K1Z_YMMM256: Code = 2912 # type: ignore
+EVEX_VPMOVZXDQ_ZMM_K1Z_YMMM256: int = 2912
 """
 ``VPMOVZXDQ zmm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.512.66.0F38.W0 35 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQD_XMMM64_K1Z_XMM: Code = 2913 # type: ignore
+EVEX_VPMOVQD_XMMM64_K1Z_XMM: int = 2913
 """
 ``VPMOVQD xmm1/m64 {k1}{z}, xmm2``
 
 ``EVEX.128.F3.0F38.W0 35 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQD_XMMM128_K1Z_YMM: Code = 2914 # type: ignore
+EVEX_VPMOVQD_XMMM128_K1Z_YMM: int = 2914
 """
 ``VPMOVQD xmm1/m128 {k1}{z}, ymm2``
 
 ``EVEX.256.F3.0F38.W0 35 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQD_YMMM256_K1Z_ZMM: Code = 2915 # type: ignore
+EVEX_VPMOVQD_YMMM256_K1Z_ZMM: int = 2915
 """
 ``VPMOVQD ymm1/m256 {k1}{z}, zmm2``
 
 ``EVEX.512.F3.0F38.W0 35 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMD_YMM_YMM_YMMM256: Code = 2916 # type: ignore
+VEX_VPERMD_YMM_YMM_YMMM256: int = 2916
 """
 ``VPERMD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 36 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMD_YMM_K1Z_YMM_YMMM256B32: Code = 2917 # type: ignore
+EVEX_VPERMD_YMM_K1Z_YMM_YMMM256B32: int = 2917
 """
 ``VPERMD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 36 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2918 # type: ignore
+EVEX_VPERMD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2918
 """
 ``VPERMD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 36 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMQ_YMM_K1Z_YMM_YMMM256B64: Code = 2919 # type: ignore
+EVEX_VPERMQ_YMM_K1Z_YMM_YMMM256B64: int = 2919
 """
 ``VPERMQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 36 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2920 # type: ignore
+EVEX_VPERMQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2920
 """
 ``VPERMQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 36 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PCMPGTQ_XMM_XMMM128: Code = 2921 # type: ignore
+PCMPGTQ_XMM_XMMM128: int = 2921
 """
 ``PCMPGTQ xmm1, xmm2/m128``
 
 ``66 0F 38 37 /r``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTQ_XMM_XMM_XMMM128: Code = 2922 # type: ignore
+VEX_VPCMPGTQ_XMM_XMM_XMMM128: int = 2922
 """
 ``VPCMPGTQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 37 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPGTQ_YMM_YMM_YMMM256: Code = 2923 # type: ignore
+VEX_VPCMPGTQ_YMM_YMM_YMMM256: int = 2923
 """
 ``VPCMPGTQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 37 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTQ_KR_K1_XMM_XMMM128B64: Code = 2924 # type: ignore
+EVEX_VPCMPGTQ_KR_K1_XMM_XMMM128B64: int = 2924
 """
 ``VPCMPGTQ k1 {k2}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 37 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTQ_KR_K1_YMM_YMMM256B64: Code = 2925 # type: ignore
+EVEX_VPCMPGTQ_KR_K1_YMM_YMMM256B64: int = 2925
 """
 ``VPCMPGTQ k1 {k2}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 37 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPGTQ_KR_K1_ZMM_ZMMM512B64: Code = 2926 # type: ignore
+EVEX_VPCMPGTQ_KR_K1_ZMM_ZMMM512B64: int = 2926
 """
 ``VPCMPGTQ k1 {k2}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 37 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMINSB_XMM_XMMM128: Code = 2927 # type: ignore
+PMINSB_XMM_XMMM128: int = 2927
 """
 ``PMINSB xmm1, xmm2/m128``
 
 ``66 0F 38 38 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSB_XMM_XMM_XMMM128: Code = 2928 # type: ignore
+VEX_VPMINSB_XMM_XMM_XMMM128: int = 2928
 """
 ``VPMINSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 38 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSB_YMM_YMM_YMMM256: Code = 2929 # type: ignore
+VEX_VPMINSB_YMM_YMM_YMMM256: int = 2929
 """
 ``VPMINSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 38 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSB_XMM_K1Z_XMM_XMMM128: Code = 2930 # type: ignore
+EVEX_VPMINSB_XMM_K1Z_XMM_XMMM128: int = 2930
 """
 ``VPMINSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 38 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSB_YMM_K1Z_YMM_YMMM256: Code = 2931 # type: ignore
+EVEX_VPMINSB_YMM_K1Z_YMM_YMMM256: int = 2931
 """
 ``VPMINSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 38 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2932 # type: ignore
+EVEX_VPMINSB_ZMM_K1Z_ZMM_ZMMM512: int = 2932
 """
 ``VPMINSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 38 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2D_XMM_KR: Code = 2933 # type: ignore
+EVEX_VPMOVM2D_XMM_KR: int = 2933
 """
 ``VPMOVM2D xmm1, k1``
 
 ``EVEX.128.F3.0F38.W0 38 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2D_YMM_KR: Code = 2934 # type: ignore
+EVEX_VPMOVM2D_YMM_KR: int = 2934
 """
 ``VPMOVM2D ymm1, k1``
 
 ``EVEX.256.F3.0F38.W0 38 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2D_ZMM_KR: Code = 2935 # type: ignore
+EVEX_VPMOVM2D_ZMM_KR: int = 2935
 """
 ``VPMOVM2D zmm1, k1``
 
 ``EVEX.512.F3.0F38.W0 38 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2Q_XMM_KR: Code = 2936 # type: ignore
+EVEX_VPMOVM2Q_XMM_KR: int = 2936
 """
 ``VPMOVM2Q xmm1, k1``
 
 ``EVEX.128.F3.0F38.W1 38 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2Q_YMM_KR: Code = 2937 # type: ignore
+EVEX_VPMOVM2Q_YMM_KR: int = 2937
 """
 ``VPMOVM2Q ymm1, k1``
 
 ``EVEX.256.F3.0F38.W1 38 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVM2Q_ZMM_KR: Code = 2938 # type: ignore
+EVEX_VPMOVM2Q_ZMM_KR: int = 2938
 """
 ``VPMOVM2Q zmm1, k1``
 
 ``EVEX.512.F3.0F38.W1 38 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-PMINSD_XMM_XMMM128: Code = 2939 # type: ignore
+PMINSD_XMM_XMMM128: int = 2939
 """
 ``PMINSD xmm1, xmm2/m128``
 
 ``66 0F 38 39 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSD_XMM_XMM_XMMM128: Code = 2940 # type: ignore
+VEX_VPMINSD_XMM_XMM_XMMM128: int = 2940
 """
 ``VPMINSD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 39 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINSD_YMM_YMM_YMMM256: Code = 2941 # type: ignore
+VEX_VPMINSD_YMM_YMM_YMMM256: int = 2941
 """
 ``VPMINSD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 39 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSD_XMM_K1Z_XMM_XMMM128B32: Code = 2942 # type: ignore
+EVEX_VPMINSD_XMM_K1Z_XMM_XMMM128B32: int = 2942
 """
 ``VPMINSD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 39 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSD_YMM_K1Z_YMM_YMMM256B32: Code = 2943 # type: ignore
+EVEX_VPMINSD_YMM_K1Z_YMM_YMMM256B32: int = 2943
 """
 ``VPMINSD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 39 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2944 # type: ignore
+EVEX_VPMINSD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2944
 """
 ``VPMINSD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 39 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSQ_XMM_K1Z_XMM_XMMM128B64: Code = 2945 # type: ignore
+EVEX_VPMINSQ_XMM_K1Z_XMM_XMMM128B64: int = 2945
 """
 ``VPMINSQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 39 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSQ_YMM_K1Z_YMM_YMMM256B64: Code = 2946 # type: ignore
+EVEX_VPMINSQ_YMM_K1Z_YMM_YMMM256B64: int = 2946
 """
 ``VPMINSQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 39 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINSQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2947 # type: ignore
+EVEX_VPMINSQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2947
 """
 ``VPMINSQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 39 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVD2M_KR_XMM: Code = 2948 # type: ignore
+EVEX_VPMOVD2M_KR_XMM: int = 2948
 """
 ``VPMOVD2M k1, xmm1``
 
 ``EVEX.128.F3.0F38.W0 39 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVD2M_KR_YMM: Code = 2949 # type: ignore
+EVEX_VPMOVD2M_KR_YMM: int = 2949
 """
 ``VPMOVD2M k1, ymm1``
 
 ``EVEX.256.F3.0F38.W0 39 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVD2M_KR_ZMM: Code = 2950 # type: ignore
+EVEX_VPMOVD2M_KR_ZMM: int = 2950
 """
 ``VPMOVD2M k1, zmm1``
 
 ``EVEX.512.F3.0F38.W0 39 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQ2M_KR_XMM: Code = 2951 # type: ignore
+EVEX_VPMOVQ2M_KR_XMM: int = 2951
 """
 ``VPMOVQ2M k1, xmm1``
 
 ``EVEX.128.F3.0F38.W1 39 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQ2M_KR_YMM: Code = 2952 # type: ignore
+EVEX_VPMOVQ2M_KR_YMM: int = 2952
 """
 ``VPMOVQ2M k1, ymm1``
 
 ``EVEX.256.F3.0F38.W1 39 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMOVQ2M_KR_ZMM: Code = 2953 # type: ignore
+EVEX_VPMOVQ2M_KR_ZMM: int = 2953
 """
 ``VPMOVQ2M k1, zmm1``
 
 ``EVEX.512.F3.0F38.W1 39 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-PMINUW_XMM_XMMM128: Code = 2954 # type: ignore
+PMINUW_XMM_XMMM128: int = 2954
 """
 ``PMINUW xmm1, xmm2/m128``
 
 ``66 0F 38 3A /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUW_XMM_XMM_XMMM128: Code = 2955 # type: ignore
+VEX_VPMINUW_XMM_XMM_XMMM128: int = 2955
 """
 ``VPMINUW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3A /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUW_YMM_YMM_YMMM256: Code = 2956 # type: ignore
+VEX_VPMINUW_YMM_YMM_YMMM256: int = 2956
 """
 ``VPMINUW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3A /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUW_XMM_K1Z_XMM_XMMM128: Code = 2957 # type: ignore
+EVEX_VPMINUW_XMM_K1Z_XMM_XMMM128: int = 2957
 """
 ``VPMINUW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 3A /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUW_YMM_K1Z_YMM_YMMM256: Code = 2958 # type: ignore
+EVEX_VPMINUW_YMM_K1Z_YMM_YMMM256: int = 2958
 """
 ``VPMINUW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 3A /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUW_ZMM_K1Z_ZMM_ZMMM512: Code = 2959 # type: ignore
+EVEX_VPMINUW_ZMM_K1Z_ZMM_ZMMM512: int = 2959
 """
 ``VPMINUW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 3A /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMW2D_XMM_KR: Code = 2960 # type: ignore
+EVEX_VPBROADCASTMW2D_XMM_KR: int = 2960
 """
 ``VPBROADCASTMW2D xmm1, k1``
 
 ``EVEX.128.F3.0F38.W0 3A /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMW2D_YMM_KR: Code = 2961 # type: ignore
+EVEX_VPBROADCASTMW2D_YMM_KR: int = 2961
 """
 ``VPBROADCASTMW2D ymm1, k1``
 
 ``EVEX.256.F3.0F38.W0 3A /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTMW2D_ZMM_KR: Code = 2962 # type: ignore
+EVEX_VPBROADCASTMW2D_ZMM_KR: int = 2962
 """
 ``VPBROADCASTMW2D zmm1, k1``
 
 ``EVEX.512.F3.0F38.W0 3A /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-PMINUD_XMM_XMMM128: Code = 2963 # type: ignore
+PMINUD_XMM_XMMM128: int = 2963
 """
 ``PMINUD xmm1, xmm2/m128``
 
 ``66 0F 38 3B /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUD_XMM_XMM_XMMM128: Code = 2964 # type: ignore
+VEX_VPMINUD_XMM_XMM_XMMM128: int = 2964
 """
 ``VPMINUD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3B /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMINUD_YMM_YMM_YMMM256: Code = 2965 # type: ignore
+VEX_VPMINUD_YMM_YMM_YMMM256: int = 2965
 """
 ``VPMINUD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3B /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUD_XMM_K1Z_XMM_XMMM128B32: Code = 2966 # type: ignore
+EVEX_VPMINUD_XMM_K1Z_XMM_XMMM128B32: int = 2966
 """
 ``VPMINUD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 3B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUD_YMM_K1Z_YMM_YMMM256B32: Code = 2967 # type: ignore
+EVEX_VPMINUD_YMM_K1Z_YMM_YMMM256B32: int = 2967
 """
 ``VPMINUD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 3B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2968 # type: ignore
+EVEX_VPMINUD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2968
 """
 ``VPMINUD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 3B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUQ_XMM_K1Z_XMM_XMMM128B64: Code = 2969 # type: ignore
+EVEX_VPMINUQ_XMM_K1Z_XMM_XMMM128B64: int = 2969
 """
 ``VPMINUQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 3B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUQ_YMM_K1Z_YMM_YMMM256B64: Code = 2970 # type: ignore
+EVEX_VPMINUQ_YMM_K1Z_YMM_YMMM256B64: int = 2970
 """
 ``VPMINUQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 3B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMINUQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2971 # type: ignore
+EVEX_VPMINUQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2971
 """
 ``VPMINUQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 3B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMAXSB_XMM_XMMM128: Code = 2972 # type: ignore
+PMAXSB_XMM_XMMM128: int = 2972
 """
 ``PMAXSB xmm1, xmm2/m128``
 
 ``66 0F 38 3C /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSB_XMM_XMM_XMMM128: Code = 2973 # type: ignore
+VEX_VPMAXSB_XMM_XMM_XMMM128: int = 2973
 """
 ``VPMAXSB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3C /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSB_YMM_YMM_YMMM256: Code = 2974 # type: ignore
+VEX_VPMAXSB_YMM_YMM_YMMM256: int = 2974
 """
 ``VPMAXSB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSB_XMM_K1Z_XMM_XMMM128: Code = 2975 # type: ignore
+EVEX_VPMAXSB_XMM_K1Z_XMM_XMMM128: int = 2975
 """
 ``VPMAXSB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 3C /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSB_YMM_K1Z_YMM_YMMM256: Code = 2976 # type: ignore
+EVEX_VPMAXSB_YMM_K1Z_YMM_YMMM256: int = 2976
 """
 ``VPMAXSB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 3C /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSB_ZMM_K1Z_ZMM_ZMMM512: Code = 2977 # type: ignore
+EVEX_VPMAXSB_ZMM_K1Z_ZMM_ZMMM512: int = 2977
 """
 ``VPMAXSB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 3C /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMAXSD_XMM_XMMM128: Code = 2978 # type: ignore
+PMAXSD_XMM_XMMM128: int = 2978
 """
 ``PMAXSD xmm1, xmm2/m128``
 
 ``66 0F 38 3D /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSD_XMM_XMM_XMMM128: Code = 2979 # type: ignore
+VEX_VPMAXSD_XMM_XMM_XMMM128: int = 2979
 """
 ``VPMAXSD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3D /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXSD_YMM_YMM_YMMM256: Code = 2980 # type: ignore
+VEX_VPMAXSD_YMM_YMM_YMMM256: int = 2980
 """
 ``VPMAXSD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3D /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSD_XMM_K1Z_XMM_XMMM128B32: Code = 2981 # type: ignore
+EVEX_VPMAXSD_XMM_K1Z_XMM_XMMM128B32: int = 2981
 """
 ``VPMAXSD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 3D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSD_YMM_K1Z_YMM_YMMM256B32: Code = 2982 # type: ignore
+EVEX_VPMAXSD_YMM_K1Z_YMM_YMMM256B32: int = 2982
 """
 ``VPMAXSD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 3D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2983 # type: ignore
+EVEX_VPMAXSD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2983
 """
 ``VPMAXSD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 3D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSQ_XMM_K1Z_XMM_XMMM128B64: Code = 2984 # type: ignore
+EVEX_VPMAXSQ_XMM_K1Z_XMM_XMMM128B64: int = 2984
 """
 ``VPMAXSQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 3D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSQ_YMM_K1Z_YMM_YMMM256B64: Code = 2985 # type: ignore
+EVEX_VPMAXSQ_YMM_K1Z_YMM_YMMM256B64: int = 2985
 """
 ``VPMAXSQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 3D /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXSQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 2986 # type: ignore
+EVEX_VPMAXSQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 2986
 """
 ``VPMAXSQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 3D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMAXUW_XMM_XMMM128: Code = 2987 # type: ignore
+PMAXUW_XMM_XMMM128: int = 2987
 """
 ``PMAXUW xmm1, xmm2/m128``
 
 ``66 0F 38 3E /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUW_XMM_XMM_XMMM128: Code = 2988 # type: ignore
+VEX_VPMAXUW_XMM_XMM_XMMM128: int = 2988
 """
 ``VPMAXUW xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3E /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUW_YMM_YMM_YMMM256: Code = 2989 # type: ignore
+VEX_VPMAXUW_YMM_YMM_YMMM256: int = 2989
 """
 ``VPMAXUW ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUW_XMM_K1Z_XMM_XMMM128: Code = 2990 # type: ignore
+EVEX_VPMAXUW_XMM_K1Z_XMM_XMMM128: int = 2990
 """
 ``VPMAXUW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG 3E /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUW_YMM_K1Z_YMM_YMMM256: Code = 2991 # type: ignore
+EVEX_VPMAXUW_YMM_K1Z_YMM_YMMM256: int = 2991
 """
 ``VPMAXUW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG 3E /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUW_ZMM_K1Z_ZMM_ZMMM512: Code = 2992 # type: ignore
+EVEX_VPMAXUW_ZMM_K1Z_ZMM_ZMMM512: int = 2992
 """
 ``VPMAXUW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG 3E /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PMAXUD_XMM_XMMM128: Code = 2993 # type: ignore
+PMAXUD_XMM_XMMM128: int = 2993
 """
 ``PMAXUD xmm1, xmm2/m128``
 
 ``66 0F 38 3F /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUD_XMM_XMM_XMMM128: Code = 2994 # type: ignore
+VEX_VPMAXUD_XMM_XMM_XMMM128: int = 2994
 """
 ``VPMAXUD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 3F /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMAXUD_YMM_YMM_YMMM256: Code = 2995 # type: ignore
+VEX_VPMAXUD_YMM_YMM_YMMM256: int = 2995
 """
 ``VPMAXUD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 3F /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUD_XMM_K1Z_XMM_XMMM128B32: Code = 2996 # type: ignore
+EVEX_VPMAXUD_XMM_K1Z_XMM_XMMM128B32: int = 2996
 """
 ``VPMAXUD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 3F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUD_YMM_K1Z_YMM_YMMM256B32: Code = 2997 # type: ignore
+EVEX_VPMAXUD_YMM_K1Z_YMM_YMMM256B32: int = 2997
 """
 ``VPMAXUD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 3F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 2998 # type: ignore
+EVEX_VPMAXUD_ZMM_K1Z_ZMM_ZMMM512B32: int = 2998
 """
 ``VPMAXUD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 3F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUQ_XMM_K1Z_XMM_XMMM128B64: Code = 2999 # type: ignore
+EVEX_VPMAXUQ_XMM_K1Z_XMM_XMMM128B64: int = 2999
 """
 ``VPMAXUQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 3F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUQ_YMM_K1Z_YMM_YMMM256B64: Code = 3000 # type: ignore
+EVEX_VPMAXUQ_YMM_K1Z_YMM_YMMM256B64: int = 3000
 """
 ``VPMAXUQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 3F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMAXUQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3001 # type: ignore
+EVEX_VPMAXUQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3001
 """
 ``VPMAXUQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 3F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PMULLD_XMM_XMMM128: Code = 3002 # type: ignore
+PMULLD_XMM_XMMM128: int = 3002
 """
 ``PMULLD xmm1, xmm2/m128``
 
 ``66 0F 38 40 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPMULLD_XMM_XMM_XMMM128: Code = 3003 # type: ignore
+VEX_VPMULLD_XMM_XMM_XMMM128: int = 3003
 """
 ``VPMULLD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG 40 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPMULLD_YMM_YMM_YMMM256: Code = 3004 # type: ignore
+VEX_VPMULLD_YMM_YMM_YMMM256: int = 3004
 """
 ``VPMULLD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG 40 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLD_XMM_K1Z_XMM_XMMM128B32: Code = 3005 # type: ignore
+EVEX_VPMULLD_XMM_K1Z_XMM_XMMM128B32: int = 3005
 """
 ``VPMULLD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 40 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLD_YMM_K1Z_YMM_YMMM256B32: Code = 3006 # type: ignore
+EVEX_VPMULLD_YMM_K1Z_YMM_YMMM256B32: int = 3006
 """
 ``VPMULLD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 40 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3007 # type: ignore
+EVEX_VPMULLD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3007
 """
 ``VPMULLD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 40 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLQ_XMM_K1Z_XMM_XMMM128B64: Code = 3008 # type: ignore
+EVEX_VPMULLQ_XMM_K1Z_XMM_XMMM128B64: int = 3008
 """
 ``VPMULLQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 40 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLQ_YMM_K1Z_YMM_YMMM256B64: Code = 3009 # type: ignore
+EVEX_VPMULLQ_YMM_K1Z_YMM_YMMM256B64: int = 3009
 """
 ``VPMULLQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 40 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULLQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3010 # type: ignore
+EVEX_VPMULLQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3010
 """
 ``VPMULLQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 40 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-PHMINPOSUW_XMM_XMMM128: Code = 3011 # type: ignore
+PHMINPOSUW_XMM_XMMM128: int = 3011
 """
 ``PHMINPOSUW xmm1, xmm2/m128``
 
 ``66 0F 38 41 /r``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPHMINPOSUW_XMM_XMMM128: Code = 3012 # type: ignore
+VEX_VPHMINPOSUW_XMM_XMMM128: int = 3012
 """
 ``VPHMINPOSUW xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG 41 /r``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPS_XMM_K1Z_XMMM128B32: Code = 3013 # type: ignore
+EVEX_VGETEXPPS_XMM_K1Z_XMMM128B32: int = 3013
 """
 ``VGETEXPPS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 42 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPS_YMM_K1Z_YMMM256B32: Code = 3014 # type: ignore
+EVEX_VGETEXPPS_YMM_K1Z_YMMM256B32: int = 3014
 """
 ``VGETEXPPS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 42 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPS_ZMM_K1Z_ZMMM512B32_SAE: Code = 3015 # type: ignore
+EVEX_VGETEXPPS_ZMM_K1Z_ZMMM512B32_SAE: int = 3015
 """
 ``VGETEXPPS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.66.0F38.W0 42 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPD_XMM_K1Z_XMMM128B64: Code = 3016 # type: ignore
+EVEX_VGETEXPPD_XMM_K1Z_XMMM128B64: int = 3016
 """
 ``VGETEXPPD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 42 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPD_YMM_K1Z_YMMM256B64: Code = 3017 # type: ignore
+EVEX_VGETEXPPD_YMM_K1Z_YMMM256B64: int = 3017
 """
 ``VGETEXPPD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 42 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPPD_ZMM_K1Z_ZMMM512B64_SAE: Code = 3018 # type: ignore
+EVEX_VGETEXPPD_ZMM_K1Z_ZMMM512B64_SAE: int = 3018
 """
 ``VGETEXPPD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F38.W1 42 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPSS_XMM_K1Z_XMM_XMMM32_SAE: Code = 3019 # type: ignore
+EVEX_VGETEXPSS_XMM_K1Z_XMM_XMMM32_SAE: int = 3019
 """
 ``VGETEXPSS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.66.0F38.W0 43 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETEXPSD_XMM_K1Z_XMM_XMMM64_SAE: Code = 3020 # type: ignore
+EVEX_VGETEXPSD_XMM_K1Z_XMM_XMMM64_SAE: int = 3020
 """
 ``VGETEXPSD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}``
 
 ``EVEX.LIG.66.0F38.W1 43 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTD_XMM_K1Z_XMMM128B32: Code = 3021 # type: ignore
+EVEX_VPLZCNTD_XMM_K1Z_XMMM128B32: int = 3021
 """
 ``VPLZCNTD xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 44 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTD_YMM_K1Z_YMMM256B32: Code = 3022 # type: ignore
+EVEX_VPLZCNTD_YMM_K1Z_YMMM256B32: int = 3022
 """
 ``VPLZCNTD ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 44 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTD_ZMM_K1Z_ZMMM512B32: Code = 3023 # type: ignore
+EVEX_VPLZCNTD_ZMM_K1Z_ZMMM512B32: int = 3023
 """
 ``VPLZCNTD zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 44 /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTQ_XMM_K1Z_XMMM128B64: Code = 3024 # type: ignore
+EVEX_VPLZCNTQ_XMM_K1Z_XMMM128B64: int = 3024
 """
 ``VPLZCNTQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 44 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTQ_YMM_K1Z_YMMM256B64: Code = 3025 # type: ignore
+EVEX_VPLZCNTQ_YMM_K1Z_YMMM256B64: int = 3025
 """
 ``VPLZCNTQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 44 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPLZCNTQ_ZMM_K1Z_ZMMM512B64: Code = 3026 # type: ignore
+EVEX_VPLZCNTQ_ZMM_K1Z_ZMMM512B64: int = 3026
 """
 ``VPLZCNTQ zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 44 /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLVD_XMM_XMM_XMMM128: Code = 3027 # type: ignore
+VEX_VPSRLVD_XMM_XMM_XMMM128: int = 3027
 """
 ``VPSRLVD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 45 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLVD_YMM_YMM_YMMM256: Code = 3028 # type: ignore
+VEX_VPSRLVD_YMM_YMM_YMMM256: int = 3028
 """
 ``VPSRLVD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 45 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLVQ_XMM_XMM_XMMM128: Code = 3029 # type: ignore
+VEX_VPSRLVQ_XMM_XMM_XMMM128: int = 3029
 """
 ``VPSRLVQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 45 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRLVQ_YMM_YMM_YMMM256: Code = 3030 # type: ignore
+VEX_VPSRLVQ_YMM_YMM_YMMM256: int = 3030
 """
 ``VPSRLVQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 45 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVD_XMM_K1Z_XMM_XMMM128B32: Code = 3031 # type: ignore
+EVEX_VPSRLVD_XMM_K1Z_XMM_XMMM128B32: int = 3031
 """
 ``VPSRLVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 45 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVD_YMM_K1Z_YMM_YMMM256B32: Code = 3032 # type: ignore
+EVEX_VPSRLVD_YMM_K1Z_YMM_YMMM256B32: int = 3032
 """
 ``VPSRLVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 45 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3033 # type: ignore
+EVEX_VPSRLVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3033
 """
 ``VPSRLVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 45 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVQ_XMM_K1Z_XMM_XMMM128B64: Code = 3034 # type: ignore
+EVEX_VPSRLVQ_XMM_K1Z_XMM_XMMM128B64: int = 3034
 """
 ``VPSRLVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 45 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVQ_YMM_K1Z_YMM_YMMM256B64: Code = 3035 # type: ignore
+EVEX_VPSRLVQ_YMM_K1Z_YMM_YMMM256B64: int = 3035
 """
 ``VPSRLVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 45 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRLVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3036 # type: ignore
+EVEX_VPSRLVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3036
 """
 ``VPSRLVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 45 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAVD_XMM_XMM_XMMM128: Code = 3037 # type: ignore
+VEX_VPSRAVD_XMM_XMM_XMMM128: int = 3037
 """
 ``VPSRAVD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 46 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSRAVD_YMM_YMM_YMMM256: Code = 3038 # type: ignore
+VEX_VPSRAVD_YMM_YMM_YMMM256: int = 3038
 """
 ``VPSRAVD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 46 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVD_XMM_K1Z_XMM_XMMM128B32: Code = 3039 # type: ignore
+EVEX_VPSRAVD_XMM_K1Z_XMM_XMMM128B32: int = 3039
 """
 ``VPSRAVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 46 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVD_YMM_K1Z_YMM_YMMM256B32: Code = 3040 # type: ignore
+EVEX_VPSRAVD_YMM_K1Z_YMM_YMMM256B32: int = 3040
 """
 ``VPSRAVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 46 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3041 # type: ignore
+EVEX_VPSRAVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3041
 """
 ``VPSRAVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 46 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVQ_XMM_K1Z_XMM_XMMM128B64: Code = 3042 # type: ignore
+EVEX_VPSRAVQ_XMM_K1Z_XMM_XMMM128B64: int = 3042
 """
 ``VPSRAVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 46 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVQ_YMM_K1Z_YMM_YMMM256B64: Code = 3043 # type: ignore
+EVEX_VPSRAVQ_YMM_K1Z_YMM_YMMM256B64: int = 3043
 """
 ``VPSRAVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 46 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSRAVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3044 # type: ignore
+EVEX_VPSRAVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3044
 """
 ``VPSRAVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 46 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLVD_XMM_XMM_XMMM128: Code = 3045 # type: ignore
+VEX_VPSLLVD_XMM_XMM_XMMM128: int = 3045
 """
 ``VPSLLVD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 47 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLVD_YMM_YMM_YMMM256: Code = 3046 # type: ignore
+VEX_VPSLLVD_YMM_YMM_YMMM256: int = 3046
 """
 ``VPSLLVD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 47 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLVQ_XMM_XMM_XMMM128: Code = 3047 # type: ignore
+VEX_VPSLLVQ_XMM_XMM_XMMM128: int = 3047
 """
 ``VPSLLVQ xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 47 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPSLLVQ_YMM_YMM_YMMM256: Code = 3048 # type: ignore
+VEX_VPSLLVQ_YMM_YMM_YMMM256: int = 3048
 """
 ``VPSLLVQ ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 47 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVD_XMM_K1Z_XMM_XMMM128B32: Code = 3049 # type: ignore
+EVEX_VPSLLVD_XMM_K1Z_XMM_XMMM128B32: int = 3049
 """
 ``VPSLLVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 47 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVD_YMM_K1Z_YMM_YMMM256B32: Code = 3050 # type: ignore
+EVEX_VPSLLVD_YMM_K1Z_YMM_YMMM256B32: int = 3050
 """
 ``VPSLLVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 47 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3051 # type: ignore
+EVEX_VPSLLVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3051
 """
 ``VPSLLVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 47 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVQ_XMM_K1Z_XMM_XMMM128B64: Code = 3052 # type: ignore
+EVEX_VPSLLVQ_XMM_K1Z_XMM_XMMM128B64: int = 3052
 """
 ``VPSLLVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 47 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVQ_YMM_K1Z_YMM_YMMM256B64: Code = 3053 # type: ignore
+EVEX_VPSLLVQ_YMM_K1Z_YMM_YMMM256B64: int = 3053
 """
 ``VPSLLVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 47 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSLLVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3054 # type: ignore
+EVEX_VPSLLVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3054
 """
 ``VPSLLVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 47 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PS_XMM_K1Z_XMMM128B32: Code = 3055 # type: ignore
+EVEX_VRCP14PS_XMM_K1Z_XMMM128B32: int = 3055
 """
 ``VRCP14PS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 4C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PS_YMM_K1Z_YMMM256B32: Code = 3056 # type: ignore
+EVEX_VRCP14PS_YMM_K1Z_YMMM256B32: int = 3056
 """
 ``VRCP14PS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 4C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PS_ZMM_K1Z_ZMMM512B32: Code = 3057 # type: ignore
+EVEX_VRCP14PS_ZMM_K1Z_ZMMM512B32: int = 3057
 """
 ``VRCP14PS zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 4C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PD_XMM_K1Z_XMMM128B64: Code = 3058 # type: ignore
+EVEX_VRCP14PD_XMM_K1Z_XMMM128B64: int = 3058
 """
 ``VRCP14PD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 4C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PD_YMM_K1Z_YMMM256B64: Code = 3059 # type: ignore
+EVEX_VRCP14PD_YMM_K1Z_YMMM256B64: int = 3059
 """
 ``VRCP14PD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 4C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14PD_ZMM_K1Z_ZMMM512B64: Code = 3060 # type: ignore
+EVEX_VRCP14PD_ZMM_K1Z_ZMMM512B64: int = 3060
 """
 ``VRCP14PD zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 4C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14SS_XMM_K1Z_XMM_XMMM32: Code = 3061 # type: ignore
+EVEX_VRCP14SS_XMM_K1Z_XMM_XMMM32: int = 3061
 """
 ``VRCP14SS xmm1 {k1}{z}, xmm2, xmm3/m32``
 
 ``EVEX.LIG.66.0F38.W0 4D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP14SD_XMM_K1Z_XMM_XMMM64: Code = 3062 # type: ignore
+EVEX_VRCP14SD_XMM_K1Z_XMM_XMMM64: int = 3062
 """
 ``VRCP14SD xmm1 {k1}{z}, xmm2, xmm3/m64``
 
 ``EVEX.LIG.66.0F38.W1 4D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PS_XMM_K1Z_XMMM128B32: Code = 3063 # type: ignore
+EVEX_VRSQRT14PS_XMM_K1Z_XMMM128B32: int = 3063
 """
 ``VRSQRT14PS xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 4E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PS_YMM_K1Z_YMMM256B32: Code = 3064 # type: ignore
+EVEX_VRSQRT14PS_YMM_K1Z_YMMM256B32: int = 3064
 """
 ``VRSQRT14PS ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 4E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PS_ZMM_K1Z_ZMMM512B32: Code = 3065 # type: ignore
+EVEX_VRSQRT14PS_ZMM_K1Z_ZMMM512B32: int = 3065
 """
 ``VRSQRT14PS zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 4E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PD_XMM_K1Z_XMMM128B64: Code = 3066 # type: ignore
+EVEX_VRSQRT14PD_XMM_K1Z_XMMM128B64: int = 3066
 """
 ``VRSQRT14PD xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 4E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PD_YMM_K1Z_YMMM256B64: Code = 3067 # type: ignore
+EVEX_VRSQRT14PD_YMM_K1Z_YMMM256B64: int = 3067
 """
 ``VRSQRT14PD ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 4E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14PD_ZMM_K1Z_ZMMM512B64: Code = 3068 # type: ignore
+EVEX_VRSQRT14PD_ZMM_K1Z_ZMMM512B64: int = 3068
 """
 ``VRSQRT14PD zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 4E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14SS_XMM_K1Z_XMM_XMMM32: Code = 3069 # type: ignore
+EVEX_VRSQRT14SS_XMM_K1Z_XMM_XMMM32: int = 3069
 """
 ``VRSQRT14SS xmm1 {k1}{z}, xmm2, xmm3/m32``
 
 ``EVEX.LIG.66.0F38.W0 4F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT14SD_XMM_K1Z_XMM_XMMM64: Code = 3070 # type: ignore
+EVEX_VRSQRT14SD_XMM_K1Z_XMM_XMMM64: int = 3070
 """
 ``VRSQRT14SD xmm1 {k1}{z}, xmm2, xmm3/m64``
 
 ``EVEX.LIG.66.0F38.W1 4F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSD_XMM_K1Z_XMM_XMMM128B32: Code = 3071 # type: ignore
+EVEX_VPDPBUSD_XMM_K1Z_XMM_XMMM128B32: int = 3071
 """
 ``VPDPBUSD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 50 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSD_YMM_K1Z_YMM_YMMM256B32: Code = 3072 # type: ignore
+EVEX_VPDPBUSD_YMM_K1Z_YMM_YMMM256B32: int = 3072
 """
 ``VPDPBUSD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 50 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3073 # type: ignore
+EVEX_VPDPBUSD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3073
 """
 ``VPDPBUSD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 50 /r``
 
 ``AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSDS_XMM_K1Z_XMM_XMMM128B32: Code = 3074 # type: ignore
+EVEX_VPDPBUSDS_XMM_K1Z_XMM_XMMM128B32: int = 3074
 """
 ``VPDPBUSDS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 51 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSDS_YMM_K1Z_YMM_YMMM256B32: Code = 3075 # type: ignore
+EVEX_VPDPBUSDS_YMM_K1Z_YMM_YMMM256B32: int = 3075
 """
 ``VPDPBUSDS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 51 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPBUSDS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3076 # type: ignore
+EVEX_VPDPBUSDS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3076
 """
 ``VPDPBUSDS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 51 /r``
 
 ``AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSD_XMM_K1Z_XMM_XMMM128B32: Code = 3077 # type: ignore
+EVEX_VPDPWSSD_XMM_K1Z_XMM_XMMM128B32: int = 3077
 """
 ``VPDPWSSD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 52 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSD_YMM_K1Z_YMM_YMMM256B32: Code = 3078 # type: ignore
+EVEX_VPDPWSSD_YMM_K1Z_YMM_YMMM256B32: int = 3078
 """
 ``VPDPWSSD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 52 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3079 # type: ignore
+EVEX_VPDPWSSD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3079
 """
 ``VPDPWSSD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 52 /r``
 
 ``AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VDPBF16PS_XMM_K1Z_XMM_XMMM128B32: Code = 3080 # type: ignore
+EVEX_VDPBF16PS_XMM_K1Z_XMM_XMMM128B32: int = 3080
 """
 ``VDPBF16PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.F3.0F38.W0 52 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VDPBF16PS_YMM_K1Z_YMM_YMMM256B32: Code = 3081 # type: ignore
+EVEX_VDPBF16PS_YMM_K1Z_YMM_YMMM256B32: int = 3081
 """
 ``VDPBF16PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.F3.0F38.W0 52 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VDPBF16PS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3082 # type: ignore
+EVEX_VDPBF16PS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3082
 """
 ``VDPBF16PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.F3.0F38.W0 52 /r``
 
 ``AVX512F and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VP4DPWSSD_ZMM_K1Z_ZMMP3_M128: Code = 3083 # type: ignore
+EVEX_VP4DPWSSD_ZMM_K1Z_ZMMP3_M128: int = 3083
 """
 ``VP4DPWSSD zmm1 {k1}{z}, zmm2+3, m128``
 
 ``EVEX.512.F2.0F38.W0 52 /r``
 
 ``AVX512_4VNNIW``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSDS_XMM_K1Z_XMM_XMMM128B32: Code = 3084 # type: ignore
+EVEX_VPDPWSSDS_XMM_K1Z_XMM_XMMM128B32: int = 3084
 """
 ``VPDPWSSDS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 53 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSDS_YMM_K1Z_YMM_YMMM256B32: Code = 3085 # type: ignore
+EVEX_VPDPWSSDS_YMM_K1Z_YMM_YMMM256B32: int = 3085
 """
 ``VPDPWSSDS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 53 /r``
 
 ``AVX512VL and AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VPDPWSSDS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3086 # type: ignore
+EVEX_VPDPWSSDS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3086
 """
 ``VPDPWSSDS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 53 /r``
 
 ``AVX512_VNNI``
 
 ``16/32/64-bit``
 """
-EVEX_VP4DPWSSDS_ZMM_K1Z_ZMMP3_M128: Code = 3087 # type: ignore
+EVEX_VP4DPWSSDS_ZMM_K1Z_ZMMP3_M128: int = 3087
 """
 ``VP4DPWSSDS zmm1 {k1}{z}, zmm2+3, m128``
 
 ``EVEX.512.F2.0F38.W0 53 /r``
 
 ``AVX512_4VNNIW``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTB_XMM_K1Z_XMMM128: Code = 3088 # type: ignore
+EVEX_VPOPCNTB_XMM_K1Z_XMMM128: int = 3088
 """
 ``VPOPCNTB xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W0 54 /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTB_YMM_K1Z_YMMM256: Code = 3089 # type: ignore
+EVEX_VPOPCNTB_YMM_K1Z_YMMM256: int = 3089
 """
 ``VPOPCNTB ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W0 54 /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTB_ZMM_K1Z_ZMMM512: Code = 3090 # type: ignore
+EVEX_VPOPCNTB_ZMM_K1Z_ZMMM512: int = 3090
 """
 ``VPOPCNTB zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W0 54 /r``
 
 ``AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTW_XMM_K1Z_XMMM128: Code = 3091 # type: ignore
+EVEX_VPOPCNTW_XMM_K1Z_XMMM128: int = 3091
 """
 ``VPOPCNTW xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W1 54 /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTW_YMM_K1Z_YMMM256: Code = 3092 # type: ignore
+EVEX_VPOPCNTW_YMM_K1Z_YMMM256: int = 3092
 """
 ``VPOPCNTW ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W1 54 /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTW_ZMM_K1Z_ZMMM512: Code = 3093 # type: ignore
+EVEX_VPOPCNTW_ZMM_K1Z_ZMMM512: int = 3093
 """
 ``VPOPCNTW zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W1 54 /r``
 
 ``AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTD_XMM_K1Z_XMMM128B32: Code = 3094 # type: ignore
+EVEX_VPOPCNTD_XMM_K1Z_XMMM128B32: int = 3094
 """
 ``VPOPCNTD xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 55 /r``
 
 ``AVX512VL and AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTD_YMM_K1Z_YMMM256B32: Code = 3095 # type: ignore
+EVEX_VPOPCNTD_YMM_K1Z_YMMM256B32: int = 3095
 """
 ``VPOPCNTD ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 55 /r``
 
 ``AVX512VL and AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTD_ZMM_K1Z_ZMMM512B32: Code = 3096 # type: ignore
+EVEX_VPOPCNTD_ZMM_K1Z_ZMMM512B32: int = 3096
 """
 ``VPOPCNTD zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 55 /r``
 
 ``AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTQ_XMM_K1Z_XMMM128B64: Code = 3097 # type: ignore
+EVEX_VPOPCNTQ_XMM_K1Z_XMMM128B64: int = 3097
 """
 ``VPOPCNTQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 55 /r``
 
 ``AVX512VL and AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTQ_YMM_K1Z_YMMM256B64: Code = 3098 # type: ignore
+EVEX_VPOPCNTQ_YMM_K1Z_YMMM256B64: int = 3098
 """
 ``VPOPCNTQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 55 /r``
 
 ``AVX512VL and AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPOPCNTQ_ZMM_K1Z_ZMMM512B64: Code = 3099 # type: ignore
+EVEX_VPOPCNTQ_ZMM_K1Z_ZMMM512B64: int = 3099
 """
 ``VPOPCNTQ zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 55 /r``
 
 ``AVX512_VPOPCNTDQ``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTD_XMM_XMMM32: Code = 3100 # type: ignore
+VEX_VPBROADCASTD_XMM_XMMM32: int = 3100
 """
 ``VPBROADCASTD xmm1, xmm2/m32``
 
 ``VEX.128.66.0F38.W0 58 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTD_YMM_XMMM32: Code = 3101 # type: ignore
+VEX_VPBROADCASTD_YMM_XMMM32: int = 3101
 """
 ``VPBROADCASTD ymm1, xmm2/m32``
 
 ``VEX.256.66.0F38.W0 58 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_XMM_K1Z_XMMM32: Code = 3102 # type: ignore
+EVEX_VPBROADCASTD_XMM_K1Z_XMMM32: int = 3102
 """
 ``VPBROADCASTD xmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.128.66.0F38.W0 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_YMM_K1Z_XMMM32: Code = 3103 # type: ignore
+EVEX_VPBROADCASTD_YMM_K1Z_XMMM32: int = 3103
 """
 ``VPBROADCASTD ymm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.256.66.0F38.W0 58 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_ZMM_K1Z_XMMM32: Code = 3104 # type: ignore
+EVEX_VPBROADCASTD_ZMM_K1Z_XMMM32: int = 3104
 """
 ``VPBROADCASTD zmm1 {k1}{z}, xmm2/m32``
 
 ``EVEX.512.66.0F38.W0 58 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTQ_XMM_XMMM64: Code = 3105 # type: ignore
+VEX_VPBROADCASTQ_XMM_XMMM64: int = 3105
 """
 ``VPBROADCASTQ xmm1, xmm2/m64``
 
 ``VEX.128.66.0F38.W0 59 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTQ_YMM_XMMM64: Code = 3106 # type: ignore
+VEX_VPBROADCASTQ_YMM_XMMM64: int = 3106
 """
 ``VPBROADCASTQ ymm1, xmm2/m64``
 
 ``VEX.256.66.0F38.W0 59 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X2_XMM_K1Z_XMMM64: Code = 3107 # type: ignore
+EVEX_VBROADCASTI32X2_XMM_K1Z_XMMM64: int = 3107
 """
 ``VBROADCASTI32X2 xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.W0 59 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X2_YMM_K1Z_XMMM64: Code = 3108 # type: ignore
+EVEX_VBROADCASTI32X2_YMM_K1Z_XMMM64: int = 3108
 """
 ``VBROADCASTI32X2 ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.W0 59 /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X2_ZMM_K1Z_XMMM64: Code = 3109 # type: ignore
+EVEX_VBROADCASTI32X2_ZMM_K1Z_XMMM64: int = 3109
 """
 ``VBROADCASTI32X2 zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.W0 59 /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTQ_XMM_K1Z_XMMM64: Code = 3110 # type: ignore
+EVEX_VPBROADCASTQ_XMM_K1Z_XMMM64: int = 3110
 """
 ``VPBROADCASTQ xmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.128.66.0F38.W1 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTQ_YMM_K1Z_XMMM64: Code = 3111 # type: ignore
+EVEX_VPBROADCASTQ_YMM_K1Z_XMMM64: int = 3111
 """
 ``VPBROADCASTQ ymm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.256.66.0F38.W1 59 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTQ_ZMM_K1Z_XMMM64: Code = 3112 # type: ignore
+EVEX_VPBROADCASTQ_ZMM_K1Z_XMMM64: int = 3112
 """
 ``VPBROADCASTQ zmm1 {k1}{z}, xmm2/m64``
 
 ``EVEX.512.66.0F38.W1 59 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTI128_YMM_M128: Code = 3113 # type: ignore
+VEX_VBROADCASTI128_YMM_M128: int = 3113
 """
 ``VBROADCASTI128 ymm1, m128``
 
 ``VEX.256.66.0F38.W0 5A /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X4_YMM_K1Z_M128: Code = 3114 # type: ignore
+EVEX_VBROADCASTI32X4_YMM_K1Z_M128: int = 3114
 """
 ``VBROADCASTI32X4 ymm1 {k1}{z}, m128``
 
 ``EVEX.256.66.0F38.W0 5A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X4_ZMM_K1Z_M128: Code = 3115 # type: ignore
+EVEX_VBROADCASTI32X4_ZMM_K1Z_M128: int = 3115
 """
 ``VBROADCASTI32X4 zmm1 {k1}{z}, m128``
 
 ``EVEX.512.66.0F38.W0 5A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI64X2_YMM_K1Z_M128: Code = 3116 # type: ignore
+EVEX_VBROADCASTI64X2_YMM_K1Z_M128: int = 3116
 """
 ``VBROADCASTI64X2 ymm1 {k1}{z}, m128``
 
 ``EVEX.256.66.0F38.W1 5A /r``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI64X2_ZMM_K1Z_M128: Code = 3117 # type: ignore
+EVEX_VBROADCASTI64X2_ZMM_K1Z_M128: int = 3117
 """
 ``VBROADCASTI64X2 zmm1 {k1}{z}, m128``
 
 ``EVEX.512.66.0F38.W1 5A /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI32X8_ZMM_K1Z_M256: Code = 3118 # type: ignore
+EVEX_VBROADCASTI32X8_ZMM_K1Z_M256: int = 3118
 """
 ``VBROADCASTI32X8 zmm1 {k1}{z}, m256``
 
 ``EVEX.512.66.0F38.W0 5B /r``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VBROADCASTI64X4_ZMM_K1Z_M256: Code = 3119 # type: ignore
+EVEX_VBROADCASTI64X4_ZMM_K1Z_M256: int = 3119
 """
 ``VBROADCASTI64X4 zmm1 {k1}{z}, m256``
 
 ``EVEX.512.66.0F38.W1 5B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDB_XMM_K1Z_XMMM128: Code = 3120 # type: ignore
+EVEX_VPEXPANDB_XMM_K1Z_XMMM128: int = 3120
 """
 ``VPEXPANDB xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W0 62 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDB_YMM_K1Z_YMMM256: Code = 3121 # type: ignore
+EVEX_VPEXPANDB_YMM_K1Z_YMMM256: int = 3121
 """
 ``VPEXPANDB ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W0 62 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDB_ZMM_K1Z_ZMMM512: Code = 3122 # type: ignore
+EVEX_VPEXPANDB_ZMM_K1Z_ZMMM512: int = 3122
 """
 ``VPEXPANDB zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W0 62 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDW_XMM_K1Z_XMMM128: Code = 3123 # type: ignore
+EVEX_VPEXPANDW_XMM_K1Z_XMMM128: int = 3123
 """
 ``VPEXPANDW xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W1 62 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDW_YMM_K1Z_YMMM256: Code = 3124 # type: ignore
+EVEX_VPEXPANDW_YMM_K1Z_YMMM256: int = 3124
 """
 ``VPEXPANDW ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W1 62 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDW_ZMM_K1Z_ZMMM512: Code = 3125 # type: ignore
+EVEX_VPEXPANDW_ZMM_K1Z_ZMMM512: int = 3125
 """
 ``VPEXPANDW zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W1 62 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSB_XMMM128_K1Z_XMM: Code = 3126 # type: ignore
+EVEX_VPCOMPRESSB_XMMM128_K1Z_XMM: int = 3126
 """
 ``VPCOMPRESSB xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W0 63 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSB_YMMM256_K1Z_YMM: Code = 3127 # type: ignore
+EVEX_VPCOMPRESSB_YMMM256_K1Z_YMM: int = 3127
 """
 ``VPCOMPRESSB ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W0 63 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSB_ZMMM512_K1Z_ZMM: Code = 3128 # type: ignore
+EVEX_VPCOMPRESSB_ZMMM512_K1Z_ZMM: int = 3128
 """
 ``VPCOMPRESSB zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W0 63 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSW_XMMM128_K1Z_XMM: Code = 3129 # type: ignore
+EVEX_VPCOMPRESSW_XMMM128_K1Z_XMM: int = 3129
 """
 ``VPCOMPRESSW xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W1 63 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSW_YMMM256_K1Z_YMM: Code = 3130 # type: ignore
+EVEX_VPCOMPRESSW_YMMM256_K1Z_YMM: int = 3130
 """
 ``VPCOMPRESSW ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W1 63 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSW_ZMMM512_K1Z_ZMM: Code = 3131 # type: ignore
+EVEX_VPCOMPRESSW_ZMMM512_K1Z_ZMM: int = 3131
 """
 ``VPCOMPRESSW zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W1 63 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMD_XMM_K1Z_XMM_XMMM128B32: Code = 3132 # type: ignore
+EVEX_VPBLENDMD_XMM_K1Z_XMM_XMMM128B32: int = 3132
 """
 ``VPBLENDMD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 64 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMD_YMM_K1Z_YMM_YMMM256B32: Code = 3133 # type: ignore
+EVEX_VPBLENDMD_YMM_K1Z_YMM_YMMM256B32: int = 3133
 """
 ``VPBLENDMD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 64 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3134 # type: ignore
+EVEX_VPBLENDMD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3134
 """
 ``VPBLENDMD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 64 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMQ_XMM_K1Z_XMM_XMMM128B64: Code = 3135 # type: ignore
+EVEX_VPBLENDMQ_XMM_K1Z_XMM_XMMM128B64: int = 3135
 """
 ``VPBLENDMQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 64 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMQ_YMM_K1Z_YMM_YMMM256B64: Code = 3136 # type: ignore
+EVEX_VPBLENDMQ_YMM_K1Z_YMM_YMMM256B64: int = 3136
 """
 ``VPBLENDMQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 64 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3137 # type: ignore
+EVEX_VPBLENDMQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3137
 """
 ``VPBLENDMQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 64 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPS_XMM_K1Z_XMM_XMMM128B32: Code = 3138 # type: ignore
+EVEX_VBLENDMPS_XMM_K1Z_XMM_XMMM128B32: int = 3138
 """
 ``VBLENDMPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 65 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPS_YMM_K1Z_YMM_YMMM256B32: Code = 3139 # type: ignore
+EVEX_VBLENDMPS_YMM_K1Z_YMM_YMMM256B32: int = 3139
 """
 ``VBLENDMPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 65 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3140 # type: ignore
+EVEX_VBLENDMPS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3140
 """
 ``VBLENDMPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 65 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPD_XMM_K1Z_XMM_XMMM128B64: Code = 3141 # type: ignore
+EVEX_VBLENDMPD_XMM_K1Z_XMM_XMMM128B64: int = 3141
 """
 ``VBLENDMPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 65 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPD_YMM_K1Z_YMM_YMMM256B64: Code = 3142 # type: ignore
+EVEX_VBLENDMPD_YMM_K1Z_YMM_YMMM256B64: int = 3142
 """
 ``VBLENDMPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 65 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VBLENDMPD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3143 # type: ignore
+EVEX_VBLENDMPD_ZMM_K1Z_ZMM_ZMMM512B64: int = 3143
 """
 ``VBLENDMPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 65 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMB_XMM_K1Z_XMM_XMMM128: Code = 3144 # type: ignore
+EVEX_VPBLENDMB_XMM_K1Z_XMM_XMMM128: int = 3144
 """
 ``VPBLENDMB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 66 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMB_YMM_K1Z_YMM_YMMM256: Code = 3145 # type: ignore
+EVEX_VPBLENDMB_YMM_K1Z_YMM_YMMM256: int = 3145
 """
 ``VPBLENDMB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 66 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMB_ZMM_K1Z_ZMM_ZMMM512: Code = 3146 # type: ignore
+EVEX_VPBLENDMB_ZMM_K1Z_ZMM_ZMMM512: int = 3146
 """
 ``VPBLENDMB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 66 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMW_XMM_K1Z_XMM_XMMM128: Code = 3147 # type: ignore
+EVEX_VPBLENDMW_XMM_K1Z_XMM_XMMM128: int = 3147
 """
 ``VPBLENDMW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 66 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMW_YMM_K1Z_YMM_YMMM256: Code = 3148 # type: ignore
+EVEX_VPBLENDMW_YMM_K1Z_YMM_YMMM256: int = 3148
 """
 ``VPBLENDMW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 66 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBLENDMW_ZMM_K1Z_ZMM_ZMMM512: Code = 3149 # type: ignore
+EVEX_VPBLENDMW_ZMM_K1Z_ZMM_ZMMM512: int = 3149
 """
 ``VPBLENDMW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 66 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTD_KP1_XMM_XMMM128B32: Code = 3150 # type: ignore
+EVEX_VP2INTERSECTD_KP1_XMM_XMMM128B32: int = 3150
 """
 ``VP2INTERSECTD k1+1, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.F2.0F38.W0 68 /r``
 
 ``AVX512VL and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTD_KP1_YMM_YMMM256B32: Code = 3151 # type: ignore
+EVEX_VP2INTERSECTD_KP1_YMM_YMMM256B32: int = 3151
 """
 ``VP2INTERSECTD k1+1, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.F2.0F38.W0 68 /r``
 
 ``AVX512VL and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTD_KP1_ZMM_ZMMM512B32: Code = 3152 # type: ignore
+EVEX_VP2INTERSECTD_KP1_ZMM_ZMMM512B32: int = 3152
 """
 ``VP2INTERSECTD k1+1, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.F2.0F38.W0 68 /r``
 
 ``AVX512F and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTQ_KP1_XMM_XMMM128B64: Code = 3153 # type: ignore
+EVEX_VP2INTERSECTQ_KP1_XMM_XMMM128B64: int = 3153
 """
 ``VP2INTERSECTQ k1+1, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.F2.0F38.W1 68 /r``
 
 ``AVX512VL and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTQ_KP1_YMM_YMMM256B64: Code = 3154 # type: ignore
+EVEX_VP2INTERSECTQ_KP1_YMM_YMMM256B64: int = 3154
 """
 ``VP2INTERSECTQ k1+1, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.F2.0F38.W1 68 /r``
 
 ``AVX512VL and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VP2INTERSECTQ_KP1_ZMM_ZMMM512B64: Code = 3155 # type: ignore
+EVEX_VP2INTERSECTQ_KP1_ZMM_ZMMM512B64: int = 3155
 """
 ``VP2INTERSECTQ k1+1, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.F2.0F38.W1 68 /r``
 
 ``AVX512F and AVX512_VP2INTERSECT``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVW_XMM_K1Z_XMM_XMMM128: Code = 3156 # type: ignore
+EVEX_VPSHLDVW_XMM_K1Z_XMM_XMMM128: int = 3156
 """
 ``VPSHLDVW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 70 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVW_YMM_K1Z_YMM_YMMM256: Code = 3157 # type: ignore
+EVEX_VPSHLDVW_YMM_K1Z_YMM_YMMM256: int = 3157
 """
 ``VPSHLDVW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 70 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVW_ZMM_K1Z_ZMM_ZMMM512: Code = 3158 # type: ignore
+EVEX_VPSHLDVW_ZMM_K1Z_ZMM_ZMMM512: int = 3158
 """
 ``VPSHLDVW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 70 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVD_XMM_K1Z_XMM_XMMM128B32: Code = 3159 # type: ignore
+EVEX_VPSHLDVD_XMM_K1Z_XMM_XMMM128B32: int = 3159
 """
 ``VPSHLDVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 71 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVD_YMM_K1Z_YMM_YMMM256B32: Code = 3160 # type: ignore
+EVEX_VPSHLDVD_YMM_K1Z_YMM_YMMM256B32: int = 3160
 """
 ``VPSHLDVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 71 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3161 # type: ignore
+EVEX_VPSHLDVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3161
 """
 ``VPSHLDVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 71 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVQ_XMM_K1Z_XMM_XMMM128B64: Code = 3162 # type: ignore
+EVEX_VPSHLDVQ_XMM_K1Z_XMM_XMMM128B64: int = 3162
 """
 ``VPSHLDVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 71 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVQ_YMM_K1Z_YMM_YMMM256B64: Code = 3163 # type: ignore
+EVEX_VPSHLDVQ_YMM_K1Z_YMM_YMMM256B64: int = 3163
 """
 ``VPSHLDVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 71 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3164 # type: ignore
+EVEX_VPSHLDVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3164
 """
 ``VPSHLDVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 71 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVW_XMM_K1Z_XMM_XMMM128: Code = 3165 # type: ignore
+EVEX_VPSHRDVW_XMM_K1Z_XMM_XMMM128: int = 3165
 """
 ``VPSHRDVW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 72 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVW_YMM_K1Z_YMM_YMMM256: Code = 3166 # type: ignore
+EVEX_VPSHRDVW_YMM_K1Z_YMM_YMMM256: int = 3166
 """
 ``VPSHRDVW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 72 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVW_ZMM_K1Z_ZMM_ZMMM512: Code = 3167 # type: ignore
+EVEX_VPSHRDVW_ZMM_K1Z_ZMM_ZMMM512: int = 3167
 """
 ``VPSHRDVW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 72 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNEPS2BF16_XMM_K1Z_XMMM128B32: Code = 3168 # type: ignore
+EVEX_VCVTNEPS2BF16_XMM_K1Z_XMMM128B32: int = 3168
 """
 ``VCVTNEPS2BF16 xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.F3.0F38.W0 72 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNEPS2BF16_XMM_K1Z_YMMM256B32: Code = 3169 # type: ignore
+EVEX_VCVTNEPS2BF16_XMM_K1Z_YMMM256B32: int = 3169
 """
 ``VCVTNEPS2BF16 xmm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.F3.0F38.W0 72 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNEPS2BF16_YMM_K1Z_ZMMM512B32: Code = 3170 # type: ignore
+EVEX_VCVTNEPS2BF16_YMM_K1Z_ZMMM512B32: int = 3170
 """
 ``VCVTNEPS2BF16 ymm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.F3.0F38.W0 72 /r``
 
 ``AVX512F and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNE2PS2BF16_XMM_K1Z_XMM_XMMM128B32: Code = 3171 # type: ignore
+EVEX_VCVTNE2PS2BF16_XMM_K1Z_XMM_XMMM128B32: int = 3171
 """
 ``VCVTNE2PS2BF16 xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.F2.0F38.W0 72 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNE2PS2BF16_YMM_K1Z_YMM_YMMM256B32: Code = 3172 # type: ignore
+EVEX_VCVTNE2PS2BF16_YMM_K1Z_YMM_YMMM256B32: int = 3172
 """
 ``VCVTNE2PS2BF16 ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.F2.0F38.W0 72 /r``
 
 ``AVX512VL and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTNE2PS2BF16_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3173 # type: ignore
+EVEX_VCVTNE2PS2BF16_ZMM_K1Z_ZMM_ZMMM512B32: int = 3173
 """
 ``VCVTNE2PS2BF16 zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.F2.0F38.W0 72 /r``
 
 ``AVX512F and AVX512_BF16``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVD_XMM_K1Z_XMM_XMMM128B32: Code = 3174 # type: ignore
+EVEX_VPSHRDVD_XMM_K1Z_XMM_XMMM128B32: int = 3174
 """
 ``VPSHRDVD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 73 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVD_YMM_K1Z_YMM_YMMM256B32: Code = 3175 # type: ignore
+EVEX_VPSHRDVD_YMM_K1Z_YMM_YMMM256B32: int = 3175
 """
 ``VPSHRDVD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 73 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVD_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3176 # type: ignore
+EVEX_VPSHRDVD_ZMM_K1Z_ZMM_ZMMM512B32: int = 3176
 """
 ``VPSHRDVD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 73 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVQ_XMM_K1Z_XMM_XMMM128B64: Code = 3177 # type: ignore
+EVEX_VPSHRDVQ_XMM_K1Z_XMM_XMMM128B64: int = 3177
 """
 ``VPSHRDVQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 73 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVQ_YMM_K1Z_YMM_YMMM256B64: Code = 3178 # type: ignore
+EVEX_VPSHRDVQ_YMM_K1Z_YMM_YMMM256B64: int = 3178
 """
 ``VPSHRDVQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 73 /r``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDVQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3179 # type: ignore
+EVEX_VPSHRDVQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3179
 """
 ``VPSHRDVQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 73 /r``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2B_XMM_K1Z_XMM_XMMM128: Code = 3180 # type: ignore
+EVEX_VPERMI2B_XMM_K1Z_XMM_XMMM128: int = 3180
 """
 ``VPERMI2B xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 75 /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2B_YMM_K1Z_YMM_YMMM256: Code = 3181 # type: ignore
+EVEX_VPERMI2B_YMM_K1Z_YMM_YMMM256: int = 3181
 """
 ``VPERMI2B ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 75 /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2B_ZMM_K1Z_ZMM_ZMMM512: Code = 3182 # type: ignore
+EVEX_VPERMI2B_ZMM_K1Z_ZMM_ZMMM512: int = 3182
 """
 ``VPERMI2B zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 75 /r``
 
 ``AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2W_XMM_K1Z_XMM_XMMM128: Code = 3183 # type: ignore
+EVEX_VPERMI2W_XMM_K1Z_XMM_XMMM128: int = 3183
 """
 ``VPERMI2W xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 75 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2W_YMM_K1Z_YMM_YMMM256: Code = 3184 # type: ignore
+EVEX_VPERMI2W_YMM_K1Z_YMM_YMMM256: int = 3184
 """
 ``VPERMI2W ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 75 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2W_ZMM_K1Z_ZMM_ZMMM512: Code = 3185 # type: ignore
+EVEX_VPERMI2W_ZMM_K1Z_ZMM_ZMMM512: int = 3185
 """
 ``VPERMI2W zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 75 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2D_XMM_K1Z_XMM_XMMM128B32: Code = 3186 # type: ignore
+EVEX_VPERMI2D_XMM_K1Z_XMM_XMMM128B32: int = 3186
 """
 ``VPERMI2D xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2D_YMM_K1Z_YMM_YMMM256B32: Code = 3187 # type: ignore
+EVEX_VPERMI2D_YMM_K1Z_YMM_YMMM256B32: int = 3187
 """
 ``VPERMI2D ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2D_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3188 # type: ignore
+EVEX_VPERMI2D_ZMM_K1Z_ZMM_ZMMM512B32: int = 3188
 """
 ``VPERMI2D zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 76 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2Q_XMM_K1Z_XMM_XMMM128B64: Code = 3189 # type: ignore
+EVEX_VPERMI2Q_XMM_K1Z_XMM_XMMM128B64: int = 3189
 """
 ``VPERMI2Q xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2Q_YMM_K1Z_YMM_YMMM256B64: Code = 3190 # type: ignore
+EVEX_VPERMI2Q_YMM_K1Z_YMM_YMMM256B64: int = 3190
 """
 ``VPERMI2Q ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 76 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2Q_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3191 # type: ignore
+EVEX_VPERMI2Q_ZMM_K1Z_ZMM_ZMMM512B64: int = 3191
 """
 ``VPERMI2Q zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 76 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PS_XMM_K1Z_XMM_XMMM128B32: Code = 3192 # type: ignore
+EVEX_VPERMI2PS_XMM_K1Z_XMM_XMMM128B32: int = 3192
 """
 ``VPERMI2PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 77 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PS_YMM_K1Z_YMM_YMMM256B32: Code = 3193 # type: ignore
+EVEX_VPERMI2PS_YMM_K1Z_YMM_YMMM256B32: int = 3193
 """
 ``VPERMI2PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 77 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3194 # type: ignore
+EVEX_VPERMI2PS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3194
 """
 ``VPERMI2PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 77 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PD_XMM_K1Z_XMM_XMMM128B64: Code = 3195 # type: ignore
+EVEX_VPERMI2PD_XMM_K1Z_XMM_XMMM128B64: int = 3195
 """
 ``VPERMI2PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 77 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PD_YMM_K1Z_YMM_YMMM256B64: Code = 3196 # type: ignore
+EVEX_VPERMI2PD_YMM_K1Z_YMM_YMMM256B64: int = 3196
 """
 ``VPERMI2PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 77 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMI2PD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3197 # type: ignore
+EVEX_VPERMI2PD_ZMM_K1Z_ZMM_ZMMM512B64: int = 3197
 """
 ``VPERMI2PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 77 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTB_XMM_XMMM8: Code = 3198 # type: ignore
+VEX_VPBROADCASTB_XMM_XMMM8: int = 3198
 """
 ``VPBROADCASTB xmm1, xmm2/m8``
 
 ``VEX.128.66.0F38.W0 78 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTB_YMM_XMMM8: Code = 3199 # type: ignore
+VEX_VPBROADCASTB_YMM_XMMM8: int = 3199
 """
 ``VPBROADCASTB ymm1, xmm2/m8``
 
 ``VEX.256.66.0F38.W0 78 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_XMM_K1Z_XMMM8: Code = 3200 # type: ignore
+EVEX_VPBROADCASTB_XMM_K1Z_XMMM8: int = 3200
 """
 ``VPBROADCASTB xmm1 {k1}{z}, xmm2/m8``
 
 ``EVEX.128.66.0F38.W0 78 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_YMM_K1Z_XMMM8: Code = 3201 # type: ignore
+EVEX_VPBROADCASTB_YMM_K1Z_XMMM8: int = 3201
 """
 ``VPBROADCASTB ymm1 {k1}{z}, xmm2/m8``
 
 ``EVEX.256.66.0F38.W0 78 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_ZMM_K1Z_XMMM8: Code = 3202 # type: ignore
+EVEX_VPBROADCASTB_ZMM_K1Z_XMMM8: int = 3202
 """
 ``VPBROADCASTB zmm1 {k1}{z}, xmm2/m8``
 
 ``EVEX.512.66.0F38.W0 78 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTW_XMM_XMMM16: Code = 3203 # type: ignore
+VEX_VPBROADCASTW_XMM_XMMM16: int = 3203
 """
 ``VPBROADCASTW xmm1, xmm2/m16``
 
 ``VEX.128.66.0F38.W0 79 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPBROADCASTW_YMM_XMMM16: Code = 3204 # type: ignore
+VEX_VPBROADCASTW_YMM_XMMM16: int = 3204
 """
 ``VPBROADCASTW ymm1, xmm2/m16``
 
 ``VEX.256.66.0F38.W0 79 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_XMM_K1Z_XMMM16: Code = 3205 # type: ignore
+EVEX_VPBROADCASTW_XMM_K1Z_XMMM16: int = 3205
 """
 ``VPBROADCASTW xmm1 {k1}{z}, xmm2/m16``
 
 ``EVEX.128.66.0F38.W0 79 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_YMM_K1Z_XMMM16: Code = 3206 # type: ignore
+EVEX_VPBROADCASTW_YMM_K1Z_XMMM16: int = 3206
 """
 ``VPBROADCASTW ymm1 {k1}{z}, xmm2/m16``
 
 ``EVEX.256.66.0F38.W0 79 /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_ZMM_K1Z_XMMM16: Code = 3207 # type: ignore
+EVEX_VPBROADCASTW_ZMM_K1Z_XMMM16: int = 3207
 """
 ``VPBROADCASTW zmm1 {k1}{z}, xmm2/m16``
 
 ``EVEX.512.66.0F38.W0 79 /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_XMM_K1Z_R32: Code = 3208 # type: ignore
+EVEX_VPBROADCASTB_XMM_K1Z_R32: int = 3208
 """
 ``VPBROADCASTB xmm1 {k1}{z}, r32``
 
 ``EVEX.128.66.0F38.W0 7A /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_YMM_K1Z_R32: Code = 3209 # type: ignore
+EVEX_VPBROADCASTB_YMM_K1Z_R32: int = 3209
 """
 ``VPBROADCASTB ymm1 {k1}{z}, r32``
 
 ``EVEX.256.66.0F38.W0 7A /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTB_ZMM_K1Z_R32: Code = 3210 # type: ignore
+EVEX_VPBROADCASTB_ZMM_K1Z_R32: int = 3210
 """
 ``VPBROADCASTB zmm1 {k1}{z}, r32``
 
 ``EVEX.512.66.0F38.W0 7A /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_XMM_K1Z_R32: Code = 3211 # type: ignore
+EVEX_VPBROADCASTW_XMM_K1Z_R32: int = 3211
 """
 ``VPBROADCASTW xmm1 {k1}{z}, r32``
 
 ``EVEX.128.66.0F38.W0 7B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_YMM_K1Z_R32: Code = 3212 # type: ignore
+EVEX_VPBROADCASTW_YMM_K1Z_R32: int = 3212
 """
 ``VPBROADCASTW ymm1 {k1}{z}, r32``
 
 ``EVEX.256.66.0F38.W0 7B /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTW_ZMM_K1Z_R32: Code = 3213 # type: ignore
+EVEX_VPBROADCASTW_ZMM_K1Z_R32: int = 3213
 """
 ``VPBROADCASTW zmm1 {k1}{z}, r32``
 
 ``EVEX.512.66.0F38.W0 7B /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_XMM_K1Z_R32: Code = 3214 # type: ignore
+EVEX_VPBROADCASTD_XMM_K1Z_R32: int = 3214
 """
 ``VPBROADCASTD xmm1 {k1}{z}, r32``
 
 ``EVEX.128.66.0F38.W0 7C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_YMM_K1Z_R32: Code = 3215 # type: ignore
+EVEX_VPBROADCASTD_YMM_K1Z_R32: int = 3215
 """
 ``VPBROADCASTD ymm1 {k1}{z}, r32``
 
 ``EVEX.256.66.0F38.W0 7C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTD_ZMM_K1Z_R32: Code = 3216 # type: ignore
+EVEX_VPBROADCASTD_ZMM_K1Z_R32: int = 3216
 """
 ``VPBROADCASTD zmm1 {k1}{z}, r32``
 
 ``EVEX.512.66.0F38.W0 7C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPBROADCASTQ_XMM_K1Z_R64: Code = 3217 # type: ignore
+EVEX_VPBROADCASTQ_XMM_K1Z_R64: int = 3217
 """
 ``VPBROADCASTQ xmm1 {k1}{z}, r64``
 
 ``EVEX.128.66.0F38.W1 7C /r``
 
 ``AVX512VL and AVX512F``
 
 ``64-bit``
 """
-EVEX_VPBROADCASTQ_YMM_K1Z_R64: Code = 3218 # type: ignore
+EVEX_VPBROADCASTQ_YMM_K1Z_R64: int = 3218
 """
 ``VPBROADCASTQ ymm1 {k1}{z}, r64``
 
 ``EVEX.256.66.0F38.W1 7C /r``
 
 ``AVX512VL and AVX512F``
 
 ``64-bit``
 """
-EVEX_VPBROADCASTQ_ZMM_K1Z_R64: Code = 3219 # type: ignore
+EVEX_VPBROADCASTQ_ZMM_K1Z_R64: int = 3219
 """
 ``VPBROADCASTQ zmm1 {k1}{z}, r64``
 
 ``EVEX.512.66.0F38.W1 7C /r``
 
 ``AVX512F``
 
 ``64-bit``
 """
-EVEX_VPERMT2B_XMM_K1Z_XMM_XMMM128: Code = 3220 # type: ignore
+EVEX_VPERMT2B_XMM_K1Z_XMM_XMMM128: int = 3220
 """
 ``VPERMT2B xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 7D /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2B_YMM_K1Z_YMM_YMMM256: Code = 3221 # type: ignore
+EVEX_VPERMT2B_YMM_K1Z_YMM_YMMM256: int = 3221
 """
 ``VPERMT2B ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 7D /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2B_ZMM_K1Z_ZMM_ZMMM512: Code = 3222 # type: ignore
+EVEX_VPERMT2B_ZMM_K1Z_ZMM_ZMMM512: int = 3222
 """
 ``VPERMT2B zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 7D /r``
 
 ``AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2W_XMM_K1Z_XMM_XMMM128: Code = 3223 # type: ignore
+EVEX_VPERMT2W_XMM_K1Z_XMM_XMMM128: int = 3223
 """
 ``VPERMT2W xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 7D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2W_YMM_K1Z_YMM_YMMM256: Code = 3224 # type: ignore
+EVEX_VPERMT2W_YMM_K1Z_YMM_YMMM256: int = 3224
 """
 ``VPERMT2W ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 7D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2W_ZMM_K1Z_ZMM_ZMMM512: Code = 3225 # type: ignore
+EVEX_VPERMT2W_ZMM_K1Z_ZMM_ZMMM512: int = 3225
 """
 ``VPERMT2W zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 7D /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2D_XMM_K1Z_XMM_XMMM128B32: Code = 3226 # type: ignore
+EVEX_VPERMT2D_XMM_K1Z_XMM_XMMM128B32: int = 3226
 """
 ``VPERMT2D xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 7E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2D_YMM_K1Z_YMM_YMMM256B32: Code = 3227 # type: ignore
+EVEX_VPERMT2D_YMM_K1Z_YMM_YMMM256B32: int = 3227
 """
 ``VPERMT2D ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 7E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2D_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3228 # type: ignore
+EVEX_VPERMT2D_ZMM_K1Z_ZMM_ZMMM512B32: int = 3228
 """
 ``VPERMT2D zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 7E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2Q_XMM_K1Z_XMM_XMMM128B64: Code = 3229 # type: ignore
+EVEX_VPERMT2Q_XMM_K1Z_XMM_XMMM128B64: int = 3229
 """
 ``VPERMT2Q xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 7E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2Q_YMM_K1Z_YMM_YMMM256B64: Code = 3230 # type: ignore
+EVEX_VPERMT2Q_YMM_K1Z_YMM_YMMM256B64: int = 3230
 """
 ``VPERMT2Q ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 7E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2Q_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3231 # type: ignore
+EVEX_VPERMT2Q_ZMM_K1Z_ZMM_ZMMM512B64: int = 3231
 """
 ``VPERMT2Q zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 7E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PS_XMM_K1Z_XMM_XMMM128B32: Code = 3232 # type: ignore
+EVEX_VPERMT2PS_XMM_K1Z_XMM_XMMM128B32: int = 3232
 """
 ``VPERMT2PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PS_YMM_K1Z_YMM_YMMM256B32: Code = 3233 # type: ignore
+EVEX_VPERMT2PS_YMM_K1Z_YMM_YMMM256B32: int = 3233
 """
 ``VPERMT2PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PS_ZMM_K1Z_ZMM_ZMMM512B32: Code = 3234 # type: ignore
+EVEX_VPERMT2PS_ZMM_K1Z_ZMM_ZMMM512B32: int = 3234
 """
 ``VPERMT2PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PD_XMM_K1Z_XMM_XMMM128B64: Code = 3235 # type: ignore
+EVEX_VPERMT2PD_XMM_K1Z_XMM_XMMM128B64: int = 3235
 """
 ``VPERMT2PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PD_YMM_K1Z_YMM_YMMM256B64: Code = 3236 # type: ignore
+EVEX_VPERMT2PD_YMM_K1Z_YMM_YMMM256B64: int = 3236
 """
 ``VPERMT2PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 7F /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMT2PD_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3237 # type: ignore
+EVEX_VPERMT2PD_ZMM_K1Z_ZMM_ZMMM512B64: int = 3237
 """
 ``VPERMT2PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 7F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-INVEPT_R32_M128: Code = 3238 # type: ignore
+INVEPT_R32_M128: int = 3238
 """
 ``INVEPT r32, m128``
 
 ``66 0F 38 80 /r``
 
 ``VMX and IA32_VMX_EPT_VPID_CAP[bit 20]``
 
 ``16/32-bit``
 """
-INVEPT_R64_M128: Code = 3239 # type: ignore
+INVEPT_R64_M128: int = 3239
 """
 ``INVEPT r64, m128``
 
 ``66 0F 38 80 /r``
 
 ``VMX and IA32_VMX_EPT_VPID_CAP[bit 20]``
 
 ``64-bit``
 """
-INVVPID_R32_M128: Code = 3240 # type: ignore
+INVVPID_R32_M128: int = 3240
 """
 ``INVVPID r32, m128``
 
 ``66 0F 38 81 /r``
 
 ``VMX and IA32_VMX_EPT_VPID_CAP[bit 32]``
 
 ``16/32-bit``
 """
-INVVPID_R64_M128: Code = 3241 # type: ignore
+INVVPID_R64_M128: int = 3241
 """
 ``INVVPID r64, m128``
 
 ``66 0F 38 81 /r``
 
 ``VMX and IA32_VMX_EPT_VPID_CAP[bit 32]``
 
 ``64-bit``
 """
-INVPCID_R32_M128: Code = 3242 # type: ignore
+INVPCID_R32_M128: int = 3242
 """
 ``INVPCID r32, m128``
 
 ``66 0F 38 82 /r``
 
 ``INVPCID``
 
 ``16/32-bit``
 """
-INVPCID_R64_M128: Code = 3243 # type: ignore
+INVPCID_R64_M128: int = 3243
 """
 ``INVPCID r64, m128``
 
 ``66 0F 38 82 /r``
 
 ``INVPCID``
 
 ``64-bit``
 """
-EVEX_VPMULTISHIFTQB_XMM_K1Z_XMM_XMMM128B64: Code = 3244 # type: ignore
+EVEX_VPMULTISHIFTQB_XMM_K1Z_XMM_XMMM128B64: int = 3244
 """
 ``VPMULTISHIFTQB xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 83 /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULTISHIFTQB_YMM_K1Z_YMM_YMMM256B64: Code = 3245 # type: ignore
+EVEX_VPMULTISHIFTQB_YMM_K1Z_YMM_YMMM256B64: int = 3245
 """
 ``VPMULTISHIFTQB ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 83 /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPMULTISHIFTQB_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3246 # type: ignore
+EVEX_VPMULTISHIFTQB_ZMM_K1Z_ZMM_ZMMM512B64: int = 3246
 """
 ``VPMULTISHIFTQB zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 83 /r``
 
 ``AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPS_XMM_K1Z_XMMM128: Code = 3247 # type: ignore
+EVEX_VEXPANDPS_XMM_K1Z_XMMM128: int = 3247
 """
 ``VEXPANDPS xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W0 88 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPS_YMM_K1Z_YMMM256: Code = 3248 # type: ignore
+EVEX_VEXPANDPS_YMM_K1Z_YMMM256: int = 3248
 """
 ``VEXPANDPS ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W0 88 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPS_ZMM_K1Z_ZMMM512: Code = 3249 # type: ignore
+EVEX_VEXPANDPS_ZMM_K1Z_ZMMM512: int = 3249
 """
 ``VEXPANDPS zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W0 88 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPD_XMM_K1Z_XMMM128: Code = 3250 # type: ignore
+EVEX_VEXPANDPD_XMM_K1Z_XMMM128: int = 3250
 """
 ``VEXPANDPD xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W1 88 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPD_YMM_K1Z_YMMM256: Code = 3251 # type: ignore
+EVEX_VEXPANDPD_YMM_K1Z_YMMM256: int = 3251
 """
 ``VEXPANDPD ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W1 88 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXPANDPD_ZMM_K1Z_ZMMM512: Code = 3252 # type: ignore
+EVEX_VEXPANDPD_ZMM_K1Z_ZMMM512: int = 3252
 """
 ``VEXPANDPD zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W1 88 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDD_XMM_K1Z_XMMM128: Code = 3253 # type: ignore
+EVEX_VPEXPANDD_XMM_K1Z_XMMM128: int = 3253
 """
 ``VPEXPANDD xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W0 89 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDD_YMM_K1Z_YMMM256: Code = 3254 # type: ignore
+EVEX_VPEXPANDD_YMM_K1Z_YMMM256: int = 3254
 """
 ``VPEXPANDD ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W0 89 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDD_ZMM_K1Z_ZMMM512: Code = 3255 # type: ignore
+EVEX_VPEXPANDD_ZMM_K1Z_ZMMM512: int = 3255
 """
 ``VPEXPANDD zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W0 89 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDQ_XMM_K1Z_XMMM128: Code = 3256 # type: ignore
+EVEX_VPEXPANDQ_XMM_K1Z_XMMM128: int = 3256
 """
 ``VPEXPANDQ xmm1 {k1}{z}, xmm2/m128``
 
 ``EVEX.128.66.0F38.W1 89 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDQ_YMM_K1Z_YMMM256: Code = 3257 # type: ignore
+EVEX_VPEXPANDQ_YMM_K1Z_YMMM256: int = 3257
 """
 ``VPEXPANDQ ymm1 {k1}{z}, ymm2/m256``
 
 ``EVEX.256.66.0F38.W1 89 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXPANDQ_ZMM_K1Z_ZMMM512: Code = 3258 # type: ignore
+EVEX_VPEXPANDQ_ZMM_K1Z_ZMMM512: int = 3258
 """
 ``VPEXPANDQ zmm1 {k1}{z}, zmm2/m512``
 
 ``EVEX.512.66.0F38.W1 89 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPS_XMMM128_K1Z_XMM: Code = 3259 # type: ignore
+EVEX_VCOMPRESSPS_XMMM128_K1Z_XMM: int = 3259
 """
 ``VCOMPRESSPS xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W0 8A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPS_YMMM256_K1Z_YMM: Code = 3260 # type: ignore
+EVEX_VCOMPRESSPS_YMMM256_K1Z_YMM: int = 3260
 """
 ``VCOMPRESSPS ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W0 8A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPS_ZMMM512_K1Z_ZMM: Code = 3261 # type: ignore
+EVEX_VCOMPRESSPS_ZMMM512_K1Z_ZMM: int = 3261
 """
 ``VCOMPRESSPS zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W0 8A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPD_XMMM128_K1Z_XMM: Code = 3262 # type: ignore
+EVEX_VCOMPRESSPD_XMMM128_K1Z_XMM: int = 3262
 """
 ``VCOMPRESSPD xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W1 8A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPD_YMMM256_K1Z_YMM: Code = 3263 # type: ignore
+EVEX_VCOMPRESSPD_YMMM256_K1Z_YMM: int = 3263
 """
 ``VCOMPRESSPD ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W1 8A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCOMPRESSPD_ZMMM512_K1Z_ZMM: Code = 3264 # type: ignore
+EVEX_VCOMPRESSPD_ZMMM512_K1Z_ZMM: int = 3264
 """
 ``VCOMPRESSPD zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W1 8A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSD_XMMM128_K1Z_XMM: Code = 3265 # type: ignore
+EVEX_VPCOMPRESSD_XMMM128_K1Z_XMM: int = 3265
 """
 ``VPCOMPRESSD xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W0 8B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSD_YMMM256_K1Z_YMM: Code = 3266 # type: ignore
+EVEX_VPCOMPRESSD_YMMM256_K1Z_YMM: int = 3266
 """
 ``VPCOMPRESSD ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W0 8B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSD_ZMMM512_K1Z_ZMM: Code = 3267 # type: ignore
+EVEX_VPCOMPRESSD_ZMMM512_K1Z_ZMM: int = 3267
 """
 ``VPCOMPRESSD zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W0 8B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSQ_XMMM128_K1Z_XMM: Code = 3268 # type: ignore
+EVEX_VPCOMPRESSQ_XMMM128_K1Z_XMM: int = 3268
 """
 ``VPCOMPRESSQ xmm1/m128 {k1}{z}, xmm2``
 
 ``EVEX.128.66.0F38.W1 8B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSQ_YMMM256_K1Z_YMM: Code = 3269 # type: ignore
+EVEX_VPCOMPRESSQ_YMMM256_K1Z_YMM: int = 3269
 """
 ``VPCOMPRESSQ ymm1/m256 {k1}{z}, ymm2``
 
 ``EVEX.256.66.0F38.W1 8B /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCOMPRESSQ_ZMMM512_K1Z_ZMM: Code = 3270 # type: ignore
+EVEX_VPCOMPRESSQ_ZMMM512_K1Z_ZMM: int = 3270
 """
 ``VPCOMPRESSQ zmm1/m512 {k1}{z}, zmm2``
 
 ``EVEX.512.66.0F38.W1 8B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVD_XMM_XMM_M128: Code = 3271 # type: ignore
+VEX_VPMASKMOVD_XMM_XMM_M128: int = 3271
 """
 ``VPMASKMOVD xmm1, xmm2, m128``
 
 ``VEX.128.66.0F38.W0 8C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVD_YMM_YMM_M256: Code = 3272 # type: ignore
+VEX_VPMASKMOVD_YMM_YMM_M256: int = 3272
 """
 ``VPMASKMOVD ymm1, ymm2, m256``
 
 ``VEX.256.66.0F38.W0 8C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVQ_XMM_XMM_M128: Code = 3273 # type: ignore
+VEX_VPMASKMOVQ_XMM_XMM_M128: int = 3273
 """
 ``VPMASKMOVQ xmm1, xmm2, m128``
 
 ``VEX.128.66.0F38.W1 8C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVQ_YMM_YMM_M256: Code = 3274 # type: ignore
+VEX_VPMASKMOVQ_YMM_YMM_M256: int = 3274
 """
 ``VPMASKMOVQ ymm1, ymm2, m256``
 
 ``VEX.256.66.0F38.W1 8C /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMB_XMM_K1Z_XMM_XMMM128: Code = 3275 # type: ignore
+EVEX_VPERMB_XMM_K1Z_XMM_XMMM128: int = 3275
 """
 ``VPERMB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 8D /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMB_YMM_K1Z_YMM_YMMM256: Code = 3276 # type: ignore
+EVEX_VPERMB_YMM_K1Z_YMM_YMMM256: int = 3276
 """
 ``VPERMB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 8D /r``
 
 ``AVX512VL and AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMB_ZMM_K1Z_ZMM_ZMMM512: Code = 3277 # type: ignore
+EVEX_VPERMB_ZMM_K1Z_ZMM_ZMMM512: int = 3277
 """
 ``VPERMB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 8D /r``
 
 ``AVX512_VBMI``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMW_XMM_K1Z_XMM_XMMM128: Code = 3278 # type: ignore
+EVEX_VPERMW_XMM_K1Z_XMM_XMMM128: int = 3278
 """
 ``VPERMW xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W1 8D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMW_YMM_K1Z_YMM_YMMM256: Code = 3279 # type: ignore
+EVEX_VPERMW_YMM_K1Z_YMM_YMMM256: int = 3279
 """
 ``VPERMW ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W1 8D /r``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMW_ZMM_K1Z_ZMM_ZMMM512: Code = 3280 # type: ignore
+EVEX_VPERMW_ZMM_K1Z_ZMM_ZMMM512: int = 3280
 """
 ``VPERMW zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W1 8D /r``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVD_M128_XMM_XMM: Code = 3281 # type: ignore
+VEX_VPMASKMOVD_M128_XMM_XMM: int = 3281
 """
 ``VPMASKMOVD m128, xmm1, xmm2``
 
 ``VEX.128.66.0F38.W0 8E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVD_M256_YMM_YMM: Code = 3282 # type: ignore
+VEX_VPMASKMOVD_M256_YMM_YMM: int = 3282
 """
 ``VPMASKMOVD m256, ymm1, ymm2``
 
 ``VEX.256.66.0F38.W0 8E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVQ_M128_XMM_XMM: Code = 3283 # type: ignore
+VEX_VPMASKMOVQ_M128_XMM_XMM: int = 3283
 """
 ``VPMASKMOVQ m128, xmm1, xmm2``
 
 ``VEX.128.66.0F38.W1 8E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPMASKMOVQ_M256_YMM_YMM: Code = 3284 # type: ignore
+VEX_VPMASKMOVQ_M256_YMM_YMM: int = 3284
 """
 ``VPMASKMOVQ m256, ymm1, ymm2``
 
 ``VEX.256.66.0F38.W1 8E /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFBITQMB_KR_K1_XMM_XMMM128: Code = 3285 # type: ignore
+EVEX_VPSHUFBITQMB_KR_K1_XMM_XMMM128: int = 3285
 """
 ``VPSHUFBITQMB k1 {k2}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 8F /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFBITQMB_KR_K1_YMM_YMMM256: Code = 3286 # type: ignore
+EVEX_VPSHUFBITQMB_KR_K1_YMM_YMMM256: int = 3286
 """
 ``VPSHUFBITQMB k1 {k2}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 8F /r``
 
 ``AVX512VL and AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHUFBITQMB_KR_K1_ZMM_ZMMM512: Code = 3287 # type: ignore
+EVEX_VPSHUFBITQMB_KR_K1_ZMM_ZMMM512: int = 3287
 """
 ``VPSHUFBITQMB k1 {k2}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 8F /r``
 
 ``AVX512_BITALG``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERDD_XMM_VM32X_XMM: Code = 3288 # type: ignore
+VEX_VPGATHERDD_XMM_VM32X_XMM: int = 3288
 """
 ``VPGATHERDD xmm1, vm32x, xmm2``
 
 ``VEX.128.66.0F38.W0 90 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERDD_YMM_VM32Y_YMM: Code = 3289 # type: ignore
+VEX_VPGATHERDD_YMM_VM32Y_YMM: int = 3289
 """
 ``VPGATHERDD ymm1, vm32y, ymm2``
 
 ``VEX.256.66.0F38.W0 90 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERDQ_XMM_VM32X_XMM: Code = 3290 # type: ignore
+VEX_VPGATHERDQ_XMM_VM32X_XMM: int = 3290
 """
 ``VPGATHERDQ xmm1, vm32x, xmm2``
 
 ``VEX.128.66.0F38.W1 90 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERDQ_YMM_VM32X_YMM: Code = 3291 # type: ignore
+VEX_VPGATHERDQ_YMM_VM32X_YMM: int = 3291
 """
 ``VPGATHERDQ ymm1, vm32x, ymm2``
 
 ``VEX.256.66.0F38.W1 90 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDD_XMM_K1_VM32X: Code = 3292 # type: ignore
+EVEX_VPGATHERDD_XMM_K1_VM32X: int = 3292
 """
 ``VPGATHERDD xmm1 {k1}, vm32x``
 
 ``EVEX.128.66.0F38.W0 90 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDD_YMM_K1_VM32Y: Code = 3293 # type: ignore
+EVEX_VPGATHERDD_YMM_K1_VM32Y: int = 3293
 """
 ``VPGATHERDD ymm1 {k1}, vm32y``
 
 ``EVEX.256.66.0F38.W0 90 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDD_ZMM_K1_VM32Z: Code = 3294 # type: ignore
+EVEX_VPGATHERDD_ZMM_K1_VM32Z: int = 3294
 """
 ``VPGATHERDD zmm1 {k1}, vm32z``
 
 ``EVEX.512.66.0F38.W0 90 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDQ_XMM_K1_VM32X: Code = 3295 # type: ignore
+EVEX_VPGATHERDQ_XMM_K1_VM32X: int = 3295
 """
 ``VPGATHERDQ xmm1 {k1}, vm32x``
 
 ``EVEX.128.66.0F38.W1 90 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDQ_YMM_K1_VM32X: Code = 3296 # type: ignore
+EVEX_VPGATHERDQ_YMM_K1_VM32X: int = 3296
 """
 ``VPGATHERDQ ymm1 {k1}, vm32x``
 
 ``EVEX.256.66.0F38.W1 90 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERDQ_ZMM_K1_VM32Y: Code = 3297 # type: ignore
+EVEX_VPGATHERDQ_ZMM_K1_VM32Y: int = 3297
 """
 ``VPGATHERDQ zmm1 {k1}, vm32y``
 
 ``EVEX.512.66.0F38.W1 90 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERQD_XMM_VM64X_XMM: Code = 3298 # type: ignore
+VEX_VPGATHERQD_XMM_VM64X_XMM: int = 3298
 """
 ``VPGATHERQD xmm1, vm64x, xmm2``
 
 ``VEX.128.66.0F38.W0 91 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERQD_XMM_VM64Y_XMM: Code = 3299 # type: ignore
+VEX_VPGATHERQD_XMM_VM64Y_XMM: int = 3299
 """
 ``VPGATHERQD xmm1, vm64y, xmm2``
 
 ``VEX.256.66.0F38.W0 91 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERQQ_XMM_VM64X_XMM: Code = 3300 # type: ignore
+VEX_VPGATHERQQ_XMM_VM64X_XMM: int = 3300
 """
 ``VPGATHERQQ xmm1, vm64x, xmm2``
 
 ``VEX.128.66.0F38.W1 91 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPGATHERQQ_YMM_VM64Y_YMM: Code = 3301 # type: ignore
+VEX_VPGATHERQQ_YMM_VM64Y_YMM: int = 3301
 """
 ``VPGATHERQQ ymm1, vm64y, ymm2``
 
 ``VEX.256.66.0F38.W1 91 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQD_XMM_K1_VM64X: Code = 3302 # type: ignore
+EVEX_VPGATHERQD_XMM_K1_VM64X: int = 3302
 """
 ``VPGATHERQD xmm1 {k1}, vm64x``
 
 ``EVEX.128.66.0F38.W0 91 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQD_XMM_K1_VM64Y: Code = 3303 # type: ignore
+EVEX_VPGATHERQD_XMM_K1_VM64Y: int = 3303
 """
 ``VPGATHERQD xmm1 {k1}, vm64y``
 
 ``EVEX.256.66.0F38.W0 91 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQD_YMM_K1_VM64Z: Code = 3304 # type: ignore
+EVEX_VPGATHERQD_YMM_K1_VM64Z: int = 3304
 """
 ``VPGATHERQD ymm1 {k1}, vm64z``
 
 ``EVEX.512.66.0F38.W0 91 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQQ_XMM_K1_VM64X: Code = 3305 # type: ignore
+EVEX_VPGATHERQQ_XMM_K1_VM64X: int = 3305
 """
 ``VPGATHERQQ xmm1 {k1}, vm64x``
 
 ``EVEX.128.66.0F38.W1 91 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQQ_YMM_K1_VM64Y: Code = 3306 # type: ignore
+EVEX_VPGATHERQQ_YMM_K1_VM64Y: int = 3306
 """
 ``VPGATHERQQ ymm1 {k1}, vm64y``
 
 ``EVEX.256.66.0F38.W1 91 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPGATHERQQ_ZMM_K1_VM64Z: Code = 3307 # type: ignore
+EVEX_VPGATHERQQ_ZMM_K1_VM64Z: int = 3307
 """
 ``VPGATHERQQ zmm1 {k1}, vm64z``
 
 ``EVEX.512.66.0F38.W1 91 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERDPS_XMM_VM32X_XMM: Code = 3308 # type: ignore
+VEX_VGATHERDPS_XMM_VM32X_XMM: int = 3308
 """
 ``VGATHERDPS xmm1, vm32x, xmm2``
 
 ``VEX.128.66.0F38.W0 92 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERDPS_YMM_VM32Y_YMM: Code = 3309 # type: ignore
+VEX_VGATHERDPS_YMM_VM32Y_YMM: int = 3309
 """
 ``VGATHERDPS ymm1, vm32y, ymm2``
 
 ``VEX.256.66.0F38.W0 92 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERDPD_XMM_VM32X_XMM: Code = 3310 # type: ignore
+VEX_VGATHERDPD_XMM_VM32X_XMM: int = 3310
 """
 ``VGATHERDPD xmm1, vm32x, xmm2``
 
 ``VEX.128.66.0F38.W1 92 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERDPD_YMM_VM32X_YMM: Code = 3311 # type: ignore
+VEX_VGATHERDPD_YMM_VM32X_YMM: int = 3311
 """
 ``VGATHERDPD ymm1, vm32x, ymm2``
 
 ``VEX.256.66.0F38.W1 92 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPS_XMM_K1_VM32X: Code = 3312 # type: ignore
+EVEX_VGATHERDPS_XMM_K1_VM32X: int = 3312
 """
 ``VGATHERDPS xmm1 {k1}, vm32x``
 
 ``EVEX.128.66.0F38.W0 92 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPS_YMM_K1_VM32Y: Code = 3313 # type: ignore
+EVEX_VGATHERDPS_YMM_K1_VM32Y: int = 3313
 """
 ``VGATHERDPS ymm1 {k1}, vm32y``
 
 ``EVEX.256.66.0F38.W0 92 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPS_ZMM_K1_VM32Z: Code = 3314 # type: ignore
+EVEX_VGATHERDPS_ZMM_K1_VM32Z: int = 3314
 """
 ``VGATHERDPS zmm1 {k1}, vm32z``
 
 ``EVEX.512.66.0F38.W0 92 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPD_XMM_K1_VM32X: Code = 3315 # type: ignore
+EVEX_VGATHERDPD_XMM_K1_VM32X: int = 3315
 """
 ``VGATHERDPD xmm1 {k1}, vm32x``
 
 ``EVEX.128.66.0F38.W1 92 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPD_YMM_K1_VM32X: Code = 3316 # type: ignore
+EVEX_VGATHERDPD_YMM_K1_VM32X: int = 3316
 """
 ``VGATHERDPD ymm1 {k1}, vm32x``
 
 ``EVEX.256.66.0F38.W1 92 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERDPD_ZMM_K1_VM32Y: Code = 3317 # type: ignore
+EVEX_VGATHERDPD_ZMM_K1_VM32Y: int = 3317
 """
 ``VGATHERDPD zmm1 {k1}, vm32y``
 
 ``EVEX.512.66.0F38.W1 92 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERQPS_XMM_VM64X_XMM: Code = 3318 # type: ignore
+VEX_VGATHERQPS_XMM_VM64X_XMM: int = 3318
 """
 ``VGATHERQPS xmm1, vm64x, xmm2``
 
 ``VEX.128.66.0F38.W0 93 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERQPS_XMM_VM64Y_XMM: Code = 3319 # type: ignore
+VEX_VGATHERQPS_XMM_VM64Y_XMM: int = 3319
 """
 ``VGATHERQPS xmm1, vm64y, xmm2``
 
 ``VEX.256.66.0F38.W0 93 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERQPD_XMM_VM64X_XMM: Code = 3320 # type: ignore
+VEX_VGATHERQPD_XMM_VM64X_XMM: int = 3320
 """
 ``VGATHERQPD xmm1, vm64x, xmm2``
 
 ``VEX.128.66.0F38.W1 93 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VGATHERQPD_YMM_VM64Y_YMM: Code = 3321 # type: ignore
+VEX_VGATHERQPD_YMM_VM64Y_YMM: int = 3321
 """
 ``VGATHERQPD ymm1, vm64y, ymm2``
 
 ``VEX.256.66.0F38.W1 93 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPS_XMM_K1_VM64X: Code = 3322 # type: ignore
+EVEX_VGATHERQPS_XMM_K1_VM64X: int = 3322
 """
 ``VGATHERQPS xmm1 {k1}, vm64x``
 
 ``EVEX.128.66.0F38.W0 93 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPS_XMM_K1_VM64Y: Code = 3323 # type: ignore
+EVEX_VGATHERQPS_XMM_K1_VM64Y: int = 3323
 """
 ``VGATHERQPS xmm1 {k1}, vm64y``
 
 ``EVEX.256.66.0F38.W0 93 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPS_YMM_K1_VM64Z: Code = 3324 # type: ignore
+EVEX_VGATHERQPS_YMM_K1_VM64Z: int = 3324
 """
 ``VGATHERQPS ymm1 {k1}, vm64z``
 
 ``EVEX.512.66.0F38.W0 93 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPD_XMM_K1_VM64X: Code = 3325 # type: ignore
+EVEX_VGATHERQPD_XMM_K1_VM64X: int = 3325
 """
 ``VGATHERQPD xmm1 {k1}, vm64x``
 
 ``EVEX.128.66.0F38.W1 93 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPD_YMM_K1_VM64Y: Code = 3326 # type: ignore
+EVEX_VGATHERQPD_YMM_K1_VM64Y: int = 3326
 """
 ``VGATHERQPD ymm1 {k1}, vm64y``
 
 ``EVEX.256.66.0F38.W1 93 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERQPD_ZMM_K1_VM64Z: Code = 3327 # type: ignore
+EVEX_VGATHERQPD_ZMM_K1_VM64Z: int = 3327
 """
 ``VGATHERQPD zmm1 {k1}, vm64z``
 
 ``EVEX.512.66.0F38.W1 93 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB132PS_XMM_XMM_XMMM128: Code = 3328 # type: ignore
+VEX_VFMADDSUB132PS_XMM_XMM_XMMM128: int = 3328
 """
 ``VFMADDSUB132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 96 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB132PS_YMM_YMM_YMMM256: Code = 3329 # type: ignore
+VEX_VFMADDSUB132PS_YMM_YMM_YMMM256: int = 3329
 """
 ``VFMADDSUB132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 96 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB132PD_XMM_XMM_XMMM128: Code = 3330 # type: ignore
+VEX_VFMADDSUB132PD_XMM_XMM_XMMM128: int = 3330
 """
 ``VFMADDSUB132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 96 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB132PD_YMM_YMM_YMMM256: Code = 3331 # type: ignore
+VEX_VFMADDSUB132PD_YMM_YMM_YMMM256: int = 3331
 """
 ``VFMADDSUB132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 96 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3332 # type: ignore
+EVEX_VFMADDSUB132PS_XMM_K1Z_XMM_XMMM128B32: int = 3332
 """
 ``VFMADDSUB132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 96 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3333 # type: ignore
+EVEX_VFMADDSUB132PS_YMM_K1Z_YMM_YMMM256B32: int = 3333
 """
 ``VFMADDSUB132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 96 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3334 # type: ignore
+EVEX_VFMADDSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3334
 """
 ``VFMADDSUB132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 96 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3335 # type: ignore
+EVEX_VFMADDSUB132PD_XMM_K1Z_XMM_XMMM128B64: int = 3335
 """
 ``VFMADDSUB132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 96 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3336 # type: ignore
+EVEX_VFMADDSUB132PD_YMM_K1Z_YMM_YMMM256B64: int = 3336
 """
 ``VFMADDSUB132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 96 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3337 # type: ignore
+EVEX_VFMADDSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3337
 """
 ``VFMADDSUB132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 96 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD132PS_XMM_XMM_XMMM128: Code = 3338 # type: ignore
+VEX_VFMSUBADD132PS_XMM_XMM_XMMM128: int = 3338
 """
 ``VFMSUBADD132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 97 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD132PS_YMM_YMM_YMMM256: Code = 3339 # type: ignore
+VEX_VFMSUBADD132PS_YMM_YMM_YMMM256: int = 3339
 """
 ``VFMSUBADD132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 97 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD132PD_XMM_XMM_XMMM128: Code = 3340 # type: ignore
+VEX_VFMSUBADD132PD_XMM_XMM_XMMM128: int = 3340
 """
 ``VFMSUBADD132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 97 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD132PD_YMM_YMM_YMMM256: Code = 3341 # type: ignore
+VEX_VFMSUBADD132PD_YMM_YMM_YMMM256: int = 3341
 """
 ``VFMSUBADD132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 97 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3342 # type: ignore
+EVEX_VFMSUBADD132PS_XMM_K1Z_XMM_XMMM128B32: int = 3342
 """
 ``VFMSUBADD132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 97 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3343 # type: ignore
+EVEX_VFMSUBADD132PS_YMM_K1Z_YMM_YMMM256B32: int = 3343
 """
 ``VFMSUBADD132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 97 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3344 # type: ignore
+EVEX_VFMSUBADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3344
 """
 ``VFMSUBADD132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 97 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3345 # type: ignore
+EVEX_VFMSUBADD132PD_XMM_K1Z_XMM_XMMM128B64: int = 3345
 """
 ``VFMSUBADD132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 97 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3346 # type: ignore
+EVEX_VFMSUBADD132PD_YMM_K1Z_YMM_YMMM256B64: int = 3346
 """
 ``VFMSUBADD132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 97 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3347 # type: ignore
+EVEX_VFMSUBADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3347
 """
 ``VFMSUBADD132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 97 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132PS_XMM_XMM_XMMM128: Code = 3348 # type: ignore
+VEX_VFMADD132PS_XMM_XMM_XMMM128: int = 3348
 """
 ``VFMADD132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 98 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132PS_YMM_YMM_YMMM256: Code = 3349 # type: ignore
+VEX_VFMADD132PS_YMM_YMM_YMMM256: int = 3349
 """
 ``VFMADD132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 98 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132PD_XMM_XMM_XMMM128: Code = 3350 # type: ignore
+VEX_VFMADD132PD_XMM_XMM_XMMM128: int = 3350
 """
 ``VFMADD132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 98 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132PD_YMM_YMM_YMMM256: Code = 3351 # type: ignore
+VEX_VFMADD132PD_YMM_YMM_YMMM256: int = 3351
 """
 ``VFMADD132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 98 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3352 # type: ignore
+EVEX_VFMADD132PS_XMM_K1Z_XMM_XMMM128B32: int = 3352
 """
 ``VFMADD132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 98 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3353 # type: ignore
+EVEX_VFMADD132PS_YMM_K1Z_YMM_YMMM256B32: int = 3353
 """
 ``VFMADD132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 98 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3354 # type: ignore
+EVEX_VFMADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3354
 """
 ``VFMADD132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 98 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3355 # type: ignore
+EVEX_VFMADD132PD_XMM_K1Z_XMM_XMMM128B64: int = 3355
 """
 ``VFMADD132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 98 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3356 # type: ignore
+EVEX_VFMADD132PD_YMM_K1Z_YMM_YMMM256B64: int = 3356
 """
 ``VFMADD132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 98 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3357 # type: ignore
+EVEX_VFMADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3357
 """
 ``VFMADD132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 98 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132SS_XMM_XMM_XMMM32: Code = 3358 # type: ignore
+VEX_VFMADD132SS_XMM_XMM_XMMM32: int = 3358
 """
 ``VFMADD132SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 99 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD132SD_XMM_XMM_XMMM64: Code = 3359 # type: ignore
+VEX_VFMADD132SD_XMM_XMM_XMMM64: int = 3359
 """
 ``VFMADD132SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 99 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3360 # type: ignore
+EVEX_VFMADD132SS_XMM_K1Z_XMM_XMMM32_ER: int = 3360
 """
 ``VFMADD132SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 99 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD132SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3361 # type: ignore
+EVEX_VFMADD132SD_XMM_K1Z_XMM_XMMM64_ER: int = 3361
 """
 ``VFMADD132SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 99 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132PS_XMM_XMM_XMMM128: Code = 3362 # type: ignore
+VEX_VFMSUB132PS_XMM_XMM_XMMM128: int = 3362
 """
 ``VFMSUB132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 9A /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132PS_YMM_YMM_YMMM256: Code = 3363 # type: ignore
+VEX_VFMSUB132PS_YMM_YMM_YMMM256: int = 3363
 """
 ``VFMSUB132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 9A /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132PD_XMM_XMM_XMMM128: Code = 3364 # type: ignore
+VEX_VFMSUB132PD_XMM_XMM_XMMM128: int = 3364
 """
 ``VFMSUB132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 9A /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132PD_YMM_YMM_YMMM256: Code = 3365 # type: ignore
+VEX_VFMSUB132PD_YMM_YMM_YMMM256: int = 3365
 """
 ``VFMSUB132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 9A /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3366 # type: ignore
+EVEX_VFMSUB132PS_XMM_K1Z_XMM_XMMM128B32: int = 3366
 """
 ``VFMSUB132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 9A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3367 # type: ignore
+EVEX_VFMSUB132PS_YMM_K1Z_YMM_YMMM256B32: int = 3367
 """
 ``VFMSUB132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 9A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3368 # type: ignore
+EVEX_VFMSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3368
 """
 ``VFMSUB132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 9A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3369 # type: ignore
+EVEX_VFMSUB132PD_XMM_K1Z_XMM_XMMM128B64: int = 3369
 """
 ``VFMSUB132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 9A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3370 # type: ignore
+EVEX_VFMSUB132PD_YMM_K1Z_YMM_YMMM256B64: int = 3370
 """
 ``VFMSUB132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 9A /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3371 # type: ignore
+EVEX_VFMSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3371
 """
 ``VFMSUB132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 9A /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_V4FMADDPS_ZMM_K1Z_ZMMP3_M128: Code = 3372 # type: ignore
+EVEX_V4FMADDPS_ZMM_K1Z_ZMMP3_M128: int = 3372
 """
 ``V4FMADDPS zmm1 {k1}{z}, zmm2+3, m128``
 
 ``EVEX.512.F2.0F38.W0 9A /r``
 
 ``AVX512_4FMAPS``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132SS_XMM_XMM_XMMM32: Code = 3373 # type: ignore
+VEX_VFMSUB132SS_XMM_XMM_XMMM32: int = 3373
 """
 ``VFMSUB132SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 9B /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB132SD_XMM_XMM_XMMM64: Code = 3374 # type: ignore
+VEX_VFMSUB132SD_XMM_XMM_XMMM64: int = 3374
 """
 ``VFMSUB132SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 9B /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3375 # type: ignore
+EVEX_VFMSUB132SS_XMM_K1Z_XMM_XMMM32_ER: int = 3375
 """
 ``VFMSUB132SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 9B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB132SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3376 # type: ignore
+EVEX_VFMSUB132SD_XMM_K1Z_XMM_XMMM64_ER: int = 3376
 """
 ``VFMSUB132SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 9B /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_V4FMADDSS_XMM_K1Z_XMMP3_M128: Code = 3377 # type: ignore
+EVEX_V4FMADDSS_XMM_K1Z_XMMP3_M128: int = 3377
 """
 ``V4FMADDSS xmm1 {k1}{z}, xmm2+3, m128``
 
 ``EVEX.LIG.F2.0F38.W0 9B /r``
 
 ``AVX512_4FMAPS``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132PS_XMM_XMM_XMMM128: Code = 3378 # type: ignore
+VEX_VFNMADD132PS_XMM_XMM_XMMM128: int = 3378
 """
 ``VFNMADD132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 9C /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132PS_YMM_YMM_YMMM256: Code = 3379 # type: ignore
+VEX_VFNMADD132PS_YMM_YMM_YMMM256: int = 3379
 """
 ``VFNMADD132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 9C /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132PD_XMM_XMM_XMMM128: Code = 3380 # type: ignore
+VEX_VFNMADD132PD_XMM_XMM_XMMM128: int = 3380
 """
 ``VFNMADD132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 9C /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132PD_YMM_YMM_YMMM256: Code = 3381 # type: ignore
+VEX_VFNMADD132PD_YMM_YMM_YMMM256: int = 3381
 """
 ``VFNMADD132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 9C /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3382 # type: ignore
+EVEX_VFNMADD132PS_XMM_K1Z_XMM_XMMM128B32: int = 3382
 """
 ``VFNMADD132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 9C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3383 # type: ignore
+EVEX_VFNMADD132PS_YMM_K1Z_YMM_YMMM256B32: int = 3383
 """
 ``VFNMADD132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 9C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3384 # type: ignore
+EVEX_VFNMADD132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3384
 """
 ``VFNMADD132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 9C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3385 # type: ignore
+EVEX_VFNMADD132PD_XMM_K1Z_XMM_XMMM128B64: int = 3385
 """
 ``VFNMADD132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 9C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3386 # type: ignore
+EVEX_VFNMADD132PD_YMM_K1Z_YMM_YMMM256B64: int = 3386
 """
 ``VFNMADD132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 9C /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3387 # type: ignore
+EVEX_VFNMADD132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3387
 """
 ``VFNMADD132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 9C /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132SS_XMM_XMM_XMMM32: Code = 3388 # type: ignore
+VEX_VFNMADD132SS_XMM_XMM_XMMM32: int = 3388
 """
 ``VFNMADD132SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 9D /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD132SD_XMM_XMM_XMMM64: Code = 3389 # type: ignore
+VEX_VFNMADD132SD_XMM_XMM_XMMM64: int = 3389
 """
 ``VFNMADD132SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 9D /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3390 # type: ignore
+EVEX_VFNMADD132SS_XMM_K1Z_XMM_XMMM32_ER: int = 3390
 """
 ``VFNMADD132SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 9D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD132SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3391 # type: ignore
+EVEX_VFNMADD132SD_XMM_K1Z_XMM_XMMM64_ER: int = 3391
 """
 ``VFNMADD132SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 9D /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132PS_XMM_XMM_XMMM128: Code = 3392 # type: ignore
+VEX_VFNMSUB132PS_XMM_XMM_XMMM128: int = 3392
 """
 ``VFNMSUB132PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 9E /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132PS_YMM_YMM_YMMM256: Code = 3393 # type: ignore
+VEX_VFNMSUB132PS_YMM_YMM_YMMM256: int = 3393
 """
 ``VFNMSUB132PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 9E /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132PD_XMM_XMM_XMMM128: Code = 3394 # type: ignore
+VEX_VFNMSUB132PD_XMM_XMM_XMMM128: int = 3394
 """
 ``VFNMSUB132PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 9E /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132PD_YMM_YMM_YMMM256: Code = 3395 # type: ignore
+VEX_VFNMSUB132PD_YMM_YMM_YMMM256: int = 3395
 """
 ``VFNMSUB132PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 9E /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PS_XMM_K1Z_XMM_XMMM128B32: Code = 3396 # type: ignore
+EVEX_VFNMSUB132PS_XMM_K1Z_XMM_XMMM128B32: int = 3396
 """
 ``VFNMSUB132PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 9E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PS_YMM_K1Z_YMM_YMMM256B32: Code = 3397 # type: ignore
+EVEX_VFNMSUB132PS_YMM_K1Z_YMM_YMMM256B32: int = 3397
 """
 ``VFNMSUB132PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 9E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3398 # type: ignore
+EVEX_VFNMSUB132PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3398
 """
 ``VFNMSUB132PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 9E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PD_XMM_K1Z_XMM_XMMM128B64: Code = 3399 # type: ignore
+EVEX_VFNMSUB132PD_XMM_K1Z_XMM_XMMM128B64: int = 3399
 """
 ``VFNMSUB132PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 9E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PD_YMM_K1Z_YMM_YMMM256B64: Code = 3400 # type: ignore
+EVEX_VFNMSUB132PD_YMM_K1Z_YMM_YMMM256B64: int = 3400
 """
 ``VFNMSUB132PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 9E /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3401 # type: ignore
+EVEX_VFNMSUB132PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3401
 """
 ``VFNMSUB132PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 9E /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132SS_XMM_XMM_XMMM32: Code = 3402 # type: ignore
+VEX_VFNMSUB132SS_XMM_XMM_XMMM32: int = 3402
 """
 ``VFNMSUB132SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 9F /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB132SD_XMM_XMM_XMMM64: Code = 3403 # type: ignore
+VEX_VFNMSUB132SD_XMM_XMM_XMMM64: int = 3403
 """
 ``VFNMSUB132SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 9F /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3404 # type: ignore
+EVEX_VFNMSUB132SS_XMM_K1Z_XMM_XMMM32_ER: int = 3404
 """
 ``VFNMSUB132SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 9F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB132SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3405 # type: ignore
+EVEX_VFNMSUB132SD_XMM_K1Z_XMM_XMMM64_ER: int = 3405
 """
 ``VFNMSUB132SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 9F /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDD_VM32X_K1_XMM: Code = 3406 # type: ignore
+EVEX_VPSCATTERDD_VM32X_K1_XMM: int = 3406
 """
 ``VPSCATTERDD vm32x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W0 A0 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDD_VM32Y_K1_YMM: Code = 3407 # type: ignore
+EVEX_VPSCATTERDD_VM32Y_K1_YMM: int = 3407
 """
 ``VPSCATTERDD vm32y {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W0 A0 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDD_VM32Z_K1_ZMM: Code = 3408 # type: ignore
+EVEX_VPSCATTERDD_VM32Z_K1_ZMM: int = 3408
 """
 ``VPSCATTERDD vm32z {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W0 A0 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDQ_VM32X_K1_XMM: Code = 3409 # type: ignore
+EVEX_VPSCATTERDQ_VM32X_K1_XMM: int = 3409
 """
 ``VPSCATTERDQ vm32x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W1 A0 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDQ_VM32X_K1_YMM: Code = 3410 # type: ignore
+EVEX_VPSCATTERDQ_VM32X_K1_YMM: int = 3410
 """
 ``VPSCATTERDQ vm32x {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W1 A0 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERDQ_VM32Y_K1_ZMM: Code = 3411 # type: ignore
+EVEX_VPSCATTERDQ_VM32Y_K1_ZMM: int = 3411
 """
 ``VPSCATTERDQ vm32y {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W1 A0 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQD_VM64X_K1_XMM: Code = 3412 # type: ignore
+EVEX_VPSCATTERQD_VM64X_K1_XMM: int = 3412
 """
 ``VPSCATTERQD vm64x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W0 A1 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQD_VM64Y_K1_XMM: Code = 3413 # type: ignore
+EVEX_VPSCATTERQD_VM64Y_K1_XMM: int = 3413
 """
 ``VPSCATTERQD vm64y {k1}, xmm1``
 
 ``EVEX.256.66.0F38.W0 A1 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQD_VM64Z_K1_YMM: Code = 3414 # type: ignore
+EVEX_VPSCATTERQD_VM64Z_K1_YMM: int = 3414
 """
 ``VPSCATTERQD vm64z {k1}, ymm1``
 
 ``EVEX.512.66.0F38.W0 A1 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQQ_VM64X_K1_XMM: Code = 3415 # type: ignore
+EVEX_VPSCATTERQQ_VM64X_K1_XMM: int = 3415
 """
 ``VPSCATTERQQ vm64x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W1 A1 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQQ_VM64Y_K1_YMM: Code = 3416 # type: ignore
+EVEX_VPSCATTERQQ_VM64Y_K1_YMM: int = 3416
 """
 ``VPSCATTERQQ vm64y {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W1 A1 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPSCATTERQQ_VM64Z_K1_ZMM: Code = 3417 # type: ignore
+EVEX_VPSCATTERQQ_VM64Z_K1_ZMM: int = 3417
 """
 ``VPSCATTERQQ vm64z {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W1 A1 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPS_VM32X_K1_XMM: Code = 3418 # type: ignore
+EVEX_VSCATTERDPS_VM32X_K1_XMM: int = 3418
 """
 ``VSCATTERDPS vm32x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W0 A2 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPS_VM32Y_K1_YMM: Code = 3419 # type: ignore
+EVEX_VSCATTERDPS_VM32Y_K1_YMM: int = 3419
 """
 ``VSCATTERDPS vm32y {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W0 A2 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPS_VM32Z_K1_ZMM: Code = 3420 # type: ignore
+EVEX_VSCATTERDPS_VM32Z_K1_ZMM: int = 3420
 """
 ``VSCATTERDPS vm32z {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W0 A2 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPD_VM32X_K1_XMM: Code = 3421 # type: ignore
+EVEX_VSCATTERDPD_VM32X_K1_XMM: int = 3421
 """
 ``VSCATTERDPD vm32x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W1 A2 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPD_VM32X_K1_YMM: Code = 3422 # type: ignore
+EVEX_VSCATTERDPD_VM32X_K1_YMM: int = 3422
 """
 ``VSCATTERDPD vm32x {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W1 A2 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERDPD_VM32Y_K1_ZMM: Code = 3423 # type: ignore
+EVEX_VSCATTERDPD_VM32Y_K1_ZMM: int = 3423
 """
 ``VSCATTERDPD vm32y {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W1 A2 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPS_VM64X_K1_XMM: Code = 3424 # type: ignore
+EVEX_VSCATTERQPS_VM64X_K1_XMM: int = 3424
 """
 ``VSCATTERQPS vm64x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W0 A3 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPS_VM64Y_K1_XMM: Code = 3425 # type: ignore
+EVEX_VSCATTERQPS_VM64Y_K1_XMM: int = 3425
 """
 ``VSCATTERQPS vm64y {k1}, xmm1``
 
 ``EVEX.256.66.0F38.W0 A3 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPS_VM64Z_K1_YMM: Code = 3426 # type: ignore
+EVEX_VSCATTERQPS_VM64Z_K1_YMM: int = 3426
 """
 ``VSCATTERQPS vm64z {k1}, ymm1``
 
 ``EVEX.512.66.0F38.W0 A3 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPD_VM64X_K1_XMM: Code = 3427 # type: ignore
+EVEX_VSCATTERQPD_VM64X_K1_XMM: int = 3427
 """
 ``VSCATTERQPD vm64x {k1}, xmm1``
 
 ``EVEX.128.66.0F38.W1 A3 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPD_VM64Y_K1_YMM: Code = 3428 # type: ignore
+EVEX_VSCATTERQPD_VM64Y_K1_YMM: int = 3428
 """
 ``VSCATTERQPD vm64y {k1}, ymm1``
 
 ``EVEX.256.66.0F38.W1 A3 /vsib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERQPD_VM64Z_K1_ZMM: Code = 3429 # type: ignore
+EVEX_VSCATTERQPD_VM64Z_K1_ZMM: int = 3429
 """
 ``VSCATTERQPD vm64z {k1}, zmm1``
 
 ``EVEX.512.66.0F38.W1 A3 /vsib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB213PS_XMM_XMM_XMMM128: Code = 3430 # type: ignore
+VEX_VFMADDSUB213PS_XMM_XMM_XMMM128: int = 3430
 """
 ``VFMADDSUB213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 A6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB213PS_YMM_YMM_YMMM256: Code = 3431 # type: ignore
+VEX_VFMADDSUB213PS_YMM_YMM_YMMM256: int = 3431
 """
 ``VFMADDSUB213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 A6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB213PD_XMM_XMM_XMMM128: Code = 3432 # type: ignore
+VEX_VFMADDSUB213PD_XMM_XMM_XMMM128: int = 3432
 """
 ``VFMADDSUB213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 A6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB213PD_YMM_YMM_YMMM256: Code = 3433 # type: ignore
+VEX_VFMADDSUB213PD_YMM_YMM_YMMM256: int = 3433
 """
 ``VFMADDSUB213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 A6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3434 # type: ignore
+EVEX_VFMADDSUB213PS_XMM_K1Z_XMM_XMMM128B32: int = 3434
 """
 ``VFMADDSUB213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 A6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3435 # type: ignore
+EVEX_VFMADDSUB213PS_YMM_K1Z_YMM_YMMM256B32: int = 3435
 """
 ``VFMADDSUB213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 A6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3436 # type: ignore
+EVEX_VFMADDSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3436
 """
 ``VFMADDSUB213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 A6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3437 # type: ignore
+EVEX_VFMADDSUB213PD_XMM_K1Z_XMM_XMMM128B64: int = 3437
 """
 ``VFMADDSUB213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 A6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3438 # type: ignore
+EVEX_VFMADDSUB213PD_YMM_K1Z_YMM_YMMM256B64: int = 3438
 """
 ``VFMADDSUB213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 A6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3439 # type: ignore
+EVEX_VFMADDSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3439
 """
 ``VFMADDSUB213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 A6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD213PS_XMM_XMM_XMMM128: Code = 3440 # type: ignore
+VEX_VFMSUBADD213PS_XMM_XMM_XMMM128: int = 3440
 """
 ``VFMSUBADD213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 A7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD213PS_YMM_YMM_YMMM256: Code = 3441 # type: ignore
+VEX_VFMSUBADD213PS_YMM_YMM_YMMM256: int = 3441
 """
 ``VFMSUBADD213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 A7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD213PD_XMM_XMM_XMMM128: Code = 3442 # type: ignore
+VEX_VFMSUBADD213PD_XMM_XMM_XMMM128: int = 3442
 """
 ``VFMSUBADD213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 A7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD213PD_YMM_YMM_YMMM256: Code = 3443 # type: ignore
+VEX_VFMSUBADD213PD_YMM_YMM_YMMM256: int = 3443
 """
 ``VFMSUBADD213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 A7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3444 # type: ignore
+EVEX_VFMSUBADD213PS_XMM_K1Z_XMM_XMMM128B32: int = 3444
 """
 ``VFMSUBADD213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 A7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3445 # type: ignore
+EVEX_VFMSUBADD213PS_YMM_K1Z_YMM_YMMM256B32: int = 3445
 """
 ``VFMSUBADD213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 A7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3446 # type: ignore
+EVEX_VFMSUBADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3446
 """
 ``VFMSUBADD213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 A7 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3447 # type: ignore
+EVEX_VFMSUBADD213PD_XMM_K1Z_XMM_XMMM128B64: int = 3447
 """
 ``VFMSUBADD213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 A7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3448 # type: ignore
+EVEX_VFMSUBADD213PD_YMM_K1Z_YMM_YMMM256B64: int = 3448
 """
 ``VFMSUBADD213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 A7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3449 # type: ignore
+EVEX_VFMSUBADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3449
 """
 ``VFMSUBADD213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 A7 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213PS_XMM_XMM_XMMM128: Code = 3450 # type: ignore
+VEX_VFMADD213PS_XMM_XMM_XMMM128: int = 3450
 """
 ``VFMADD213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 A8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213PS_YMM_YMM_YMMM256: Code = 3451 # type: ignore
+VEX_VFMADD213PS_YMM_YMM_YMMM256: int = 3451
 """
 ``VFMADD213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 A8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213PD_XMM_XMM_XMMM128: Code = 3452 # type: ignore
+VEX_VFMADD213PD_XMM_XMM_XMMM128: int = 3452
 """
 ``VFMADD213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 A8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213PD_YMM_YMM_YMMM256: Code = 3453 # type: ignore
+VEX_VFMADD213PD_YMM_YMM_YMMM256: int = 3453
 """
 ``VFMADD213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 A8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3454 # type: ignore
+EVEX_VFMADD213PS_XMM_K1Z_XMM_XMMM128B32: int = 3454
 """
 ``VFMADD213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 A8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3455 # type: ignore
+EVEX_VFMADD213PS_YMM_K1Z_YMM_YMMM256B32: int = 3455
 """
 ``VFMADD213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 A8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3456 # type: ignore
+EVEX_VFMADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3456
 """
 ``VFMADD213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 A8 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3457 # type: ignore
+EVEX_VFMADD213PD_XMM_K1Z_XMM_XMMM128B64: int = 3457
 """
 ``VFMADD213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 A8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3458 # type: ignore
+EVEX_VFMADD213PD_YMM_K1Z_YMM_YMMM256B64: int = 3458
 """
 ``VFMADD213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 A8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3459 # type: ignore
+EVEX_VFMADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3459
 """
 ``VFMADD213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 A8 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213SS_XMM_XMM_XMMM32: Code = 3460 # type: ignore
+VEX_VFMADD213SS_XMM_XMM_XMMM32: int = 3460
 """
 ``VFMADD213SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 A9 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD213SD_XMM_XMM_XMMM64: Code = 3461 # type: ignore
+VEX_VFMADD213SD_XMM_XMM_XMMM64: int = 3461
 """
 ``VFMADD213SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 A9 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3462 # type: ignore
+EVEX_VFMADD213SS_XMM_K1Z_XMM_XMMM32_ER: int = 3462
 """
 ``VFMADD213SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 A9 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD213SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3463 # type: ignore
+EVEX_VFMADD213SD_XMM_K1Z_XMM_XMMM64_ER: int = 3463
 """
 ``VFMADD213SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 A9 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213PS_XMM_XMM_XMMM128: Code = 3464 # type: ignore
+VEX_VFMSUB213PS_XMM_XMM_XMMM128: int = 3464
 """
 ``VFMSUB213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 AA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213PS_YMM_YMM_YMMM256: Code = 3465 # type: ignore
+VEX_VFMSUB213PS_YMM_YMM_YMMM256: int = 3465
 """
 ``VFMSUB213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 AA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213PD_XMM_XMM_XMMM128: Code = 3466 # type: ignore
+VEX_VFMSUB213PD_XMM_XMM_XMMM128: int = 3466
 """
 ``VFMSUB213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 AA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213PD_YMM_YMM_YMMM256: Code = 3467 # type: ignore
+VEX_VFMSUB213PD_YMM_YMM_YMMM256: int = 3467
 """
 ``VFMSUB213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 AA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3468 # type: ignore
+EVEX_VFMSUB213PS_XMM_K1Z_XMM_XMMM128B32: int = 3468
 """
 ``VFMSUB213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 AA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3469 # type: ignore
+EVEX_VFMSUB213PS_YMM_K1Z_YMM_YMMM256B32: int = 3469
 """
 ``VFMSUB213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 AA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3470 # type: ignore
+EVEX_VFMSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3470
 """
 ``VFMSUB213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 AA /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3471 # type: ignore
+EVEX_VFMSUB213PD_XMM_K1Z_XMM_XMMM128B64: int = 3471
 """
 ``VFMSUB213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 AA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3472 # type: ignore
+EVEX_VFMSUB213PD_YMM_K1Z_YMM_YMMM256B64: int = 3472
 """
 ``VFMSUB213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 AA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3473 # type: ignore
+EVEX_VFMSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3473
 """
 ``VFMSUB213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 AA /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_V4FNMADDPS_ZMM_K1Z_ZMMP3_M128: Code = 3474 # type: ignore
+EVEX_V4FNMADDPS_ZMM_K1Z_ZMMP3_M128: int = 3474
 """
 ``V4FNMADDPS zmm1 {k1}{z}, zmm2+3, m128``
 
 ``EVEX.512.F2.0F38.W0 AA /r``
 
 ``AVX512_4FMAPS``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213SS_XMM_XMM_XMMM32: Code = 3475 # type: ignore
+VEX_VFMSUB213SS_XMM_XMM_XMMM32: int = 3475
 """
 ``VFMSUB213SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 AB /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB213SD_XMM_XMM_XMMM64: Code = 3476 # type: ignore
+VEX_VFMSUB213SD_XMM_XMM_XMMM64: int = 3476
 """
 ``VFMSUB213SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 AB /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3477 # type: ignore
+EVEX_VFMSUB213SS_XMM_K1Z_XMM_XMMM32_ER: int = 3477
 """
 ``VFMSUB213SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 AB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB213SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3478 # type: ignore
+EVEX_VFMSUB213SD_XMM_K1Z_XMM_XMMM64_ER: int = 3478
 """
 ``VFMSUB213SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 AB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_V4FNMADDSS_XMM_K1Z_XMMP3_M128: Code = 3479 # type: ignore
+EVEX_V4FNMADDSS_XMM_K1Z_XMMP3_M128: int = 3479
 """
 ``V4FNMADDSS xmm1 {k1}{z}, xmm2+3, m128``
 
 ``EVEX.LIG.F2.0F38.W0 AB /r``
 
 ``AVX512_4FMAPS``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213PS_XMM_XMM_XMMM128: Code = 3480 # type: ignore
+VEX_VFNMADD213PS_XMM_XMM_XMMM128: int = 3480
 """
 ``VFNMADD213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 AC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213PS_YMM_YMM_YMMM256: Code = 3481 # type: ignore
+VEX_VFNMADD213PS_YMM_YMM_YMMM256: int = 3481
 """
 ``VFNMADD213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 AC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213PD_XMM_XMM_XMMM128: Code = 3482 # type: ignore
+VEX_VFNMADD213PD_XMM_XMM_XMMM128: int = 3482
 """
 ``VFNMADD213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 AC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213PD_YMM_YMM_YMMM256: Code = 3483 # type: ignore
+VEX_VFNMADD213PD_YMM_YMM_YMMM256: int = 3483
 """
 ``VFNMADD213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 AC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3484 # type: ignore
+EVEX_VFNMADD213PS_XMM_K1Z_XMM_XMMM128B32: int = 3484
 """
 ``VFNMADD213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 AC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3485 # type: ignore
+EVEX_VFNMADD213PS_YMM_K1Z_YMM_YMMM256B32: int = 3485
 """
 ``VFNMADD213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 AC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3486 # type: ignore
+EVEX_VFNMADD213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3486
 """
 ``VFNMADD213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 AC /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3487 # type: ignore
+EVEX_VFNMADD213PD_XMM_K1Z_XMM_XMMM128B64: int = 3487
 """
 ``VFNMADD213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 AC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3488 # type: ignore
+EVEX_VFNMADD213PD_YMM_K1Z_YMM_YMMM256B64: int = 3488
 """
 ``VFNMADD213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 AC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3489 # type: ignore
+EVEX_VFNMADD213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3489
 """
 ``VFNMADD213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 AC /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213SS_XMM_XMM_XMMM32: Code = 3490 # type: ignore
+VEX_VFNMADD213SS_XMM_XMM_XMMM32: int = 3490
 """
 ``VFNMADD213SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 AD /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD213SD_XMM_XMM_XMMM64: Code = 3491 # type: ignore
+VEX_VFNMADD213SD_XMM_XMM_XMMM64: int = 3491
 """
 ``VFNMADD213SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 AD /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3492 # type: ignore
+EVEX_VFNMADD213SS_XMM_K1Z_XMM_XMMM32_ER: int = 3492
 """
 ``VFNMADD213SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 AD /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD213SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3493 # type: ignore
+EVEX_VFNMADD213SD_XMM_K1Z_XMM_XMMM64_ER: int = 3493
 """
 ``VFNMADD213SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 AD /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213PS_XMM_XMM_XMMM128: Code = 3494 # type: ignore
+VEX_VFNMSUB213PS_XMM_XMM_XMMM128: int = 3494
 """
 ``VFNMSUB213PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 AE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213PS_YMM_YMM_YMMM256: Code = 3495 # type: ignore
+VEX_VFNMSUB213PS_YMM_YMM_YMMM256: int = 3495
 """
 ``VFNMSUB213PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 AE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213PD_XMM_XMM_XMMM128: Code = 3496 # type: ignore
+VEX_VFNMSUB213PD_XMM_XMM_XMMM128: int = 3496
 """
 ``VFNMSUB213PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 AE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213PD_YMM_YMM_YMMM256: Code = 3497 # type: ignore
+VEX_VFNMSUB213PD_YMM_YMM_YMMM256: int = 3497
 """
 ``VFNMSUB213PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 AE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PS_XMM_K1Z_XMM_XMMM128B32: Code = 3498 # type: ignore
+EVEX_VFNMSUB213PS_XMM_K1Z_XMM_XMMM128B32: int = 3498
 """
 ``VFNMSUB213PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 AE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PS_YMM_K1Z_YMM_YMMM256B32: Code = 3499 # type: ignore
+EVEX_VFNMSUB213PS_YMM_K1Z_YMM_YMMM256B32: int = 3499
 """
 ``VFNMSUB213PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 AE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3500 # type: ignore
+EVEX_VFNMSUB213PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3500
 """
 ``VFNMSUB213PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 AE /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PD_XMM_K1Z_XMM_XMMM128B64: Code = 3501 # type: ignore
+EVEX_VFNMSUB213PD_XMM_K1Z_XMM_XMMM128B64: int = 3501
 """
 ``VFNMSUB213PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 AE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PD_YMM_K1Z_YMM_YMMM256B64: Code = 3502 # type: ignore
+EVEX_VFNMSUB213PD_YMM_K1Z_YMM_YMMM256B64: int = 3502
 """
 ``VFNMSUB213PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 AE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3503 # type: ignore
+EVEX_VFNMSUB213PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3503
 """
 ``VFNMSUB213PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 AE /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213SS_XMM_XMM_XMMM32: Code = 3504 # type: ignore
+VEX_VFNMSUB213SS_XMM_XMM_XMMM32: int = 3504
 """
 ``VFNMSUB213SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 AF /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB213SD_XMM_XMM_XMMM64: Code = 3505 # type: ignore
+VEX_VFNMSUB213SD_XMM_XMM_XMMM64: int = 3505
 """
 ``VFNMSUB213SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 AF /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3506 # type: ignore
+EVEX_VFNMSUB213SS_XMM_K1Z_XMM_XMMM32_ER: int = 3506
 """
 ``VFNMSUB213SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 AF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB213SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3507 # type: ignore
+EVEX_VFNMSUB213SD_XMM_K1Z_XMM_XMMM64_ER: int = 3507
 """
 ``VFNMSUB213SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 AF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52LUQ_XMM_K1Z_XMM_XMMM128B64: Code = 3508 # type: ignore
+EVEX_VPMADD52LUQ_XMM_K1Z_XMM_XMMM128B64: int = 3508
 """
 ``VPMADD52LUQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 B4 /r``
 
 ``AVX512VL and AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52LUQ_YMM_K1Z_YMM_YMMM256B64: Code = 3509 # type: ignore
+EVEX_VPMADD52LUQ_YMM_K1Z_YMM_YMMM256B64: int = 3509
 """
 ``VPMADD52LUQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 B4 /r``
 
 ``AVX512VL and AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52LUQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3510 # type: ignore
+EVEX_VPMADD52LUQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3510
 """
 ``VPMADD52LUQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 B4 /r``
 
 ``AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52HUQ_XMM_K1Z_XMM_XMMM128B64: Code = 3511 # type: ignore
+EVEX_VPMADD52HUQ_XMM_K1Z_XMM_XMMM128B64: int = 3511
 """
 ``VPMADD52HUQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 B5 /r``
 
 ``AVX512VL and AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52HUQ_YMM_K1Z_YMM_YMMM256B64: Code = 3512 # type: ignore
+EVEX_VPMADD52HUQ_YMM_K1Z_YMM_YMMM256B64: int = 3512
 """
 ``VPMADD52HUQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 B5 /r``
 
 ``AVX512VL and AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-EVEX_VPMADD52HUQ_ZMM_K1Z_ZMM_ZMMM512B64: Code = 3513 # type: ignore
+EVEX_VPMADD52HUQ_ZMM_K1Z_ZMM_ZMMM512B64: int = 3513
 """
 ``VPMADD52HUQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 B5 /r``
 
 ``AVX512_IFMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB231PS_XMM_XMM_XMMM128: Code = 3514 # type: ignore
+VEX_VFMADDSUB231PS_XMM_XMM_XMMM128: int = 3514
 """
 ``VFMADDSUB231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 B6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB231PS_YMM_YMM_YMMM256: Code = 3515 # type: ignore
+VEX_VFMADDSUB231PS_YMM_YMM_YMMM256: int = 3515
 """
 ``VFMADDSUB231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 B6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB231PD_XMM_XMM_XMMM128: Code = 3516 # type: ignore
+VEX_VFMADDSUB231PD_XMM_XMM_XMMM128: int = 3516
 """
 ``VFMADDSUB231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 B6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUB231PD_YMM_YMM_YMMM256: Code = 3517 # type: ignore
+VEX_VFMADDSUB231PD_YMM_YMM_YMMM256: int = 3517
 """
 ``VFMADDSUB231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 B6 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3518 # type: ignore
+EVEX_VFMADDSUB231PS_XMM_K1Z_XMM_XMMM128B32: int = 3518
 """
 ``VFMADDSUB231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 B6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3519 # type: ignore
+EVEX_VFMADDSUB231PS_YMM_K1Z_YMM_YMMM256B32: int = 3519
 """
 ``VFMADDSUB231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 B6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3520 # type: ignore
+EVEX_VFMADDSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3520
 """
 ``VFMADDSUB231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 B6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3521 # type: ignore
+EVEX_VFMADDSUB231PD_XMM_K1Z_XMM_XMMM128B64: int = 3521
 """
 ``VFMADDSUB231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 B6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3522 # type: ignore
+EVEX_VFMADDSUB231PD_YMM_K1Z_YMM_YMMM256B64: int = 3522
 """
 ``VFMADDSUB231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 B6 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADDSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3523 # type: ignore
+EVEX_VFMADDSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3523
 """
 ``VFMADDSUB231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 B6 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD231PS_XMM_XMM_XMMM128: Code = 3524 # type: ignore
+VEX_VFMSUBADD231PS_XMM_XMM_XMMM128: int = 3524
 """
 ``VFMSUBADD231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 B7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD231PS_YMM_YMM_YMMM256: Code = 3525 # type: ignore
+VEX_VFMSUBADD231PS_YMM_YMM_YMMM256: int = 3525
 """
 ``VFMSUBADD231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 B7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD231PD_XMM_XMM_XMMM128: Code = 3526 # type: ignore
+VEX_VFMSUBADD231PD_XMM_XMM_XMMM128: int = 3526
 """
 ``VFMSUBADD231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 B7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADD231PD_YMM_YMM_YMMM256: Code = 3527 # type: ignore
+VEX_VFMSUBADD231PD_YMM_YMM_YMMM256: int = 3527
 """
 ``VFMSUBADD231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 B7 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3528 # type: ignore
+EVEX_VFMSUBADD231PS_XMM_K1Z_XMM_XMMM128B32: int = 3528
 """
 ``VFMSUBADD231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 B7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3529 # type: ignore
+EVEX_VFMSUBADD231PS_YMM_K1Z_YMM_YMMM256B32: int = 3529
 """
 ``VFMSUBADD231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 B7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3530 # type: ignore
+EVEX_VFMSUBADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3530
 """
 ``VFMSUBADD231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 B7 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3531 # type: ignore
+EVEX_VFMSUBADD231PD_XMM_K1Z_XMM_XMMM128B64: int = 3531
 """
 ``VFMSUBADD231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 B7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3532 # type: ignore
+EVEX_VFMSUBADD231PD_YMM_K1Z_YMM_YMMM256B64: int = 3532
 """
 ``VFMSUBADD231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 B7 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUBADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3533 # type: ignore
+EVEX_VFMSUBADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3533
 """
 ``VFMSUBADD231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 B7 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231PS_XMM_XMM_XMMM128: Code = 3534 # type: ignore
+VEX_VFMADD231PS_XMM_XMM_XMMM128: int = 3534
 """
 ``VFMADD231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 B8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231PS_YMM_YMM_YMMM256: Code = 3535 # type: ignore
+VEX_VFMADD231PS_YMM_YMM_YMMM256: int = 3535
 """
 ``VFMADD231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 B8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231PD_XMM_XMM_XMMM128: Code = 3536 # type: ignore
+VEX_VFMADD231PD_XMM_XMM_XMMM128: int = 3536
 """
 ``VFMADD231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 B8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231PD_YMM_YMM_YMMM256: Code = 3537 # type: ignore
+VEX_VFMADD231PD_YMM_YMM_YMMM256: int = 3537
 """
 ``VFMADD231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 B8 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3538 # type: ignore
+EVEX_VFMADD231PS_XMM_K1Z_XMM_XMMM128B32: int = 3538
 """
 ``VFMADD231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 B8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3539 # type: ignore
+EVEX_VFMADD231PS_YMM_K1Z_YMM_YMMM256B32: int = 3539
 """
 ``VFMADD231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 B8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3540 # type: ignore
+EVEX_VFMADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3540
 """
 ``VFMADD231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 B8 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3541 # type: ignore
+EVEX_VFMADD231PD_XMM_K1Z_XMM_XMMM128B64: int = 3541
 """
 ``VFMADD231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 B8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3542 # type: ignore
+EVEX_VFMADD231PD_YMM_K1Z_YMM_YMMM256B64: int = 3542
 """
 ``VFMADD231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 B8 /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3543 # type: ignore
+EVEX_VFMADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3543
 """
 ``VFMADD231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 B8 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231SS_XMM_XMM_XMMM32: Code = 3544 # type: ignore
+VEX_VFMADD231SS_XMM_XMM_XMMM32: int = 3544
 """
 ``VFMADD231SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 B9 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMADD231SD_XMM_XMM_XMMM64: Code = 3545 # type: ignore
+VEX_VFMADD231SD_XMM_XMM_XMMM64: int = 3545
 """
 ``VFMADD231SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 B9 /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3546 # type: ignore
+EVEX_VFMADD231SS_XMM_K1Z_XMM_XMMM32_ER: int = 3546
 """
 ``VFMADD231SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 B9 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMADD231SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3547 # type: ignore
+EVEX_VFMADD231SD_XMM_K1Z_XMM_XMMM64_ER: int = 3547
 """
 ``VFMADD231SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 B9 /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231PS_XMM_XMM_XMMM128: Code = 3548 # type: ignore
+VEX_VFMSUB231PS_XMM_XMM_XMMM128: int = 3548
 """
 ``VFMSUB231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 BA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231PS_YMM_YMM_YMMM256: Code = 3549 # type: ignore
+VEX_VFMSUB231PS_YMM_YMM_YMMM256: int = 3549
 """
 ``VFMSUB231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 BA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231PD_XMM_XMM_XMMM128: Code = 3550 # type: ignore
+VEX_VFMSUB231PD_XMM_XMM_XMMM128: int = 3550
 """
 ``VFMSUB231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 BA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231PD_YMM_YMM_YMMM256: Code = 3551 # type: ignore
+VEX_VFMSUB231PD_YMM_YMM_YMMM256: int = 3551
 """
 ``VFMSUB231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 BA /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3552 # type: ignore
+EVEX_VFMSUB231PS_XMM_K1Z_XMM_XMMM128B32: int = 3552
 """
 ``VFMSUB231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 BA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3553 # type: ignore
+EVEX_VFMSUB231PS_YMM_K1Z_YMM_YMMM256B32: int = 3553
 """
 ``VFMSUB231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 BA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3554 # type: ignore
+EVEX_VFMSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3554
 """
 ``VFMSUB231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 BA /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3555 # type: ignore
+EVEX_VFMSUB231PD_XMM_K1Z_XMM_XMMM128B64: int = 3555
 """
 ``VFMSUB231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 BA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3556 # type: ignore
+EVEX_VFMSUB231PD_YMM_K1Z_YMM_YMMM256B64: int = 3556
 """
 ``VFMSUB231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 BA /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3557 # type: ignore
+EVEX_VFMSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3557
 """
 ``VFMSUB231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 BA /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231SS_XMM_XMM_XMMM32: Code = 3558 # type: ignore
+VEX_VFMSUB231SS_XMM_XMM_XMMM32: int = 3558
 """
 ``VFMSUB231SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 BB /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUB231SD_XMM_XMM_XMMM64: Code = 3559 # type: ignore
+VEX_VFMSUB231SD_XMM_XMM_XMMM64: int = 3559
 """
 ``VFMSUB231SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 BB /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3560 # type: ignore
+EVEX_VFMSUB231SS_XMM_K1Z_XMM_XMMM32_ER: int = 3560
 """
 ``VFMSUB231SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 BB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFMSUB231SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3561 # type: ignore
+EVEX_VFMSUB231SD_XMM_K1Z_XMM_XMMM64_ER: int = 3561
 """
 ``VFMSUB231SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 BB /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231PS_XMM_XMM_XMMM128: Code = 3562 # type: ignore
+VEX_VFNMADD231PS_XMM_XMM_XMMM128: int = 3562
 """
 ``VFNMADD231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 BC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231PS_YMM_YMM_YMMM256: Code = 3563 # type: ignore
+VEX_VFNMADD231PS_YMM_YMM_YMMM256: int = 3563
 """
 ``VFNMADD231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 BC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231PD_XMM_XMM_XMMM128: Code = 3564 # type: ignore
+VEX_VFNMADD231PD_XMM_XMM_XMMM128: int = 3564
 """
 ``VFNMADD231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 BC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231PD_YMM_YMM_YMMM256: Code = 3565 # type: ignore
+VEX_VFNMADD231PD_YMM_YMM_YMMM256: int = 3565
 """
 ``VFNMADD231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 BC /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3566 # type: ignore
+EVEX_VFNMADD231PS_XMM_K1Z_XMM_XMMM128B32: int = 3566
 """
 ``VFNMADD231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 BC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3567 # type: ignore
+EVEX_VFNMADD231PS_YMM_K1Z_YMM_YMMM256B32: int = 3567
 """
 ``VFNMADD231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 BC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3568 # type: ignore
+EVEX_VFNMADD231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3568
 """
 ``VFNMADD231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 BC /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3569 # type: ignore
+EVEX_VFNMADD231PD_XMM_K1Z_XMM_XMMM128B64: int = 3569
 """
 ``VFNMADD231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 BC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3570 # type: ignore
+EVEX_VFNMADD231PD_YMM_K1Z_YMM_YMMM256B64: int = 3570
 """
 ``VFNMADD231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 BC /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3571 # type: ignore
+EVEX_VFNMADD231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3571
 """
 ``VFNMADD231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 BC /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231SS_XMM_XMM_XMMM32: Code = 3572 # type: ignore
+VEX_VFNMADD231SS_XMM_XMM_XMMM32: int = 3572
 """
 ``VFNMADD231SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 BD /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADD231SD_XMM_XMM_XMMM64: Code = 3573 # type: ignore
+VEX_VFNMADD231SD_XMM_XMM_XMMM64: int = 3573
 """
 ``VFNMADD231SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 BD /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3574 # type: ignore
+EVEX_VFNMADD231SS_XMM_K1Z_XMM_XMMM32_ER: int = 3574
 """
 ``VFNMADD231SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 BD /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMADD231SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3575 # type: ignore
+EVEX_VFNMADD231SD_XMM_K1Z_XMM_XMMM64_ER: int = 3575
 """
 ``VFNMADD231SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 BD /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231PS_XMM_XMM_XMMM128: Code = 3576 # type: ignore
+VEX_VFNMSUB231PS_XMM_XMM_XMMM128: int = 3576
 """
 ``VFNMSUB231PS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 BE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231PS_YMM_YMM_YMMM256: Code = 3577 # type: ignore
+VEX_VFNMSUB231PS_YMM_YMM_YMMM256: int = 3577
 """
 ``VFNMSUB231PS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 BE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231PD_XMM_XMM_XMMM128: Code = 3578 # type: ignore
+VEX_VFNMSUB231PD_XMM_XMM_XMMM128: int = 3578
 """
 ``VFNMSUB231PD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W1 BE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231PD_YMM_YMM_YMMM256: Code = 3579 # type: ignore
+VEX_VFNMSUB231PD_YMM_YMM_YMMM256: int = 3579
 """
 ``VFNMSUB231PD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W1 BE /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PS_XMM_K1Z_XMM_XMMM128B32: Code = 3580 # type: ignore
+EVEX_VFNMSUB231PS_XMM_K1Z_XMM_XMMM128B32: int = 3580
 """
 ``VFNMSUB231PS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 BE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PS_YMM_K1Z_YMM_YMMM256B32: Code = 3581 # type: ignore
+EVEX_VFNMSUB231PS_YMM_K1Z_YMM_YMMM256B32: int = 3581
 """
 ``VFNMSUB231PS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 BE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 3582 # type: ignore
+EVEX_VFNMSUB231PS_ZMM_K1Z_ZMM_ZMMM512B32_ER: int = 3582
 """
 ``VFNMSUB231PS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
 
 ``EVEX.512.66.0F38.W0 BE /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PD_XMM_K1Z_XMM_XMMM128B64: Code = 3583 # type: ignore
+EVEX_VFNMSUB231PD_XMM_K1Z_XMM_XMMM128B64: int = 3583
 """
 ``VFNMSUB231PD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 BE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PD_YMM_K1Z_YMM_YMMM256B64: Code = 3584 # type: ignore
+EVEX_VFNMSUB231PD_YMM_K1Z_YMM_YMMM256B64: int = 3584
 """
 ``VFNMSUB231PD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 BE /r``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: Code = 3585 # type: ignore
+EVEX_VFNMSUB231PD_ZMM_K1Z_ZMM_ZMMM512B64_ER: int = 3585
 """
 ``VFNMSUB231PD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{er}``
 
 ``EVEX.512.66.0F38.W1 BE /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231SS_XMM_XMM_XMMM32: Code = 3586 # type: ignore
+VEX_VFNMSUB231SS_XMM_XMM_XMMM32: int = 3586
 """
 ``VFNMSUB231SS xmm1, xmm2, xmm3/m32``
 
 ``VEX.LIG.66.0F38.W0 BF /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUB231SD_XMM_XMM_XMMM64: Code = 3587 # type: ignore
+VEX_VFNMSUB231SD_XMM_XMM_XMMM64: int = 3587
 """
 ``VFNMSUB231SD xmm1, xmm2, xmm3/m64``
 
 ``VEX.LIG.66.0F38.W1 BF /r``
 
 ``FMA``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231SS_XMM_K1Z_XMM_XMMM32_ER: Code = 3588 # type: ignore
+EVEX_VFNMSUB231SS_XMM_K1Z_XMM_XMMM32_ER: int = 3588
 """
 ``VFNMSUB231SS xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
 
 ``EVEX.LIG.66.0F38.W0 BF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFNMSUB231SD_XMM_K1Z_XMM_XMMM64_ER: Code = 3589 # type: ignore
+EVEX_VFNMSUB231SD_XMM_K1Z_XMM_XMMM64_ER: int = 3589
 """
 ``VFNMSUB231SD xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
 
 ``EVEX.LIG.66.0F38.W1 BF /r``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTD_XMM_K1Z_XMMM128B32: Code = 3590 # type: ignore
+EVEX_VPCONFLICTD_XMM_K1Z_XMMM128B32: int = 3590
 """
 ``VPCONFLICTD xmm1 {k1}{z}, xmm2/m128/m32bcst``
 
 ``EVEX.128.66.0F38.W0 C4 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTD_YMM_K1Z_YMMM256B32: Code = 3591 # type: ignore
+EVEX_VPCONFLICTD_YMM_K1Z_YMMM256B32: int = 3591
 """
 ``VPCONFLICTD ymm1 {k1}{z}, ymm2/m256/m32bcst``
 
 ``EVEX.256.66.0F38.W0 C4 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTD_ZMM_K1Z_ZMMM512B32: Code = 3592 # type: ignore
+EVEX_VPCONFLICTD_ZMM_K1Z_ZMMM512B32: int = 3592
 """
 ``VPCONFLICTD zmm1 {k1}{z}, zmm2/m512/m32bcst``
 
 ``EVEX.512.66.0F38.W0 C4 /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTQ_XMM_K1Z_XMMM128B64: Code = 3593 # type: ignore
+EVEX_VPCONFLICTQ_XMM_K1Z_XMMM128B64: int = 3593
 """
 ``VPCONFLICTQ xmm1 {k1}{z}, xmm2/m128/m64bcst``
 
 ``EVEX.128.66.0F38.W1 C4 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTQ_YMM_K1Z_YMMM256B64: Code = 3594 # type: ignore
+EVEX_VPCONFLICTQ_YMM_K1Z_YMMM256B64: int = 3594
 """
 ``VPCONFLICTQ ymm1 {k1}{z}, ymm2/m256/m64bcst``
 
 ``EVEX.256.66.0F38.W1 C4 /r``
 
 ``AVX512VL and AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VPCONFLICTQ_ZMM_K1Z_ZMMM512B64: Code = 3595 # type: ignore
+EVEX_VPCONFLICTQ_ZMM_K1Z_ZMMM512B64: int = 3595
 """
 ``VPCONFLICTQ zmm1 {k1}{z}, zmm2/m512/m64bcst``
 
 ``EVEX.512.66.0F38.W1 C4 /r``
 
 ``AVX512CD``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF0DPS_VM32Z_K1: Code = 3596 # type: ignore
+EVEX_VGATHERPF0DPS_VM32Z_K1: int = 3596
 """
 ``VGATHERPF0DPS vm32z {k1}``
 
 ``EVEX.512.66.0F38.W0 C6 /1 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF0DPD_VM32Y_K1: Code = 3597 # type: ignore
+EVEX_VGATHERPF0DPD_VM32Y_K1: int = 3597
 """
 ``VGATHERPF0DPD vm32y {k1}``
 
 ``EVEX.512.66.0F38.W1 C6 /1 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF1DPS_VM32Z_K1: Code = 3598 # type: ignore
+EVEX_VGATHERPF1DPS_VM32Z_K1: int = 3598
 """
 ``VGATHERPF1DPS vm32z {k1}``
 
 ``EVEX.512.66.0F38.W0 C6 /2 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF1DPD_VM32Y_K1: Code = 3599 # type: ignore
+EVEX_VGATHERPF1DPD_VM32Y_K1: int = 3599
 """
 ``VGATHERPF1DPD vm32y {k1}``
 
 ``EVEX.512.66.0F38.W1 C6 /2 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF0DPS_VM32Z_K1: Code = 3600 # type: ignore
+EVEX_VSCATTERPF0DPS_VM32Z_K1: int = 3600
 """
 ``VSCATTERPF0DPS vm32z {k1}``
 
 ``EVEX.512.66.0F38.W0 C6 /5 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF0DPD_VM32Y_K1: Code = 3601 # type: ignore
+EVEX_VSCATTERPF0DPD_VM32Y_K1: int = 3601
 """
 ``VSCATTERPF0DPD vm32y {k1}``
 
 ``EVEX.512.66.0F38.W1 C6 /5 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF1DPS_VM32Z_K1: Code = 3602 # type: ignore
+EVEX_VSCATTERPF1DPS_VM32Z_K1: int = 3602
 """
 ``VSCATTERPF1DPS vm32z {k1}``
 
 ``EVEX.512.66.0F38.W0 C6 /6 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF1DPD_VM32Y_K1: Code = 3603 # type: ignore
+EVEX_VSCATTERPF1DPD_VM32Y_K1: int = 3603
 """
 ``VSCATTERPF1DPD vm32y {k1}``
 
 ``EVEX.512.66.0F38.W1 C6 /6 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF0QPS_VM64Z_K1: Code = 3604 # type: ignore
+EVEX_VGATHERPF0QPS_VM64Z_K1: int = 3604
 """
 ``VGATHERPF0QPS vm64z {k1}``
 
 ``EVEX.512.66.0F38.W0 C7 /1 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF0QPD_VM64Z_K1: Code = 3605 # type: ignore
+EVEX_VGATHERPF0QPD_VM64Z_K1: int = 3605
 """
 ``VGATHERPF0QPD vm64z {k1}``
 
 ``EVEX.512.66.0F38.W1 C7 /1 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF1QPS_VM64Z_K1: Code = 3606 # type: ignore
+EVEX_VGATHERPF1QPS_VM64Z_K1: int = 3606
 """
 ``VGATHERPF1QPS vm64z {k1}``
 
 ``EVEX.512.66.0F38.W0 C7 /2 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VGATHERPF1QPD_VM64Z_K1: Code = 3607 # type: ignore
+EVEX_VGATHERPF1QPD_VM64Z_K1: int = 3607
 """
 ``VGATHERPF1QPD vm64z {k1}``
 
 ``EVEX.512.66.0F38.W1 C7 /2 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF0QPS_VM64Z_K1: Code = 3608 # type: ignore
+EVEX_VSCATTERPF0QPS_VM64Z_K1: int = 3608
 """
 ``VSCATTERPF0QPS vm64z {k1}``
 
 ``EVEX.512.66.0F38.W0 C7 /5 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF0QPD_VM64Z_K1: Code = 3609 # type: ignore
+EVEX_VSCATTERPF0QPD_VM64Z_K1: int = 3609
 """
 ``VSCATTERPF0QPD vm64z {k1}``
 
 ``EVEX.512.66.0F38.W1 C7 /5 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF1QPS_VM64Z_K1: Code = 3610 # type: ignore
+EVEX_VSCATTERPF1QPS_VM64Z_K1: int = 3610
 """
 ``VSCATTERPF1QPS vm64z {k1}``
 
 ``EVEX.512.66.0F38.W0 C7 /6 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-EVEX_VSCATTERPF1QPD_VM64Z_K1: Code = 3611 # type: ignore
+EVEX_VSCATTERPF1QPD_VM64Z_K1: int = 3611
 """
 ``VSCATTERPF1QPD vm64z {k1}``
 
 ``EVEX.512.66.0F38.W1 C7 /6 /vsib``
 
 ``AVX512PF``
 
 ``16/32/64-bit``
 """
-SHA1NEXTE_XMM_XMMM128: Code = 3612 # type: ignore
+SHA1NEXTE_XMM_XMMM128: int = 3612
 """
 ``SHA1NEXTE xmm1, xmm2/m128``
 
 ``NP 0F 38 C8 /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-EVEX_VEXP2PS_ZMM_K1Z_ZMMM512B32_SAE: Code = 3613 # type: ignore
+EVEX_VEXP2PS_ZMM_K1Z_ZMMM512B32_SAE: int = 3613
 """
 ``VEXP2PS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.66.0F38.W0 C8 /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-EVEX_VEXP2PD_ZMM_K1Z_ZMMM512B64_SAE: Code = 3614 # type: ignore
+EVEX_VEXP2PD_ZMM_K1Z_ZMMM512B64_SAE: int = 3614
 """
 ``VEXP2PD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F38.W1 C8 /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-SHA1MSG1_XMM_XMMM128: Code = 3615 # type: ignore
+SHA1MSG1_XMM_XMMM128: int = 3615
 """
 ``SHA1MSG1 xmm1, xmm2/m128``
 
 ``NP 0F 38 C9 /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-SHA1MSG2_XMM_XMMM128: Code = 3616 # type: ignore
+SHA1MSG2_XMM_XMMM128: int = 3616
 """
 ``SHA1MSG2 xmm1, xmm2/m128``
 
 ``NP 0F 38 CA /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP28PS_ZMM_K1Z_ZMMM512B32_SAE: Code = 3617 # type: ignore
+EVEX_VRCP28PS_ZMM_K1Z_ZMMM512B32_SAE: int = 3617
 """
 ``VRCP28PS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.66.0F38.W0 CA /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP28PD_ZMM_K1Z_ZMMM512B64_SAE: Code = 3618 # type: ignore
+EVEX_VRCP28PD_ZMM_K1Z_ZMMM512B64_SAE: int = 3618
 """
 ``VRCP28PD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F38.W1 CA /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-SHA256RNDS2_XMM_XMMM128: Code = 3619 # type: ignore
+SHA256RNDS2_XMM_XMMM128: int = 3619
 """
 ``SHA256RNDS2 xmm1, xmm2/m128, <XMM0>``
 
 ``NP 0F 38 CB /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP28SS_XMM_K1Z_XMM_XMMM32_SAE: Code = 3620 # type: ignore
+EVEX_VRCP28SS_XMM_K1Z_XMM_XMMM32_SAE: int = 3620
 """
 ``VRCP28SS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.66.0F38.W0 CB /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-EVEX_VRCP28SD_XMM_K1Z_XMM_XMMM64_SAE: Code = 3621 # type: ignore
+EVEX_VRCP28SD_XMM_K1Z_XMM_XMMM64_SAE: int = 3621
 """
 ``VRCP28SD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}``
 
 ``EVEX.LIG.66.0F38.W1 CB /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-SHA256MSG1_XMM_XMMM128: Code = 3622 # type: ignore
+SHA256MSG1_XMM_XMMM128: int = 3622
 """
 ``SHA256MSG1 xmm1, xmm2/m128``
 
 ``NP 0F 38 CC /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT28PS_ZMM_K1Z_ZMMM512B32_SAE: Code = 3623 # type: ignore
+EVEX_VRSQRT28PS_ZMM_K1Z_ZMMM512B32_SAE: int = 3623
 """
 ``VRSQRT28PS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}``
 
 ``EVEX.512.66.0F38.W0 CC /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT28PD_ZMM_K1Z_ZMMM512B64_SAE: Code = 3624 # type: ignore
+EVEX_VRSQRT28PD_ZMM_K1Z_ZMMM512B64_SAE: int = 3624
 """
 ``VRSQRT28PD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}``
 
 ``EVEX.512.66.0F38.W1 CC /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-SHA256MSG2_XMM_XMMM128: Code = 3625 # type: ignore
+SHA256MSG2_XMM_XMMM128: int = 3625
 """
 ``SHA256MSG2 xmm1, xmm2/m128``
 
 ``NP 0F 38 CD /r``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT28SS_XMM_K1Z_XMM_XMMM32_SAE: Code = 3626 # type: ignore
+EVEX_VRSQRT28SS_XMM_K1Z_XMM_XMMM32_SAE: int = 3626
 """
 ``VRSQRT28SS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}``
 
 ``EVEX.LIG.66.0F38.W0 CD /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-EVEX_VRSQRT28SD_XMM_K1Z_XMM_XMMM64_SAE: Code = 3627 # type: ignore
+EVEX_VRSQRT28SD_XMM_K1Z_XMM_XMMM64_SAE: int = 3627
 """
 ``VRSQRT28SD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}``
 
 ``EVEX.LIG.66.0F38.W1 CD /r``
 
 ``AVX512ER``
 
 ``16/32/64-bit``
 """
-GF2P8MULB_XMM_XMMM128: Code = 3628 # type: ignore
+GF2P8MULB_XMM_XMMM128: int = 3628
 """
 ``GF2P8MULB xmm1, xmm2/m128``
 
 ``66 0F 38 CF /r``
 
 ``GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8MULB_XMM_XMM_XMMM128: Code = 3629 # type: ignore
+VEX_VGF2P8MULB_XMM_XMM_XMMM128: int = 3629
 """
 ``VGF2P8MULB xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 CF /r``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8MULB_YMM_YMM_YMMM256: Code = 3630 # type: ignore
+VEX_VGF2P8MULB_YMM_YMM_YMMM256: int = 3630
 """
 ``VGF2P8MULB ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 CF /r``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8MULB_XMM_K1Z_XMM_XMMM128: Code = 3631 # type: ignore
+EVEX_VGF2P8MULB_XMM_K1Z_XMM_XMMM128: int = 3631
 """
 ``VGF2P8MULB xmm1 {k1}{z}, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.W0 CF /r``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8MULB_YMM_K1Z_YMM_YMMM256: Code = 3632 # type: ignore
+EVEX_VGF2P8MULB_YMM_K1Z_YMM_YMMM256: int = 3632
 """
 ``VGF2P8MULB ymm1 {k1}{z}, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.W0 CF /r``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8MULB_ZMM_K1Z_ZMM_ZMMM512: Code = 3633 # type: ignore
+EVEX_VGF2P8MULB_ZMM_K1Z_ZMM_ZMMM512: int = 3633
 """
 ``VGF2P8MULB zmm1 {k1}{z}, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.W0 CF /r``
 
 ``AVX512F and GFNI``
 
 ``16/32/64-bit``
 """
-AESIMC_XMM_XMMM128: Code = 3634 # type: ignore
+AESIMC_XMM_XMMM128: int = 3634
 """
 ``AESIMC xmm1, xmm2/m128``
 
 ``66 0F 38 DB /r``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESIMC_XMM_XMMM128: Code = 3635 # type: ignore
+VEX_VAESIMC_XMM_XMMM128: int = 3635
 """
 ``VAESIMC xmm1, xmm2/m128``
 
 ``VEX.128.66.0F38.WIG DB /r``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-AESENC_XMM_XMMM128: Code = 3636 # type: ignore
+AESENC_XMM_XMMM128: int = 3636
 """
 ``AESENC xmm1, xmm2/m128``
 
 ``66 0F 38 DC /r``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESENC_XMM_XMM_XMMM128: Code = 3637 # type: ignore
+VEX_VAESENC_XMM_XMM_XMMM128: int = 3637
 """
 ``VAESENC xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG DC /r``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-VEX_VAESENC_YMM_YMM_YMMM256: Code = 3638 # type: ignore
+VEX_VAESENC_YMM_YMM_YMMM256: int = 3638
 """
 ``VAESENC ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG DC /r``
 
 ``VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENC_XMM_XMM_XMMM128: Code = 3639 # type: ignore
+EVEX_VAESENC_XMM_XMM_XMMM128: int = 3639
 """
 ``VAESENC xmm1, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG DC /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENC_YMM_YMM_YMMM256: Code = 3640 # type: ignore
+EVEX_VAESENC_YMM_YMM_YMMM256: int = 3640
 """
 ``VAESENC ymm1, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG DC /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENC_ZMM_ZMM_ZMMM512: Code = 3641 # type: ignore
+EVEX_VAESENC_ZMM_ZMM_ZMMM512: int = 3641
 """
 ``VAESENC zmm1, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG DC /r``
 
 ``AVX512F and VAES``
 
 ``16/32/64-bit``
 """
-AESENCLAST_XMM_XMMM128: Code = 3642 # type: ignore
+AESENCLAST_XMM_XMMM128: int = 3642
 """
 ``AESENCLAST xmm1, xmm2/m128``
 
 ``66 0F 38 DD /r``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESENCLAST_XMM_XMM_XMMM128: Code = 3643 # type: ignore
+VEX_VAESENCLAST_XMM_XMM_XMMM128: int = 3643
 """
 ``VAESENCLAST xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG DD /r``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-VEX_VAESENCLAST_YMM_YMM_YMMM256: Code = 3644 # type: ignore
+VEX_VAESENCLAST_YMM_YMM_YMMM256: int = 3644
 """
 ``VAESENCLAST ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG DD /r``
 
 ``VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENCLAST_XMM_XMM_XMMM128: Code = 3645 # type: ignore
+EVEX_VAESENCLAST_XMM_XMM_XMMM128: int = 3645
 """
 ``VAESENCLAST xmm1, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG DD /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENCLAST_YMM_YMM_YMMM256: Code = 3646 # type: ignore
+EVEX_VAESENCLAST_YMM_YMM_YMMM256: int = 3646
 """
 ``VAESENCLAST ymm1, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG DD /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESENCLAST_ZMM_ZMM_ZMMM512: Code = 3647 # type: ignore
+EVEX_VAESENCLAST_ZMM_ZMM_ZMMM512: int = 3647
 """
 ``VAESENCLAST zmm1, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG DD /r``
 
 ``AVX512F and VAES``
 
 ``16/32/64-bit``
 """
-AESDEC_XMM_XMMM128: Code = 3648 # type: ignore
+AESDEC_XMM_XMMM128: int = 3648
 """
 ``AESDEC xmm1, xmm2/m128``
 
 ``66 0F 38 DE /r``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESDEC_XMM_XMM_XMMM128: Code = 3649 # type: ignore
+VEX_VAESDEC_XMM_XMM_XMMM128: int = 3649
 """
 ``VAESDEC xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG DE /r``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-VEX_VAESDEC_YMM_YMM_YMMM256: Code = 3650 # type: ignore
+VEX_VAESDEC_YMM_YMM_YMMM256: int = 3650
 """
 ``VAESDEC ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG DE /r``
 
 ``VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDEC_XMM_XMM_XMMM128: Code = 3651 # type: ignore
+EVEX_VAESDEC_XMM_XMM_XMMM128: int = 3651
 """
 ``VAESDEC xmm1, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG DE /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDEC_YMM_YMM_YMMM256: Code = 3652 # type: ignore
+EVEX_VAESDEC_YMM_YMM_YMMM256: int = 3652
 """
 ``VAESDEC ymm1, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG DE /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDEC_ZMM_ZMM_ZMMM512: Code = 3653 # type: ignore
+EVEX_VAESDEC_ZMM_ZMM_ZMMM512: int = 3653
 """
 ``VAESDEC zmm1, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG DE /r``
 
 ``AVX512F and VAES``
 
 ``16/32/64-bit``
 """
-AESDECLAST_XMM_XMMM128: Code = 3654 # type: ignore
+AESDECLAST_XMM_XMMM128: int = 3654
 """
 ``AESDECLAST xmm1, xmm2/m128``
 
 ``66 0F 38 DF /r``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESDECLAST_XMM_XMM_XMMM128: Code = 3655 # type: ignore
+VEX_VAESDECLAST_XMM_XMM_XMMM128: int = 3655
 """
 ``VAESDECLAST xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.WIG DF /r``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-VEX_VAESDECLAST_YMM_YMM_YMMM256: Code = 3656 # type: ignore
+VEX_VAESDECLAST_YMM_YMM_YMMM256: int = 3656
 """
 ``VAESDECLAST ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.WIG DF /r``
 
 ``VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDECLAST_XMM_XMM_XMMM128: Code = 3657 # type: ignore
+EVEX_VAESDECLAST_XMM_XMM_XMMM128: int = 3657
 """
 ``VAESDECLAST xmm1, xmm2, xmm3/m128``
 
 ``EVEX.128.66.0F38.WIG DF /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDECLAST_YMM_YMM_YMMM256: Code = 3658 # type: ignore
+EVEX_VAESDECLAST_YMM_YMM_YMMM256: int = 3658
 """
 ``VAESDECLAST ymm1, ymm2, ymm3/m256``
 
 ``EVEX.256.66.0F38.WIG DF /r``
 
 ``AVX512VL and VAES``
 
 ``16/32/64-bit``
 """
-EVEX_VAESDECLAST_ZMM_ZMM_ZMMM512: Code = 3659 # type: ignore
+EVEX_VAESDECLAST_ZMM_ZMM_ZMMM512: int = 3659
 """
 ``VAESDECLAST zmm1, zmm2, zmm3/m512``
 
 ``EVEX.512.66.0F38.WIG DF /r``
 
 ``AVX512F and VAES``
 
 ``16/32/64-bit``
 """
-MOVBE_R16_M16: Code = 3660 # type: ignore
+MOVBE_R16_M16: int = 3660
 """
 ``MOVBE r16, m16``
 
 ``o16 0F 38 F0 /r``
 
 ``MOVBE``
 
 ``16/32/64-bit``
 """
-MOVBE_R32_M32: Code = 3661 # type: ignore
+MOVBE_R32_M32: int = 3661
 """
 ``MOVBE r32, m32``
 
 ``o32 0F 38 F0 /r``
 
 ``MOVBE``
 
 ``16/32/64-bit``
 """
-MOVBE_R64_M64: Code = 3662 # type: ignore
+MOVBE_R64_M64: int = 3662
 """
 ``MOVBE r64, m64``
 
 ``o64 0F 38 F0 /r``
 
 ``MOVBE``
 
 ``64-bit``
 """
-CRC32_R32_RM8: Code = 3663 # type: ignore
+CRC32_R32_RM8: int = 3663
 """
 ``CRC32 r32, r/m8``
 
 ``F2 0F 38 F0 /r``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-CRC32_R64_RM8: Code = 3664 # type: ignore
+CRC32_R64_RM8: int = 3664
 """
 ``CRC32 r64, r/m8``
 
 ``F2 o64 0F 38 F0 /r``
 
 ``SSE4.2``
 
 ``64-bit``
 """
-MOVBE_M16_R16: Code = 3665 # type: ignore
+MOVBE_M16_R16: int = 3665
 """
 ``MOVBE m16, r16``
 
 ``o16 0F 38 F1 /r``
 
 ``MOVBE``
 
 ``16/32/64-bit``
 """
-MOVBE_M32_R32: Code = 3666 # type: ignore
+MOVBE_M32_R32: int = 3666
 """
 ``MOVBE m32, r32``
 
 ``o32 0F 38 F1 /r``
 
 ``MOVBE``
 
 ``16/32/64-bit``
 """
-MOVBE_M64_R64: Code = 3667 # type: ignore
+MOVBE_M64_R64: int = 3667
 """
 ``MOVBE m64, r64``
 
 ``o64 0F 38 F1 /r``
 
 ``MOVBE``
 
 ``64-bit``
 """
-CRC32_R32_RM16: Code = 3668 # type: ignore
+CRC32_R32_RM16: int = 3668
 """
 ``CRC32 r32, r/m16``
 
 ``o16 F2 0F 38 F1 /r``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-CRC32_R32_RM32: Code = 3669 # type: ignore
+CRC32_R32_RM32: int = 3669
 """
 ``CRC32 r32, r/m32``
 
 ``o32 F2 0F 38 F1 /r``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-CRC32_R64_RM64: Code = 3670 # type: ignore
+CRC32_R64_RM64: int = 3670
 """
 ``CRC32 r64, r/m64``
 
 ``F2 o64 0F 38 F1 /r``
 
 ``SSE4.2``
 
 ``64-bit``
 """
-VEX_ANDN_R32_R32_RM32: Code = 3671 # type: ignore
+VEX_ANDN_R32_R32_RM32: int = 3671
 """
 ``ANDN r32a, r32b, r/m32``
 
 ``VEX.LZ.0F38.W0 F2 /r``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-VEX_ANDN_R64_R64_RM64: Code = 3672 # type: ignore
+VEX_ANDN_R64_R64_RM64: int = 3672
 """
 ``ANDN r64a, r64b, r/m64``
 
 ``VEX.LZ.0F38.W1 F2 /r``
 
 ``BMI1``
 
 ``64-bit``
 """
-VEX_BLSR_R32_RM32: Code = 3673 # type: ignore
+VEX_BLSR_R32_RM32: int = 3673
 """
 ``BLSR r32, r/m32``
 
 ``VEX.LZ.0F38.W0 F3 /1``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-VEX_BLSR_R64_RM64: Code = 3674 # type: ignore
+VEX_BLSR_R64_RM64: int = 3674
 """
 ``BLSR r64, r/m64``
 
 ``VEX.LZ.0F38.W1 F3 /1``
 
 ``BMI1``
 
 ``64-bit``
 """
-VEX_BLSMSK_R32_RM32: Code = 3675 # type: ignore
+VEX_BLSMSK_R32_RM32: int = 3675
 """
 ``BLSMSK r32, r/m32``
 
 ``VEX.LZ.0F38.W0 F3 /2``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-VEX_BLSMSK_R64_RM64: Code = 3676 # type: ignore
+VEX_BLSMSK_R64_RM64: int = 3676
 """
 ``BLSMSK r64, r/m64``
 
 ``VEX.LZ.0F38.W1 F3 /2``
 
 ``BMI1``
 
 ``64-bit``
 """
-VEX_BLSI_R32_RM32: Code = 3677 # type: ignore
+VEX_BLSI_R32_RM32: int = 3677
 """
 ``BLSI r32, r/m32``
 
 ``VEX.LZ.0F38.W0 F3 /3``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-VEX_BLSI_R64_RM64: Code = 3678 # type: ignore
+VEX_BLSI_R64_RM64: int = 3678
 """
 ``BLSI r64, r/m64``
 
 ``VEX.LZ.0F38.W1 F3 /3``
 
 ``BMI1``
 
 ``64-bit``
 """
-VEX_BZHI_R32_RM32_R32: Code = 3679 # type: ignore
+VEX_BZHI_R32_RM32_R32: int = 3679
 """
 ``BZHI r32a, r/m32, r32b``
 
 ``VEX.LZ.0F38.W0 F5 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_BZHI_R64_RM64_R64: Code = 3680 # type: ignore
+VEX_BZHI_R64_RM64_R64: int = 3680
 """
 ``BZHI r64a, r/m64, r64b``
 
 ``VEX.LZ.0F38.W1 F5 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-WRUSSD_M32_R32: Code = 3681 # type: ignore
+WRUSSD_M32_R32: int = 3681
 """
 ``WRUSSD m32, r32``
 
 ``66 0F 38 F5 /r``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-WRUSSQ_M64_R64: Code = 3682 # type: ignore
+WRUSSQ_M64_R64: int = 3682
 """
 ``WRUSSQ m64, r64``
 
 ``66 o64 0F 38 F5 /r``
 
 ``CET_SS``
 
 ``64-bit``
 """
-VEX_PEXT_R32_R32_RM32: Code = 3683 # type: ignore
+VEX_PEXT_R32_R32_RM32: int = 3683
 """
 ``PEXT r32a, r32b, r/m32``
 
 ``VEX.LZ.F3.0F38.W0 F5 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_PEXT_R64_R64_RM64: Code = 3684 # type: ignore
+VEX_PEXT_R64_R64_RM64: int = 3684
 """
 ``PEXT r64a, r64b, r/m64``
 
 ``VEX.LZ.F3.0F38.W1 F5 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-VEX_PDEP_R32_R32_RM32: Code = 3685 # type: ignore
+VEX_PDEP_R32_R32_RM32: int = 3685
 """
 ``PDEP r32a, r32b, r/m32``
 
 ``VEX.LZ.F2.0F38.W0 F5 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_PDEP_R64_R64_RM64: Code = 3686 # type: ignore
+VEX_PDEP_R64_R64_RM64: int = 3686
 """
 ``PDEP r64a, r64b, r/m64``
 
 ``VEX.LZ.F2.0F38.W1 F5 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-WRSSD_M32_R32: Code = 3687 # type: ignore
+WRSSD_M32_R32: int = 3687
 """
 ``WRSSD m32, r32``
 
 ``NP 0F 38 F6 /r``
 
 ``CET_SS``
 
 ``16/32/64-bit``
 """
-WRSSQ_M64_R64: Code = 3688 # type: ignore
+WRSSQ_M64_R64: int = 3688
 """
 ``WRSSQ m64, r64``
 
 ``NP o64 0F 38 F6 /r``
 
 ``CET_SS``
 
 ``64-bit``
 """
-ADCX_R32_RM32: Code = 3689 # type: ignore
+ADCX_R32_RM32: int = 3689
 """
 ``ADCX r32, r/m32``
 
 ``66 0F 38 F6 /r``
 
 ``ADX``
 
 ``16/32/64-bit``
 """
-ADCX_R64_RM64: Code = 3690 # type: ignore
+ADCX_R64_RM64: int = 3690
 """
 ``ADCX r64, r/m64``
 
 ``66 o64 0F 38 F6 /r``
 
 ``ADX``
 
 ``64-bit``
 """
-ADOX_R32_RM32: Code = 3691 # type: ignore
+ADOX_R32_RM32: int = 3691
 """
 ``ADOX r32, r/m32``
 
 ``F3 0F 38 F6 /r``
 
 ``ADX``
 
 ``16/32/64-bit``
 """
-ADOX_R64_RM64: Code = 3692 # type: ignore
+ADOX_R64_RM64: int = 3692
 """
 ``ADOX r64, r/m64``
 
 ``F3 o64 0F 38 F6 /r``
 
 ``ADX``
 
 ``64-bit``
 """
-VEX_MULX_R32_R32_RM32: Code = 3693 # type: ignore
+VEX_MULX_R32_R32_RM32: int = 3693
 """
 ``MULX r32a, r32b, r/m32``
 
 ``VEX.LZ.F2.0F38.W0 F6 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_MULX_R64_R64_RM64: Code = 3694 # type: ignore
+VEX_MULX_R64_R64_RM64: int = 3694
 """
 ``MULX r64a, r64b, r/m64``
 
 ``VEX.LZ.F2.0F38.W1 F6 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-VEX_BEXTR_R32_RM32_R32: Code = 3695 # type: ignore
+VEX_BEXTR_R32_RM32_R32: int = 3695
 """
 ``BEXTR r32a, r/m32, r32b``
 
 ``VEX.LZ.0F38.W0 F7 /r``
 
 ``BMI1``
 
 ``16/32/64-bit``
 """
-VEX_BEXTR_R64_RM64_R64: Code = 3696 # type: ignore
+VEX_BEXTR_R64_RM64_R64: int = 3696
 """
 ``BEXTR r64a, r/m64, r64b``
 
 ``VEX.LZ.0F38.W1 F7 /r``
 
 ``BMI1``
 
 ``64-bit``
 """
-VEX_SHLX_R32_RM32_R32: Code = 3697 # type: ignore
+VEX_SHLX_R32_RM32_R32: int = 3697
 """
 ``SHLX r32a, r/m32, r32b``
 
 ``VEX.LZ.66.0F38.W0 F7 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_SHLX_R64_RM64_R64: Code = 3698 # type: ignore
+VEX_SHLX_R64_RM64_R64: int = 3698
 """
 ``SHLX r64a, r/m64, r64b``
 
 ``VEX.LZ.66.0F38.W1 F7 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-VEX_SARX_R32_RM32_R32: Code = 3699 # type: ignore
+VEX_SARX_R32_RM32_R32: int = 3699
 """
 ``SARX r32a, r/m32, r32b``
 
 ``VEX.LZ.F3.0F38.W0 F7 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_SARX_R64_RM64_R64: Code = 3700 # type: ignore
+VEX_SARX_R64_RM64_R64: int = 3700
 """
 ``SARX r64a, r/m64, r64b``
 
 ``VEX.LZ.F3.0F38.W1 F7 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-VEX_SHRX_R32_RM32_R32: Code = 3701 # type: ignore
+VEX_SHRX_R32_RM32_R32: int = 3701
 """
 ``SHRX r32a, r/m32, r32b``
 
 ``VEX.LZ.F2.0F38.W0 F7 /r``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_SHRX_R64_RM64_R64: Code = 3702 # type: ignore
+VEX_SHRX_R64_RM64_R64: int = 3702
 """
 ``SHRX r64a, r/m64, r64b``
 
 ``VEX.LZ.F2.0F38.W1 F7 /r``
 
 ``BMI2``
 
 ``64-bit``
 """
-MOVDIR64B_R16_M512: Code = 3703 # type: ignore
+MOVDIR64B_R16_M512: int = 3703
 """
 ``MOVDIR64B r16, m512``
 
 ``a16 66 0F 38 F8 /r``
 
 ``MOVDIR64B``
 
 ``16/32-bit``
 """
-MOVDIR64B_R32_M512: Code = 3704 # type: ignore
+MOVDIR64B_R32_M512: int = 3704
 """
 ``MOVDIR64B r32, m512``
 
 ``a32 66 0F 38 F8 /r``
 
 ``MOVDIR64B``
 
 ``16/32/64-bit``
 """
-MOVDIR64B_R64_M512: Code = 3705 # type: ignore
+MOVDIR64B_R64_M512: int = 3705
 """
 ``MOVDIR64B r64, m512``
 
 ``a64 66 0F 38 F8 /r``
 
 ``MOVDIR64B``
 
 ``64-bit``
 """
-ENQCMDS_R16_M512: Code = 3706 # type: ignore
+ENQCMDS_R16_M512: int = 3706
 """
 ``ENQCMDS r16, m512``
 
 ``a16 F3 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``16/32-bit``
 """
-ENQCMDS_R32_M512: Code = 3707 # type: ignore
+ENQCMDS_R32_M512: int = 3707
 """
 ``ENQCMDS r32, m512``
 
 ``a32 F3 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``16/32/64-bit``
 """
-ENQCMDS_R64_M512: Code = 3708 # type: ignore
+ENQCMDS_R64_M512: int = 3708
 """
 ``ENQCMDS r64, m512``
 
 ``a64 F3 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``64-bit``
 """
-ENQCMD_R16_M512: Code = 3709 # type: ignore
+ENQCMD_R16_M512: int = 3709
 """
 ``ENQCMD r16, m512``
 
 ``a16 F2 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``16/32-bit``
 """
-ENQCMD_R32_M512: Code = 3710 # type: ignore
+ENQCMD_R32_M512: int = 3710
 """
 ``ENQCMD r32, m512``
 
 ``a32 F2 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``16/32/64-bit``
 """
-ENQCMD_R64_M512: Code = 3711 # type: ignore
+ENQCMD_R64_M512: int = 3711
 """
 ``ENQCMD r64, m512``
 
 ``a64 F2 0F 38 F8 !(11):rrr:bbb``
 
 ``ENQCMD``
 
 ``64-bit``
 """
-MOVDIRI_M32_R32: Code = 3712 # type: ignore
+MOVDIRI_M32_R32: int = 3712
 """
 ``MOVDIRI m32, r32``
 
 ``NP 0F 38 F9 /r``
 
 ``MOVDIRI``
 
 ``16/32/64-bit``
 """
-MOVDIRI_M64_R64: Code = 3713 # type: ignore
+MOVDIRI_M64_R64: int = 3713
 """
 ``MOVDIRI m64, r64``
 
 ``NP o64 0F 38 F9 /r``
 
 ``MOVDIRI``
 
 ``64-bit``
 """
-VEX_VPERMQ_YMM_YMMM256_IMM8: Code = 3714 # type: ignore
+VEX_VPERMQ_YMM_YMMM256_IMM8: int = 3714
 """
 ``VPERMQ ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.W1 00 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMQ_YMM_K1Z_YMMM256B64_IMM8: Code = 3715 # type: ignore
+EVEX_VPERMQ_YMM_K1Z_YMMM256B64_IMM8: int = 3715
 """
 ``VPERMQ ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 00 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMQ_ZMM_K1Z_ZMMM512B64_IMM8: Code = 3716 # type: ignore
+EVEX_VPERMQ_ZMM_K1Z_ZMMM512B64_IMM8: int = 3716
 """
 ``VPERMQ zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 00 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMPD_YMM_YMMM256_IMM8: Code = 3717 # type: ignore
+VEX_VPERMPD_YMM_YMMM256_IMM8: int = 3717
 """
 ``VPERMPD ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.W1 01 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPD_YMM_K1Z_YMMM256B64_IMM8: Code = 3718 # type: ignore
+EVEX_VPERMPD_YMM_K1Z_YMMM256B64_IMM8: int = 3718
 """
 ``VPERMPD ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 01 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMPD_ZMM_K1Z_ZMMM512B64_IMM8: Code = 3719 # type: ignore
+EVEX_VPERMPD_ZMM_K1Z_ZMMM512B64_IMM8: int = 3719
 """
 ``VPERMPD zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 01 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDD_XMM_XMM_XMMM128_IMM8: Code = 3720 # type: ignore
+VEX_VPBLENDD_XMM_XMM_XMMM128_IMM8: int = 3720
 """
 ``VPBLENDD xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.W0 02 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDD_YMM_YMM_YMMM256_IMM8: Code = 3721 # type: ignore
+VEX_VPBLENDD_YMM_YMM_YMMM256_IMM8: int = 3721
 """
 ``VPBLENDD ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.W0 02 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGND_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 3722 # type: ignore
+EVEX_VALIGND_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 3722
 """
 ``VALIGND xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 03 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGND_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3723 # type: ignore
+EVEX_VALIGND_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3723
 """
 ``VALIGND ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 03 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGND_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 3724 # type: ignore
+EVEX_VALIGND_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 3724
 """
 ``VALIGND zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 03 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGNQ_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 3725 # type: ignore
+EVEX_VALIGNQ_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 3725
 """
 ``VALIGNQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 03 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGNQ_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3726 # type: ignore
+EVEX_VALIGNQ_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3726
 """
 ``VALIGNQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 03 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VALIGNQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 3727 # type: ignore
+EVEX_VALIGNQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 3727
 """
 ``VALIGNQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 03 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPS_XMM_XMMM128_IMM8: Code = 3728 # type: ignore
+VEX_VPERMILPS_XMM_XMMM128_IMM8: int = 3728
 """
 ``VPERMILPS xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W0 04 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPS_YMM_YMMM256_IMM8: Code = 3729 # type: ignore
+VEX_VPERMILPS_YMM_YMMM256_IMM8: int = 3729
 """
 ``VPERMILPS ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.W0 04 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_XMM_K1Z_XMMM128B32_IMM8: Code = 3730 # type: ignore
+EVEX_VPERMILPS_XMM_K1Z_XMMM128B32_IMM8: int = 3730
 """
 ``VPERMILPS xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 04 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_YMM_K1Z_YMMM256B32_IMM8: Code = 3731 # type: ignore
+EVEX_VPERMILPS_YMM_K1Z_YMMM256B32_IMM8: int = 3731
 """
 ``VPERMILPS ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 04 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPS_ZMM_K1Z_ZMMM512B32_IMM8: Code = 3732 # type: ignore
+EVEX_VPERMILPS_ZMM_K1Z_ZMMM512B32_IMM8: int = 3732
 """
 ``VPERMILPS zmm1 {k1}{z}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 04 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPD_XMM_XMMM128_IMM8: Code = 3733 # type: ignore
+VEX_VPERMILPD_XMM_XMMM128_IMM8: int = 3733
 """
 ``VPERMILPD xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W0 05 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPERMILPD_YMM_YMMM256_IMM8: Code = 3734 # type: ignore
+VEX_VPERMILPD_YMM_YMMM256_IMM8: int = 3734
 """
 ``VPERMILPD ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.W0 05 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_XMM_K1Z_XMMM128B64_IMM8: Code = 3735 # type: ignore
+EVEX_VPERMILPD_XMM_K1Z_XMMM128B64_IMM8: int = 3735
 """
 ``VPERMILPD xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 05 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_YMM_K1Z_YMMM256B64_IMM8: Code = 3736 # type: ignore
+EVEX_VPERMILPD_YMM_K1Z_YMMM256B64_IMM8: int = 3736
 """
 ``VPERMILPD ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 05 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPERMILPD_ZMM_K1Z_ZMMM512B64_IMM8: Code = 3737 # type: ignore
+EVEX_VPERMILPD_ZMM_K1Z_ZMMM512B64_IMM8: int = 3737
 """
 ``VPERMILPD zmm1 {k1}{z}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 05 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VPERM2F128_YMM_YMM_YMMM256_IMM8: Code = 3738 # type: ignore
+VEX_VPERM2F128_YMM_YMM_YMMM256_IMM8: int = 3738
 """
 ``VPERM2F128 ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.W0 06 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-ROUNDPS_XMM_XMMM128_IMM8: Code = 3739 # type: ignore
+ROUNDPS_XMM_XMMM128_IMM8: int = 3739
 """
 ``ROUNDPS xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 08 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDPS_XMM_XMMM128_IMM8: Code = 3740 # type: ignore
+VEX_VROUNDPS_XMM_XMMM128_IMM8: int = 3740
 """
 ``VROUNDPS xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 08 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDPS_YMM_YMMM256_IMM8: Code = 3741 # type: ignore
+VEX_VROUNDPS_YMM_YMMM256_IMM8: int = 3741
 """
 ``VROUNDPS ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 08 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPS_XMM_K1Z_XMMM128B32_IMM8: Code = 3742 # type: ignore
+EVEX_VRNDSCALEPS_XMM_K1Z_XMMM128B32_IMM8: int = 3742
 """
 ``VRNDSCALEPS xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 08 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPS_YMM_K1Z_YMMM256B32_IMM8: Code = 3743 # type: ignore
+EVEX_VRNDSCALEPS_YMM_K1Z_YMMM256B32_IMM8: int = 3743
 """
 ``VRNDSCALEPS ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 08 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: Code = 3744 # type: ignore
+EVEX_VRNDSCALEPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: int = 3744
 """
 ``VRNDSCALEPS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 08 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ROUNDPD_XMM_XMMM128_IMM8: Code = 3745 # type: ignore
+ROUNDPD_XMM_XMMM128_IMM8: int = 3745
 """
 ``ROUNDPD xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 09 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDPD_XMM_XMMM128_IMM8: Code = 3746 # type: ignore
+VEX_VROUNDPD_XMM_XMMM128_IMM8: int = 3746
 """
 ``VROUNDPD xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 09 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDPD_YMM_YMMM256_IMM8: Code = 3747 # type: ignore
+VEX_VROUNDPD_YMM_YMMM256_IMM8: int = 3747
 """
 ``VROUNDPD ymm1, ymm2/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 09 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPD_XMM_K1Z_XMMM128B64_IMM8: Code = 3748 # type: ignore
+EVEX_VRNDSCALEPD_XMM_K1Z_XMMM128B64_IMM8: int = 3748
 """
 ``VRNDSCALEPD xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 09 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPD_YMM_K1Z_YMMM256B64_IMM8: Code = 3749 # type: ignore
+EVEX_VRNDSCALEPD_YMM_K1Z_YMMM256B64_IMM8: int = 3749
 """
 ``VRNDSCALEPD ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 09 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALEPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: Code = 3750 # type: ignore
+EVEX_VRNDSCALEPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: int = 3750
 """
 ``VRNDSCALEPD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W1 09 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ROUNDSS_XMM_XMMM32_IMM8: Code = 3751 # type: ignore
+ROUNDSS_XMM_XMMM32_IMM8: int = 3751
 """
 ``ROUNDSS xmm1, xmm2/m32, imm8``
 
 ``66 0F 3A 0A /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDSS_XMM_XMM_XMMM32_IMM8: Code = 3752 # type: ignore
+VEX_VROUNDSS_XMM_XMM_XMMM32_IMM8: int = 3752
 """
 ``VROUNDSS xmm1, xmm2, xmm3/m32, imm8``
 
 ``VEX.LIG.66.0F3A.WIG 0A /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: Code = 3753 # type: ignore
+EVEX_VRNDSCALESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: int = 3753
 """
 ``VRNDSCALESS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 0A /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-ROUNDSD_XMM_XMMM64_IMM8: Code = 3754 # type: ignore
+ROUNDSD_XMM_XMMM64_IMM8: int = 3754
 """
 ``ROUNDSD xmm1, xmm2/m64, imm8``
 
 ``66 0F 3A 0B /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VROUNDSD_XMM_XMM_XMMM64_IMM8: Code = 3755 # type: ignore
+VEX_VROUNDSD_XMM_XMM_XMMM64_IMM8: int = 3755
 """
 ``VROUNDSD xmm1, xmm2, xmm3/m64, imm8``
 
 ``VEX.LIG.66.0F3A.WIG 0B /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VRNDSCALESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: Code = 3756 # type: ignore
+EVEX_VRNDSCALESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: int = 3756
 """
 ``VRNDSCALESD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 0B /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-BLENDPS_XMM_XMMM128_IMM8: Code = 3757 # type: ignore
+BLENDPS_XMM_XMMM128_IMM8: int = 3757
 """
 ``BLENDPS xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 0C /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDPS_XMM_XMM_XMMM128_IMM8: Code = 3758 # type: ignore
+VEX_VBLENDPS_XMM_XMM_XMMM128_IMM8: int = 3758
 """
 ``VBLENDPS xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 0C /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDPS_YMM_YMM_YMMM256_IMM8: Code = 3759 # type: ignore
+VEX_VBLENDPS_YMM_YMM_YMMM256_IMM8: int = 3759
 """
 ``VBLENDPS ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 0C /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-BLENDPD_XMM_XMMM128_IMM8: Code = 3760 # type: ignore
+BLENDPD_XMM_XMMM128_IMM8: int = 3760
 """
 ``BLENDPD xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 0D /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDPD_XMM_XMM_XMMM128_IMM8: Code = 3761 # type: ignore
+VEX_VBLENDPD_XMM_XMM_XMMM128_IMM8: int = 3761
 """
 ``VBLENDPD xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 0D /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDPD_YMM_YMM_YMMM256_IMM8: Code = 3762 # type: ignore
+VEX_VBLENDPD_YMM_YMM_YMMM256_IMM8: int = 3762
 """
 ``VBLENDPD ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 0D /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PBLENDW_XMM_XMMM128_IMM8: Code = 3763 # type: ignore
+PBLENDW_XMM_XMMM128_IMM8: int = 3763
 """
 ``PBLENDW xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 0E /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDW_XMM_XMM_XMMM128_IMM8: Code = 3764 # type: ignore
+VEX_VPBLENDW_XMM_XMM_XMMM128_IMM8: int = 3764
 """
 ``VPBLENDW xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 0E /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDW_YMM_YMM_YMMM256_IMM8: Code = 3765 # type: ignore
+VEX_VPBLENDW_YMM_YMM_YMMM256_IMM8: int = 3765
 """
 ``VPBLENDW ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 0E /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-PALIGNR_MM_MMM64_IMM8: Code = 3766 # type: ignore
+PALIGNR_MM_MMM64_IMM8: int = 3766
 """
 ``PALIGNR mm1, mm2/m64, imm8``
 
 ``NP 0F 3A 0F /r ib``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-PALIGNR_XMM_XMMM128_IMM8: Code = 3767 # type: ignore
+PALIGNR_XMM_XMMM128_IMM8: int = 3767
 """
 ``PALIGNR xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 0F /r ib``
 
 ``SSSE3``
 
 ``16/32/64-bit``
 """
-VEX_VPALIGNR_XMM_XMM_XMMM128_IMM8: Code = 3768 # type: ignore
+VEX_VPALIGNR_XMM_XMM_XMMM128_IMM8: int = 3768
 """
 ``VPALIGNR xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 0F /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPALIGNR_YMM_YMM_YMMM256_IMM8: Code = 3769 # type: ignore
+VEX_VPALIGNR_YMM_YMM_YMMM256_IMM8: int = 3769
 """
 ``VPALIGNR ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 0F /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VPALIGNR_XMM_K1Z_XMM_XMMM128_IMM8: Code = 3770 # type: ignore
+EVEX_VPALIGNR_XMM_K1Z_XMM_XMMM128_IMM8: int = 3770
 """
 ``VPALIGNR xmm1 {k1}{z}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.WIG 0F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPALIGNR_YMM_K1Z_YMM_YMMM256_IMM8: Code = 3771 # type: ignore
+EVEX_VPALIGNR_YMM_K1Z_YMM_YMMM256_IMM8: int = 3771
 """
 ``VPALIGNR ymm1 {k1}{z}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.WIG 0F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPALIGNR_ZMM_K1Z_ZMM_ZMMM512_IMM8: Code = 3772 # type: ignore
+EVEX_VPALIGNR_ZMM_K1Z_ZMM_ZMMM512_IMM8: int = 3772
 """
 ``VPALIGNR zmm1 {k1}{z}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.WIG 0F /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-PEXTRB_R32M8_XMM_IMM8: Code = 3773 # type: ignore
+PEXTRB_R32M8_XMM_IMM8: int = 3773
 """
 ``PEXTRB r32/m8, xmm2, imm8``
 
 ``66 0F 3A 14 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-PEXTRB_R64M8_XMM_IMM8: Code = 3774 # type: ignore
+PEXTRB_R64M8_XMM_IMM8: int = 3774
 """
 ``PEXTRB r64/m8, xmm2, imm8``
 
 ``66 o64 0F 3A 14 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VPEXTRB_R32M8_XMM_IMM8: Code = 3775 # type: ignore
+VEX_VPEXTRB_R32M8_XMM_IMM8: int = 3775
 """
 ``VPEXTRB r32/m8, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W0 14 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPEXTRB_R64M8_XMM_IMM8: Code = 3776 # type: ignore
+VEX_VPEXTRB_R64M8_XMM_IMM8: int = 3776
 """
 ``VPEXTRB r64/m8, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W1 14 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPEXTRB_R32M8_XMM_IMM8: Code = 3777 # type: ignore
+EVEX_VPEXTRB_R32M8_XMM_IMM8: int = 3777
 """
 ``VPEXTRB r32/m8, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W0 14 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXTRB_R64M8_XMM_IMM8: Code = 3778 # type: ignore
+EVEX_VPEXTRB_R64M8_XMM_IMM8: int = 3778
 """
 ``VPEXTRB r64/m8, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W1 14 /r ib``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-PEXTRW_R32M16_XMM_IMM8: Code = 3779 # type: ignore
+PEXTRW_R32M16_XMM_IMM8: int = 3779
 """
 ``PEXTRW r32/m16, xmm, imm8``
 
 ``66 0F 3A 15 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-PEXTRW_R64M16_XMM_IMM8: Code = 3780 # type: ignore
+PEXTRW_R64M16_XMM_IMM8: int = 3780
 """
 ``PEXTRW r64/m16, xmm, imm8``
 
 ``66 o64 0F 3A 15 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VPEXTRW_R32M16_XMM_IMM8: Code = 3781 # type: ignore
+VEX_VPEXTRW_R32M16_XMM_IMM8: int = 3781
 """
 ``VPEXTRW r32/m16, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W0 15 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPEXTRW_R64M16_XMM_IMM8: Code = 3782 # type: ignore
+VEX_VPEXTRW_R64M16_XMM_IMM8: int = 3782
 """
 ``VPEXTRW r64/m16, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W1 15 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPEXTRW_R32M16_XMM_IMM8: Code = 3783 # type: ignore
+EVEX_VPEXTRW_R32M16_XMM_IMM8: int = 3783
 """
 ``VPEXTRW r32/m16, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W0 15 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXTRW_R64M16_XMM_IMM8: Code = 3784 # type: ignore
+EVEX_VPEXTRW_R64M16_XMM_IMM8: int = 3784
 """
 ``VPEXTRW r64/m16, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W1 15 /r ib``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-PEXTRD_RM32_XMM_IMM8: Code = 3785 # type: ignore
+PEXTRD_RM32_XMM_IMM8: int = 3785
 """
 ``PEXTRD r/m32, xmm2, imm8``
 
 ``66 0F 3A 16 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-PEXTRQ_RM64_XMM_IMM8: Code = 3786 # type: ignore
+PEXTRQ_RM64_XMM_IMM8: int = 3786
 """
 ``PEXTRQ r/m64, xmm2, imm8``
 
 ``66 o64 0F 3A 16 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VPEXTRD_RM32_XMM_IMM8: Code = 3787 # type: ignore
+VEX_VPEXTRD_RM32_XMM_IMM8: int = 3787
 """
 ``VPEXTRD r/m32, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W0 16 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPEXTRQ_RM64_XMM_IMM8: Code = 3788 # type: ignore
+VEX_VPEXTRQ_RM64_XMM_IMM8: int = 3788
 """
 ``VPEXTRQ r/m64, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W1 16 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPEXTRD_RM32_XMM_IMM8: Code = 3789 # type: ignore
+EVEX_VPEXTRD_RM32_XMM_IMM8: int = 3789
 """
 ``VPEXTRD r/m32, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W0 16 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPEXTRQ_RM64_XMM_IMM8: Code = 3790 # type: ignore
+EVEX_VPEXTRQ_RM64_XMM_IMM8: int = 3790
 """
 ``VPEXTRQ r/m64, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W1 16 /r ib``
 
 ``AVX512DQ``
 
 ``64-bit``
 """
-EXTRACTPS_RM32_XMM_IMM8: Code = 3791 # type: ignore
+EXTRACTPS_RM32_XMM_IMM8: int = 3791
 """
 ``EXTRACTPS r/m32, xmm1, imm8``
 
 ``66 0F 3A 17 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-EXTRACTPS_R64M32_XMM_IMM8: Code = 3792 # type: ignore
+EXTRACTPS_R64M32_XMM_IMM8: int = 3792
 """
 ``EXTRACTPS r64/m32, xmm1, imm8``
 
 ``66 o64 0F 3A 17 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VEXTRACTPS_RM32_XMM_IMM8: Code = 3793 # type: ignore
+VEX_VEXTRACTPS_RM32_XMM_IMM8: int = 3793
 """
 ``VEXTRACTPS r/m32, xmm1, imm8``
 
 ``VEX.128.66.0F3A.W0 17 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VEXTRACTPS_R64M32_XMM_IMM8: Code = 3794 # type: ignore
+VEX_VEXTRACTPS_R64M32_XMM_IMM8: int = 3794
 """
 ``VEXTRACTPS r64/m32, xmm1, imm8``
 
 ``VEX.128.66.0F3A.W1 17 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VEXTRACTPS_RM32_XMM_IMM8: Code = 3795 # type: ignore
+EVEX_VEXTRACTPS_RM32_XMM_IMM8: int = 3795
 """
 ``VEXTRACTPS r/m32, xmm1, imm8``
 
 ``EVEX.128.66.0F3A.W0 17 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTPS_R64M32_XMM_IMM8: Code = 3796 # type: ignore
+EVEX_VEXTRACTPS_R64M32_XMM_IMM8: int = 3796
 """
 ``VEXTRACTPS r64/m32, xmm1, imm8``
 
 ``EVEX.128.66.0F3A.W1 17 /r ib``
 
 ``AVX512F``
 
 ``64-bit``
 """
-VEX_VINSERTF128_YMM_YMM_XMMM128_IMM8: Code = 3797 # type: ignore
+VEX_VINSERTF128_YMM_YMM_XMMM128_IMM8: int = 3797
 """
 ``VINSERTF128 ymm1, ymm2, xmm3/m128, imm8``
 
 ``VEX.256.66.0F3A.W0 18 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF32X4_YMM_K1Z_YMM_XMMM128_IMM8: Code = 3798 # type: ignore
+EVEX_VINSERTF32X4_YMM_K1Z_YMM_XMMM128_IMM8: int = 3798
 """
 ``VINSERTF32X4 ymm1 {k1}{z}, ymm2, xmm3/m128, imm8``
 
 ``EVEX.256.66.0F3A.W0 18 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF32X4_ZMM_K1Z_ZMM_XMMM128_IMM8: Code = 3799 # type: ignore
+EVEX_VINSERTF32X4_ZMM_K1Z_ZMM_XMMM128_IMM8: int = 3799
 """
 ``VINSERTF32X4 zmm1 {k1}{z}, zmm2, xmm3/m128, imm8``
 
 ``EVEX.512.66.0F3A.W0 18 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF64X2_YMM_K1Z_YMM_XMMM128_IMM8: Code = 3800 # type: ignore
+EVEX_VINSERTF64X2_YMM_K1Z_YMM_XMMM128_IMM8: int = 3800
 """
 ``VINSERTF64X2 ymm1 {k1}{z}, ymm2, xmm3/m128, imm8``
 
 ``EVEX.256.66.0F3A.W1 18 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF64X2_ZMM_K1Z_ZMM_XMMM128_IMM8: Code = 3801 # type: ignore
+EVEX_VINSERTF64X2_ZMM_K1Z_ZMM_XMMM128_IMM8: int = 3801
 """
 ``VINSERTF64X2 zmm1 {k1}{z}, zmm2, xmm3/m128, imm8``
 
 ``EVEX.512.66.0F3A.W1 18 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_VEXTRACTF128_XMMM128_YMM_IMM8: Code = 3802 # type: ignore
+VEX_VEXTRACTF128_XMMM128_YMM_IMM8: int = 3802
 """
 ``VEXTRACTF128 xmm1/m128, ymm2, imm8``
 
 ``VEX.256.66.0F3A.W0 19 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF32X4_XMMM128_K1Z_YMM_IMM8: Code = 3803 # type: ignore
+EVEX_VEXTRACTF32X4_XMMM128_K1Z_YMM_IMM8: int = 3803
 """
 ``VEXTRACTF32X4 xmm1/m128 {k1}{z}, ymm2, imm8``
 
 ``EVEX.256.66.0F3A.W0 19 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF32X4_XMMM128_K1Z_ZMM_IMM8: Code = 3804 # type: ignore
+EVEX_VEXTRACTF32X4_XMMM128_K1Z_ZMM_IMM8: int = 3804
 """
 ``VEXTRACTF32X4 xmm1/m128 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W0 19 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF64X2_XMMM128_K1Z_YMM_IMM8: Code = 3805 # type: ignore
+EVEX_VEXTRACTF64X2_XMMM128_K1Z_YMM_IMM8: int = 3805
 """
 ``VEXTRACTF64X2 xmm1/m128 {k1}{z}, ymm2, imm8``
 
 ``EVEX.256.66.0F3A.W1 19 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF64X2_XMMM128_K1Z_ZMM_IMM8: Code = 3806 # type: ignore
+EVEX_VEXTRACTF64X2_XMMM128_K1Z_ZMM_IMM8: int = 3806
 """
 ``VEXTRACTF64X2 xmm1/m128 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W1 19 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF32X8_ZMM_K1Z_ZMM_YMMM256_IMM8: Code = 3807 # type: ignore
+EVEX_VINSERTF32X8_ZMM_K1Z_ZMM_YMMM256_IMM8: int = 3807
 """
 ``VINSERTF32X8 zmm1 {k1}{z}, zmm2, ymm3/m256, imm8``
 
 ``EVEX.512.66.0F3A.W0 1A /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTF64X4_ZMM_K1Z_ZMM_YMMM256_IMM8: Code = 3808 # type: ignore
+EVEX_VINSERTF64X4_ZMM_K1Z_ZMM_YMMM256_IMM8: int = 3808
 """
 ``VINSERTF64X4 zmm1 {k1}{z}, zmm2, ymm3/m256, imm8``
 
 ``EVEX.512.66.0F3A.W1 1A /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF32X8_YMMM256_K1Z_ZMM_IMM8: Code = 3809 # type: ignore
+EVEX_VEXTRACTF32X8_YMMM256_K1Z_ZMM_IMM8: int = 3809
 """
 ``VEXTRACTF32X8 ymm1/m256 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W0 1B /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTF64X4_YMMM256_K1Z_ZMM_IMM8: Code = 3810 # type: ignore
+EVEX_VEXTRACTF64X4_YMMM256_K1Z_ZMM_IMM8: int = 3810
 """
 ``VEXTRACTF64X4 ymm1/m256 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W1 1B /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2PH_XMMM64_XMM_IMM8: Code = 3811 # type: ignore
+VEX_VCVTPS2PH_XMMM64_XMM_IMM8: int = 3811
 """
 ``VCVTPS2PH xmm1/m64, xmm2, imm8``
 
 ``VEX.128.66.0F3A.W0 1D /r ib``
 
 ``F16C``
 
 ``16/32/64-bit``
 """
-VEX_VCVTPS2PH_XMMM128_YMM_IMM8: Code = 3812 # type: ignore
+VEX_VCVTPS2PH_XMMM128_YMM_IMM8: int = 3812
 """
 ``VCVTPS2PH xmm1/m128, ymm2, imm8``
 
 ``VEX.256.66.0F3A.W0 1D /r ib``
 
 ``F16C``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PH_XMMM64_K1Z_XMM_IMM8: Code = 3813 # type: ignore
+EVEX_VCVTPS2PH_XMMM64_K1Z_XMM_IMM8: int = 3813
 """
 ``VCVTPS2PH xmm1/m64 {k1}{z}, xmm2, imm8``
 
 ``EVEX.128.66.0F3A.W0 1D /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PH_XMMM128_K1Z_YMM_IMM8: Code = 3814 # type: ignore
+EVEX_VCVTPS2PH_XMMM128_K1Z_YMM_IMM8: int = 3814
 """
 ``VCVTPS2PH xmm1/m128 {k1}{z}, ymm2, imm8``
 
 ``EVEX.256.66.0F3A.W0 1D /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VCVTPS2PH_YMMM256_K1Z_ZMM_IMM8_SAE: Code = 3815 # type: ignore
+EVEX_VCVTPS2PH_YMMM256_K1Z_ZMM_IMM8_SAE: int = 3815
 """
 ``VCVTPS2PH ymm1/m256 {k1}{z}, zmm2{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 1D /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUD_KR_K1_XMM_XMMM128B32_IMM8: Code = 3816 # type: ignore
+EVEX_VPCMPUD_KR_K1_XMM_XMMM128B32_IMM8: int = 3816
 """
 ``VPCMPUD k1 {k2}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 1E /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUD_KR_K1_YMM_YMMM256B32_IMM8: Code = 3817 # type: ignore
+EVEX_VPCMPUD_KR_K1_YMM_YMMM256B32_IMM8: int = 3817
 """
 ``VPCMPUD k1 {k2}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 1E /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUD_KR_K1_ZMM_ZMMM512B32_IMM8: Code = 3818 # type: ignore
+EVEX_VPCMPUD_KR_K1_ZMM_ZMMM512B32_IMM8: int = 3818
 """
 ``VPCMPUD k1 {k2}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 1E /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUQ_KR_K1_XMM_XMMM128B64_IMM8: Code = 3819 # type: ignore
+EVEX_VPCMPUQ_KR_K1_XMM_XMMM128B64_IMM8: int = 3819
 """
 ``VPCMPUQ k1 {k2}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 1E /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUQ_KR_K1_YMM_YMMM256B64_IMM8: Code = 3820 # type: ignore
+EVEX_VPCMPUQ_KR_K1_YMM_YMMM256B64_IMM8: int = 3820
 """
 ``VPCMPUQ k1 {k2}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 1E /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUQ_KR_K1_ZMM_ZMMM512B64_IMM8: Code = 3821 # type: ignore
+EVEX_VPCMPUQ_KR_K1_ZMM_ZMMM512B64_IMM8: int = 3821
 """
 ``VPCMPUQ k1 {k2}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 1E /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPD_KR_K1_XMM_XMMM128B32_IMM8: Code = 3822 # type: ignore
+EVEX_VPCMPD_KR_K1_XMM_XMMM128B32_IMM8: int = 3822
 """
 ``VPCMPD k1 {k2}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 1F /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPD_KR_K1_YMM_YMMM256B32_IMM8: Code = 3823 # type: ignore
+EVEX_VPCMPD_KR_K1_YMM_YMMM256B32_IMM8: int = 3823
 """
 ``VPCMPD k1 {k2}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 1F /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPD_KR_K1_ZMM_ZMMM512B32_IMM8: Code = 3824 # type: ignore
+EVEX_VPCMPD_KR_K1_ZMM_ZMMM512B32_IMM8: int = 3824
 """
 ``VPCMPD k1 {k2}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 1F /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPQ_KR_K1_XMM_XMMM128B64_IMM8: Code = 3825 # type: ignore
+EVEX_VPCMPQ_KR_K1_XMM_XMMM128B64_IMM8: int = 3825
 """
 ``VPCMPQ k1 {k2}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 1F /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPQ_KR_K1_YMM_YMMM256B64_IMM8: Code = 3826 # type: ignore
+EVEX_VPCMPQ_KR_K1_YMM_YMMM256B64_IMM8: int = 3826
 """
 ``VPCMPQ k1 {k2}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 1F /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPQ_KR_K1_ZMM_ZMMM512B64_IMM8: Code = 3827 # type: ignore
+EVEX_VPCMPQ_KR_K1_ZMM_ZMMM512B64_IMM8: int = 3827
 """
 ``VPCMPQ k1 {k2}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 1F /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PINSRB_XMM_R32M8_IMM8: Code = 3828 # type: ignore
+PINSRB_XMM_R32M8_IMM8: int = 3828
 """
 ``PINSRB xmm1, r32/m8, imm8``
 
 ``66 0F 3A 20 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-PINSRB_XMM_R64M8_IMM8: Code = 3829 # type: ignore
+PINSRB_XMM_R64M8_IMM8: int = 3829
 """
 ``PINSRB xmm1, r64/m8, imm8``
 
 ``66 o64 0F 3A 20 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VPINSRB_XMM_XMM_R32M8_IMM8: Code = 3830 # type: ignore
+VEX_VPINSRB_XMM_XMM_R32M8_IMM8: int = 3830
 """
 ``VPINSRB xmm1, xmm2, r32/m8, imm8``
 
 ``VEX.128.66.0F3A.W0 20 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPINSRB_XMM_XMM_R64M8_IMM8: Code = 3831 # type: ignore
+VEX_VPINSRB_XMM_XMM_R64M8_IMM8: int = 3831
 """
 ``VPINSRB xmm1, xmm2, r64/m8, imm8``
 
 ``VEX.128.66.0F3A.W1 20 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPINSRB_XMM_XMM_R32M8_IMM8: Code = 3832 # type: ignore
+EVEX_VPINSRB_XMM_XMM_R32M8_IMM8: int = 3832
 """
 ``VPINSRB xmm1, xmm2, r32/m8, imm8``
 
 ``EVEX.128.66.0F3A.W0 20 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPINSRB_XMM_XMM_R64M8_IMM8: Code = 3833 # type: ignore
+EVEX_VPINSRB_XMM_XMM_R64M8_IMM8: int = 3833
 """
 ``VPINSRB xmm1, xmm2, r64/m8, imm8``
 
 ``EVEX.128.66.0F3A.W1 20 /r ib``
 
 ``AVX512BW``
 
 ``64-bit``
 """
-INSERTPS_XMM_XMMM32_IMM8: Code = 3834 # type: ignore
+INSERTPS_XMM_XMMM32_IMM8: int = 3834
 """
 ``INSERTPS xmm1, xmm2/m32, imm8``
 
 ``66 0F 3A 21 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VINSERTPS_XMM_XMM_XMMM32_IMM8: Code = 3835 # type: ignore
+VEX_VINSERTPS_XMM_XMM_XMMM32_IMM8: int = 3835
 """
 ``VINSERTPS xmm1, xmm2, xmm3/m32, imm8``
 
 ``VEX.128.66.0F3A.WIG 21 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTPS_XMM_XMM_XMMM32_IMM8: Code = 3836 # type: ignore
+EVEX_VINSERTPS_XMM_XMM_XMMM32_IMM8: int = 3836
 """
 ``VINSERTPS xmm1, xmm2, xmm3/m32, imm8``
 
 ``EVEX.128.66.0F3A.W0 21 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PINSRD_XMM_RM32_IMM8: Code = 3837 # type: ignore
+PINSRD_XMM_RM32_IMM8: int = 3837
 """
 ``PINSRD xmm1, r/m32, imm8``
 
 ``66 0F 3A 22 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-PINSRQ_XMM_RM64_IMM8: Code = 3838 # type: ignore
+PINSRQ_XMM_RM64_IMM8: int = 3838
 """
 ``PINSRQ xmm1, r/m64, imm8``
 
 ``66 o64 0F 3A 22 /r ib``
 
 ``SSE4.1``
 
 ``64-bit``
 """
-VEX_VPINSRD_XMM_XMM_RM32_IMM8: Code = 3839 # type: ignore
+VEX_VPINSRD_XMM_XMM_RM32_IMM8: int = 3839
 """
 ``VPINSRD xmm1, xmm2, r/m32, imm8``
 
 ``VEX.128.66.0F3A.W0 22 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPINSRQ_XMM_XMM_RM64_IMM8: Code = 3840 # type: ignore
+VEX_VPINSRQ_XMM_XMM_RM64_IMM8: int = 3840
 """
 ``VPINSRQ xmm1, xmm2, r/m64, imm8``
 
 ``VEX.128.66.0F3A.W1 22 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-EVEX_VPINSRD_XMM_XMM_RM32_IMM8: Code = 3841 # type: ignore
+EVEX_VPINSRD_XMM_XMM_RM32_IMM8: int = 3841
 """
 ``VPINSRD xmm1, xmm2, r/m32, imm8``
 
 ``EVEX.128.66.0F3A.W0 22 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPINSRQ_XMM_XMM_RM64_IMM8: Code = 3842 # type: ignore
+EVEX_VPINSRQ_XMM_XMM_RM64_IMM8: int = 3842
 """
 ``VPINSRQ xmm1, xmm2, r/m64, imm8``
 
 ``EVEX.128.66.0F3A.W1 22 /r ib``
 
 ``AVX512DQ``
 
 ``64-bit``
 """
-EVEX_VSHUFF32X4_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3843 # type: ignore
+EVEX_VSHUFF32X4_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3843
 """
 ``VSHUFF32X4 ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 23 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFF32X4_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 3844 # type: ignore
+EVEX_VSHUFF32X4_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 3844
 """
 ``VSHUFF32X4 zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 23 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFF64X2_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3845 # type: ignore
+EVEX_VSHUFF64X2_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3845
 """
 ``VSHUFF64X2 ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 23 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFF64X2_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 3846 # type: ignore
+EVEX_VSHUFF64X2_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 3846
 """
 ``VSHUFF64X2 zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 23 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGD_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 3847 # type: ignore
+EVEX_VPTERNLOGD_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 3847
 """
 ``VPTERNLOGD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 25 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGD_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3848 # type: ignore
+EVEX_VPTERNLOGD_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3848
 """
 ``VPTERNLOGD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 25 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 3849 # type: ignore
+EVEX_VPTERNLOGD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 3849
 """
 ``VPTERNLOGD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 25 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGQ_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 3850 # type: ignore
+EVEX_VPTERNLOGQ_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 3850
 """
 ``VPTERNLOGQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 25 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGQ_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3851 # type: ignore
+EVEX_VPTERNLOGQ_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3851
 """
 ``VPTERNLOGQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 25 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPTERNLOGQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 3852 # type: ignore
+EVEX_VPTERNLOGQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 3852
 """
 ``VPTERNLOGQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 25 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPS_XMM_K1Z_XMMM128B32_IMM8: Code = 3853 # type: ignore
+EVEX_VGETMANTPS_XMM_K1Z_XMMM128B32_IMM8: int = 3853
 """
 ``VGETMANTPS xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 26 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPS_YMM_K1Z_YMMM256B32_IMM8: Code = 3854 # type: ignore
+EVEX_VGETMANTPS_YMM_K1Z_YMMM256B32_IMM8: int = 3854
 """
 ``VGETMANTPS ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 26 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: Code = 3855 # type: ignore
+EVEX_VGETMANTPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: int = 3855
 """
 ``VGETMANTPS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 26 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPD_XMM_K1Z_XMMM128B64_IMM8: Code = 3856 # type: ignore
+EVEX_VGETMANTPD_XMM_K1Z_XMMM128B64_IMM8: int = 3856
 """
 ``VGETMANTPD xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 26 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPD_YMM_K1Z_YMMM256B64_IMM8: Code = 3857 # type: ignore
+EVEX_VGETMANTPD_YMM_K1Z_YMMM256B64_IMM8: int = 3857
 """
 ``VGETMANTPD ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 26 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: Code = 3858 # type: ignore
+EVEX_VGETMANTPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: int = 3858
 """
 ``VGETMANTPD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W1 26 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTSS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: Code = 3859 # type: ignore
+EVEX_VGETMANTSS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: int = 3859
 """
 ``VGETMANTSS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 27 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VGETMANTSD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: Code = 3860 # type: ignore
+EVEX_VGETMANTSD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: int = 3860
 """
 ``VGETMANTSD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 27 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTRB_KR_KR_IMM8: Code = 3861 # type: ignore
+VEX_KSHIFTRB_KR_KR_IMM8: int = 3861
 """
 ``KSHIFTRB k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W0 30 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTRW_KR_KR_IMM8: Code = 3862 # type: ignore
+VEX_KSHIFTRW_KR_KR_IMM8: int = 3862
 """
 ``KSHIFTRW k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W1 30 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTRD_KR_KR_IMM8: Code = 3863 # type: ignore
+VEX_KSHIFTRD_KR_KR_IMM8: int = 3863
 """
 ``KSHIFTRD k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W0 31 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTRQ_KR_KR_IMM8: Code = 3864 # type: ignore
+VEX_KSHIFTRQ_KR_KR_IMM8: int = 3864
 """
 ``KSHIFTRQ k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W1 31 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTLB_KR_KR_IMM8: Code = 3865 # type: ignore
+VEX_KSHIFTLB_KR_KR_IMM8: int = 3865
 """
 ``KSHIFTLB k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W0 32 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTLW_KR_KR_IMM8: Code = 3866 # type: ignore
+VEX_KSHIFTLW_KR_KR_IMM8: int = 3866
 """
 ``KSHIFTLW k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W1 32 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTLD_KR_KR_IMM8: Code = 3867 # type: ignore
+VEX_KSHIFTLD_KR_KR_IMM8: int = 3867
 """
 ``KSHIFTLD k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W0 33 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_KSHIFTLQ_KR_KR_IMM8: Code = 3868 # type: ignore
+VEX_KSHIFTLQ_KR_KR_IMM8: int = 3868
 """
 ``KSHIFTLQ k1, k2, imm8``
 
 ``VEX.L0.66.0F3A.W1 33 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-VEX_VINSERTI128_YMM_YMM_XMMM128_IMM8: Code = 3869 # type: ignore
+VEX_VINSERTI128_YMM_YMM_XMMM128_IMM8: int = 3869
 """
 ``VINSERTI128 ymm1, ymm2, xmm3/m128, imm8``
 
 ``VEX.256.66.0F3A.W0 38 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI32X4_YMM_K1Z_YMM_XMMM128_IMM8: Code = 3870 # type: ignore
+EVEX_VINSERTI32X4_YMM_K1Z_YMM_XMMM128_IMM8: int = 3870
 """
 ``VINSERTI32X4 ymm1 {k1}{z}, ymm2, xmm3/m128, imm8``
 
 ``EVEX.256.66.0F3A.W0 38 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI32X4_ZMM_K1Z_ZMM_XMMM128_IMM8: Code = 3871 # type: ignore
+EVEX_VINSERTI32X4_ZMM_K1Z_ZMM_XMMM128_IMM8: int = 3871
 """
 ``VINSERTI32X4 zmm1 {k1}{z}, zmm2, xmm3/m128, imm8``
 
 ``EVEX.512.66.0F3A.W0 38 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI64X2_YMM_K1Z_YMM_XMMM128_IMM8: Code = 3872 # type: ignore
+EVEX_VINSERTI64X2_YMM_K1Z_YMM_XMMM128_IMM8: int = 3872
 """
 ``VINSERTI64X2 ymm1 {k1}{z}, ymm2, xmm3/m128, imm8``
 
 ``EVEX.256.66.0F3A.W1 38 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI64X2_ZMM_K1Z_ZMM_XMMM128_IMM8: Code = 3873 # type: ignore
+EVEX_VINSERTI64X2_ZMM_K1Z_ZMM_XMMM128_IMM8: int = 3873
 """
 ``VINSERTI64X2 zmm1 {k1}{z}, zmm2, xmm3/m128, imm8``
 
 ``EVEX.512.66.0F3A.W1 38 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_VEXTRACTI128_XMMM128_YMM_IMM8: Code = 3874 # type: ignore
+VEX_VEXTRACTI128_XMMM128_YMM_IMM8: int = 3874
 """
 ``VEXTRACTI128 xmm1/m128, ymm2, imm8``
 
 ``VEX.256.66.0F3A.W0 39 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI32X4_XMMM128_K1Z_YMM_IMM8: Code = 3875 # type: ignore
+EVEX_VEXTRACTI32X4_XMMM128_K1Z_YMM_IMM8: int = 3875
 """
 ``VEXTRACTI32X4 xmm1/m128 {k1}{z}, ymm2, imm8``
 
 ``EVEX.256.66.0F3A.W0 39 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI32X4_XMMM128_K1Z_ZMM_IMM8: Code = 3876 # type: ignore
+EVEX_VEXTRACTI32X4_XMMM128_K1Z_ZMM_IMM8: int = 3876
 """
 ``VEXTRACTI32X4 xmm1/m128 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W0 39 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI64X2_XMMM128_K1Z_YMM_IMM8: Code = 3877 # type: ignore
+EVEX_VEXTRACTI64X2_XMMM128_K1Z_YMM_IMM8: int = 3877
 """
 ``VEXTRACTI64X2 xmm1/m128 {k1}{z}, ymm2, imm8``
 
 ``EVEX.256.66.0F3A.W1 39 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI64X2_XMMM128_K1Z_ZMM_IMM8: Code = 3878 # type: ignore
+EVEX_VEXTRACTI64X2_XMMM128_K1Z_ZMM_IMM8: int = 3878
 """
 ``VEXTRACTI64X2 xmm1/m128 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W1 39 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI32X8_ZMM_K1Z_ZMM_YMMM256_IMM8: Code = 3879 # type: ignore
+EVEX_VINSERTI32X8_ZMM_K1Z_ZMM_YMMM256_IMM8: int = 3879
 """
 ``VINSERTI32X8 zmm1 {k1}{z}, zmm2, ymm3/m256, imm8``
 
 ``EVEX.512.66.0F3A.W0 3A /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VINSERTI64X4_ZMM_K1Z_ZMM_YMMM256_IMM8: Code = 3880 # type: ignore
+EVEX_VINSERTI64X4_ZMM_K1Z_ZMM_YMMM256_IMM8: int = 3880
 """
 ``VINSERTI64X4 zmm1 {k1}{z}, zmm2, ymm3/m256, imm8``
 
 ``EVEX.512.66.0F3A.W1 3A /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI32X8_YMMM256_K1Z_ZMM_IMM8: Code = 3881 # type: ignore
+EVEX_VEXTRACTI32X8_YMMM256_K1Z_ZMM_IMM8: int = 3881
 """
 ``VEXTRACTI32X8 ymm1/m256 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W0 3B /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VEXTRACTI64X4_YMMM256_K1Z_ZMM_IMM8: Code = 3882 # type: ignore
+EVEX_VEXTRACTI64X4_YMMM256_K1Z_ZMM_IMM8: int = 3882
 """
 ``VEXTRACTI64X4 ymm1/m256 {k1}{z}, zmm2, imm8``
 
 ``EVEX.512.66.0F3A.W1 3B /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUB_KR_K1_XMM_XMMM128_IMM8: Code = 3883 # type: ignore
+EVEX_VPCMPUB_KR_K1_XMM_XMMM128_IMM8: int = 3883
 """
 ``VPCMPUB k1 {k2}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W0 3E /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUB_KR_K1_YMM_YMMM256_IMM8: Code = 3884 # type: ignore
+EVEX_VPCMPUB_KR_K1_YMM_YMMM256_IMM8: int = 3884
 """
 ``VPCMPUB k1 {k2}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W0 3E /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUB_KR_K1_ZMM_ZMMM512_IMM8: Code = 3885 # type: ignore
+EVEX_VPCMPUB_KR_K1_ZMM_ZMMM512_IMM8: int = 3885
 """
 ``VPCMPUB k1 {k2}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W0 3E /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUW_KR_K1_XMM_XMMM128_IMM8: Code = 3886 # type: ignore
+EVEX_VPCMPUW_KR_K1_XMM_XMMM128_IMM8: int = 3886
 """
 ``VPCMPUW k1 {k2}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W1 3E /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUW_KR_K1_YMM_YMMM256_IMM8: Code = 3887 # type: ignore
+EVEX_VPCMPUW_KR_K1_YMM_YMMM256_IMM8: int = 3887
 """
 ``VPCMPUW k1 {k2}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W1 3E /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPUW_KR_K1_ZMM_ZMMM512_IMM8: Code = 3888 # type: ignore
+EVEX_VPCMPUW_KR_K1_ZMM_ZMMM512_IMM8: int = 3888
 """
 ``VPCMPUW k1 {k2}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W1 3E /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPB_KR_K1_XMM_XMMM128_IMM8: Code = 3889 # type: ignore
+EVEX_VPCMPB_KR_K1_XMM_XMMM128_IMM8: int = 3889
 """
 ``VPCMPB k1 {k2}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W0 3F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPB_KR_K1_YMM_YMMM256_IMM8: Code = 3890 # type: ignore
+EVEX_VPCMPB_KR_K1_YMM_YMMM256_IMM8: int = 3890
 """
 ``VPCMPB k1 {k2}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W0 3F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPB_KR_K1_ZMM_ZMMM512_IMM8: Code = 3891 # type: ignore
+EVEX_VPCMPB_KR_K1_ZMM_ZMMM512_IMM8: int = 3891
 """
 ``VPCMPB k1 {k2}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W0 3F /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPW_KR_K1_XMM_XMMM128_IMM8: Code = 3892 # type: ignore
+EVEX_VPCMPW_KR_K1_XMM_XMMM128_IMM8: int = 3892
 """
 ``VPCMPW k1 {k2}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W1 3F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPW_KR_K1_YMM_YMMM256_IMM8: Code = 3893 # type: ignore
+EVEX_VPCMPW_KR_K1_YMM_YMMM256_IMM8: int = 3893
 """
 ``VPCMPW k1 {k2}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W1 3F /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VPCMPW_KR_K1_ZMM_ZMMM512_IMM8: Code = 3894 # type: ignore
+EVEX_VPCMPW_KR_K1_ZMM_ZMMM512_IMM8: int = 3894
 """
 ``VPCMPW k1 {k2}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W1 3F /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-DPPS_XMM_XMMM128_IMM8: Code = 3895 # type: ignore
+DPPS_XMM_XMMM128_IMM8: int = 3895
 """
 ``DPPS xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 40 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VDPPS_XMM_XMM_XMMM128_IMM8: Code = 3896 # type: ignore
+VEX_VDPPS_XMM_XMM_XMMM128_IMM8: int = 3896
 """
 ``VDPPS xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 40 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VDPPS_YMM_YMM_YMMM256_IMM8: Code = 3897 # type: ignore
+VEX_VDPPS_YMM_YMM_YMMM256_IMM8: int = 3897
 """
 ``VDPPS ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 40 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-DPPD_XMM_XMMM128_IMM8: Code = 3898 # type: ignore
+DPPD_XMM_XMMM128_IMM8: int = 3898
 """
 ``DPPD xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 41 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VDPPD_XMM_XMM_XMMM128_IMM8: Code = 3899 # type: ignore
+VEX_VDPPD_XMM_XMM_XMMM128_IMM8: int = 3899
 """
 ``VDPPD xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 41 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-MPSADBW_XMM_XMMM128_IMM8: Code = 3900 # type: ignore
+MPSADBW_XMM_XMMM128_IMM8: int = 3900
 """
 ``MPSADBW xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 42 /r ib``
 
 ``SSE4.1``
 
 ``16/32/64-bit``
 """
-VEX_VMPSADBW_XMM_XMM_XMMM128_IMM8: Code = 3901 # type: ignore
+VEX_VMPSADBW_XMM_XMM_XMMM128_IMM8: int = 3901
 """
 ``VMPSADBW xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 42 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VMPSADBW_YMM_YMM_YMMM256_IMM8: Code = 3902 # type: ignore
+VEX_VMPSADBW_YMM_YMM_YMMM256_IMM8: int = 3902
 """
 ``VMPSADBW ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 42 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VDBPSADBW_XMM_K1Z_XMM_XMMM128_IMM8: Code = 3903 # type: ignore
+EVEX_VDBPSADBW_XMM_K1Z_XMM_XMMM128_IMM8: int = 3903
 """
 ``VDBPSADBW xmm1 {k1}{z}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W0 42 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VDBPSADBW_YMM_K1Z_YMM_YMMM256_IMM8: Code = 3904 # type: ignore
+EVEX_VDBPSADBW_YMM_K1Z_YMM_YMMM256_IMM8: int = 3904
 """
 ``VDBPSADBW ymm1 {k1}{z}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W0 42 /r ib``
 
 ``AVX512VL and AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VDBPSADBW_ZMM_K1Z_ZMM_ZMMM512_IMM8: Code = 3905 # type: ignore
+EVEX_VDBPSADBW_ZMM_K1Z_ZMM_ZMMM512_IMM8: int = 3905
 """
 ``VDBPSADBW zmm1 {k1}{z}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W0 42 /r ib``
 
 ``AVX512BW``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFI32X4_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3906 # type: ignore
+EVEX_VSHUFI32X4_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3906
 """
 ``VSHUFI32X4 ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 43 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFI32X4_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 3907 # type: ignore
+EVEX_VSHUFI32X4_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 3907
 """
 ``VSHUFI32X4 zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 43 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFI64X2_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3908 # type: ignore
+EVEX_VSHUFI64X2_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3908
 """
 ``VSHUFI64X2 ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 43 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VSHUFI64X2_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 3909 # type: ignore
+EVEX_VSHUFI64X2_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 3909
 """
 ``VSHUFI64X2 zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 43 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-PCLMULQDQ_XMM_XMMM128_IMM8: Code = 3910 # type: ignore
+PCLMULQDQ_XMM_XMMM128_IMM8: int = 3910
 """
 ``PCLMULQDQ xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 44 /r ib``
 
 ``PCLMULQDQ``
 
 ``16/32/64-bit``
 """
-VEX_VPCLMULQDQ_XMM_XMM_XMMM128_IMM8: Code = 3911 # type: ignore
+VEX_VPCLMULQDQ_XMM_XMM_XMMM128_IMM8: int = 3911
 """
 ``VPCLMULQDQ xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 44 /r ib``
 
 ``PCLMULQDQ and AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCLMULQDQ_YMM_YMM_YMMM256_IMM8: Code = 3912 # type: ignore
+VEX_VPCLMULQDQ_YMM_YMM_YMMM256_IMM8: int = 3912
 """
 ``VPCLMULQDQ ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.WIG 44 /r ib``
 
 ``VPCLMULQDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPCLMULQDQ_XMM_XMM_XMMM128_IMM8: Code = 3913 # type: ignore
+EVEX_VPCLMULQDQ_XMM_XMM_XMMM128_IMM8: int = 3913
 """
 ``VPCLMULQDQ xmm1, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.WIG 44 /r ib``
 
 ``AVX512VL and VPCLMULQDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPCLMULQDQ_YMM_YMM_YMMM256_IMM8: Code = 3914 # type: ignore
+EVEX_VPCLMULQDQ_YMM_YMM_YMMM256_IMM8: int = 3914
 """
 ``VPCLMULQDQ ymm1, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.WIG 44 /r ib``
 
 ``AVX512VL and VPCLMULQDQ``
 
 ``16/32/64-bit``
 """
-EVEX_VPCLMULQDQ_ZMM_ZMM_ZMMM512_IMM8: Code = 3915 # type: ignore
+EVEX_VPCLMULQDQ_ZMM_ZMM_ZMMM512_IMM8: int = 3915
 """
 ``VPCLMULQDQ zmm1, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.WIG 44 /r ib``
 
 ``AVX512F and VPCLMULQDQ``
 
 ``16/32/64-bit``
 """
-VEX_VPERM2I128_YMM_YMM_YMMM256_IMM8: Code = 3916 # type: ignore
+VEX_VPERM2I128_YMM_YMM_YMMM256_IMM8: int = 3916
 """
 ``VPERM2I128 ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.W0 46 /r ib``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PS_XMM_XMM_XMMM128_XMM_IMM4: Code = 3917 # type: ignore
+VEX_VPERMIL2PS_XMM_XMM_XMMM128_XMM_IMM4: int = 3917
 """
 ``VPERMIL2PS xmm1, xmm2, xmm3/m128, xmm4, imm4``
 
 ``VEX.128.66.0F3A.W0 48 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PS_YMM_YMM_YMMM256_YMM_IMM4: Code = 3918 # type: ignore
+VEX_VPERMIL2PS_YMM_YMM_YMMM256_YMM_IMM4: int = 3918
 """
 ``VPERMIL2PS ymm1, ymm2, ymm3/m256, ymm4, imm4``
 
 ``VEX.256.66.0F3A.W0 48 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PS_XMM_XMM_XMM_XMMM128_IMM4: Code = 3919 # type: ignore
+VEX_VPERMIL2PS_XMM_XMM_XMM_XMMM128_IMM4: int = 3919
 """
 ``VPERMIL2PS xmm1, xmm2, xmm3, xmm4/m128, imm4``
 
 ``VEX.128.66.0F3A.W1 48 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PS_YMM_YMM_YMM_YMMM256_IMM4: Code = 3920 # type: ignore
+VEX_VPERMIL2PS_YMM_YMM_YMM_YMMM256_IMM4: int = 3920
 """
 ``VPERMIL2PS ymm1, ymm2, ymm3, ymm4/m256, imm4``
 
 ``VEX.256.66.0F3A.W1 48 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PD_XMM_XMM_XMMM128_XMM_IMM4: Code = 3921 # type: ignore
+VEX_VPERMIL2PD_XMM_XMM_XMMM128_XMM_IMM4: int = 3921
 """
 ``VPERMIL2PD xmm1, xmm2, xmm3/m128, xmm4, imm4``
 
 ``VEX.128.66.0F3A.W0 49 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PD_YMM_YMM_YMMM256_YMM_IMM4: Code = 3922 # type: ignore
+VEX_VPERMIL2PD_YMM_YMM_YMMM256_YMM_IMM4: int = 3922
 """
 ``VPERMIL2PD ymm1, ymm2, ymm3/m256, ymm4, imm4``
 
 ``VEX.256.66.0F3A.W0 49 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PD_XMM_XMM_XMM_XMMM128_IMM4: Code = 3923 # type: ignore
+VEX_VPERMIL2PD_XMM_XMM_XMM_XMMM128_IMM4: int = 3923
 """
 ``VPERMIL2PD xmm1, xmm2, xmm3, xmm4/m128, imm4``
 
 ``VEX.128.66.0F3A.W1 49 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VPERMIL2PD_YMM_YMM_YMM_YMMM256_IMM4: Code = 3924 # type: ignore
+VEX_VPERMIL2PD_YMM_YMM_YMM_YMMM256_IMM4: int = 3924
 """
 ``VPERMIL2PD ymm1, ymm2, ymm3, ymm4/m256, imm4``
 
 ``VEX.256.66.0F3A.W1 49 /r /is5``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDVPS_XMM_XMM_XMMM128_XMM: Code = 3925 # type: ignore
+VEX_VBLENDVPS_XMM_XMM_XMMM128_XMM: int = 3925
 """
 ``VBLENDVPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 4A /r /is4``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDVPS_YMM_YMM_YMMM256_YMM: Code = 3926 # type: ignore
+VEX_VBLENDVPS_YMM_YMM_YMMM256_YMM: int = 3926
 """
 ``VBLENDVPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 4A /r /is4``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDVPD_XMM_XMM_XMMM128_XMM: Code = 3927 # type: ignore
+VEX_VBLENDVPD_XMM_XMM_XMMM128_XMM: int = 3927
 """
 ``VBLENDVPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 4B /r /is4``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VBLENDVPD_YMM_YMM_YMMM256_YMM: Code = 3928 # type: ignore
+VEX_VBLENDVPD_YMM_YMM_YMMM256_YMM: int = 3928
 """
 ``VBLENDVPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 4B /r /is4``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDVB_XMM_XMM_XMMM128_XMM: Code = 3929 # type: ignore
+VEX_VPBLENDVB_XMM_XMM_XMMM128_XMM: int = 3929
 """
 ``VPBLENDVB xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 4C /r /is4``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPBLENDVB_YMM_YMM_YMMM256_YMM: Code = 3930 # type: ignore
+VEX_VPBLENDVB_YMM_YMM_YMMM256_YMM: int = 3930
 """
 ``VPBLENDVB ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 4C /r /is4``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPS_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 3931 # type: ignore
+EVEX_VRANGEPS_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 3931
 """
 ``VRANGEPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 50 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPS_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3932 # type: ignore
+EVEX_VRANGEPS_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3932
 """
 ``VRANGEPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 50 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8_SAE: Code = 3933 # type: ignore
+EVEX_VRANGEPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8_SAE: int = 3933
 """
 ``VRANGEPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 50 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPD_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 3934 # type: ignore
+EVEX_VRANGEPD_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 3934
 """
 ``VRANGEPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 50 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPD_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3935 # type: ignore
+EVEX_VRANGEPD_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3935
 """
 ``VRANGEPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 50 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGEPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8_SAE: Code = 3936 # type: ignore
+EVEX_VRANGEPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8_SAE: int = 3936
 """
 ``VRANGEPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W1 50 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: Code = 3937 # type: ignore
+EVEX_VRANGESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: int = 3937
 """
 ``VRANGESS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 51 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VRANGESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: Code = 3938 # type: ignore
+EVEX_VRANGESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: int = 3938
 """
 ``VRANGESD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 51 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPS_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 3939 # type: ignore
+EVEX_VFIXUPIMMPS_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 3939
 """
 ``VFIXUPIMMPS xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 54 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPS_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 3940 # type: ignore
+EVEX_VFIXUPIMMPS_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 3940
 """
 ``VFIXUPIMMPS ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 54 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8_SAE: Code = 3941 # type: ignore
+EVEX_VFIXUPIMMPS_ZMM_K1Z_ZMM_ZMMM512B32_IMM8_SAE: int = 3941
 """
 ``VFIXUPIMMPS zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 54 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPD_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 3942 # type: ignore
+EVEX_VFIXUPIMMPD_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 3942
 """
 ``VFIXUPIMMPD xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 54 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPD_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 3943 # type: ignore
+EVEX_VFIXUPIMMPD_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 3943
 """
 ``VFIXUPIMMPD ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 54 /r ib``
 
 ``AVX512VL and AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8_SAE: Code = 3944 # type: ignore
+EVEX_VFIXUPIMMPD_ZMM_K1Z_ZMM_ZMMM512B64_IMM8_SAE: int = 3944
 """
 ``VFIXUPIMMPD zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W1 54 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMSS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: Code = 3945 # type: ignore
+EVEX_VFIXUPIMMSS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: int = 3945
 """
 ``VFIXUPIMMSS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 55 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VFIXUPIMMSD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: Code = 3946 # type: ignore
+EVEX_VFIXUPIMMSD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: int = 3946
 """
 ``VFIXUPIMMSD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 55 /r ib``
 
 ``AVX512F``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPS_XMM_K1Z_XMMM128B32_IMM8: Code = 3947 # type: ignore
+EVEX_VREDUCEPS_XMM_K1Z_XMMM128B32_IMM8: int = 3947
 """
 ``VREDUCEPS xmm1 {k1}{z}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 56 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPS_YMM_K1Z_YMMM256B32_IMM8: Code = 3948 # type: ignore
+EVEX_VREDUCEPS_YMM_K1Z_YMMM256B32_IMM8: int = 3948
 """
 ``VREDUCEPS ymm1 {k1}{z}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 56 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: Code = 3949 # type: ignore
+EVEX_VREDUCEPS_ZMM_K1Z_ZMMM512B32_IMM8_SAE: int = 3949
 """
 ``VREDUCEPS zmm1 {k1}{z}, zmm2/m512/m32bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W0 56 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPD_XMM_K1Z_XMMM128B64_IMM8: Code = 3950 # type: ignore
+EVEX_VREDUCEPD_XMM_K1Z_XMMM128B64_IMM8: int = 3950
 """
 ``VREDUCEPD xmm1 {k1}{z}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 56 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPD_YMM_K1Z_YMMM256B64_IMM8: Code = 3951 # type: ignore
+EVEX_VREDUCEPD_YMM_K1Z_YMMM256B64_IMM8: int = 3951
 """
 ``VREDUCEPD ymm1 {k1}{z}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 56 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCEPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: Code = 3952 # type: ignore
+EVEX_VREDUCEPD_ZMM_K1Z_ZMMM512B64_IMM8_SAE: int = 3952
 """
 ``VREDUCEPD zmm1 {k1}{z}, zmm2/m512/m64bcst{sae}, imm8``
 
 ``EVEX.512.66.0F3A.W1 56 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: Code = 3953 # type: ignore
+EVEX_VREDUCESS_XMM_K1Z_XMM_XMMM32_IMM8_SAE: int = 3953
 """
 ``VREDUCESS xmm1 {k1}{z}, xmm2, xmm3/m32{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 57 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VREDUCESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: Code = 3954 # type: ignore
+EVEX_VREDUCESD_XMM_K1Z_XMM_XMMM64_IMM8_SAE: int = 3954
 """
 ``VREDUCESD xmm1 {k1}{z}, xmm2, xmm3/m64{sae}, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 57 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPS_XMM_XMM_XMMM128_XMM: Code = 3955 # type: ignore
+VEX_VFMADDSUBPS_XMM_XMM_XMMM128_XMM: int = 3955
 """
 ``VFMADDSUBPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 5C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPS_YMM_YMM_YMMM256_YMM: Code = 3956 # type: ignore
+VEX_VFMADDSUBPS_YMM_YMM_YMMM256_YMM: int = 3956
 """
 ``VFMADDSUBPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 5C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPS_XMM_XMM_XMM_XMMM128: Code = 3957 # type: ignore
+VEX_VFMADDSUBPS_XMM_XMM_XMM_XMMM128: int = 3957
 """
 ``VFMADDSUBPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 5C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPS_YMM_YMM_YMM_YMMM256: Code = 3958 # type: ignore
+VEX_VFMADDSUBPS_YMM_YMM_YMM_YMMM256: int = 3958
 """
 ``VFMADDSUBPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 5C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPD_XMM_XMM_XMMM128_XMM: Code = 3959 # type: ignore
+VEX_VFMADDSUBPD_XMM_XMM_XMMM128_XMM: int = 3959
 """
 ``VFMADDSUBPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 5D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPD_YMM_YMM_YMMM256_YMM: Code = 3960 # type: ignore
+VEX_VFMADDSUBPD_YMM_YMM_YMMM256_YMM: int = 3960
 """
 ``VFMADDSUBPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 5D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPD_XMM_XMM_XMM_XMMM128: Code = 3961 # type: ignore
+VEX_VFMADDSUBPD_XMM_XMM_XMM_XMMM128: int = 3961
 """
 ``VFMADDSUBPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 5D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSUBPD_YMM_YMM_YMM_YMMM256: Code = 3962 # type: ignore
+VEX_VFMADDSUBPD_YMM_YMM_YMM_YMMM256: int = 3962
 """
 ``VFMADDSUBPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 5D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPS_XMM_XMM_XMMM128_XMM: Code = 3963 # type: ignore
+VEX_VFMSUBADDPS_XMM_XMM_XMMM128_XMM: int = 3963
 """
 ``VFMSUBADDPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 5E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPS_YMM_YMM_YMMM256_YMM: Code = 3964 # type: ignore
+VEX_VFMSUBADDPS_YMM_YMM_YMMM256_YMM: int = 3964
 """
 ``VFMSUBADDPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 5E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPS_XMM_XMM_XMM_XMMM128: Code = 3965 # type: ignore
+VEX_VFMSUBADDPS_XMM_XMM_XMM_XMMM128: int = 3965
 """
 ``VFMSUBADDPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 5E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPS_YMM_YMM_YMM_YMMM256: Code = 3966 # type: ignore
+VEX_VFMSUBADDPS_YMM_YMM_YMM_YMMM256: int = 3966
 """
 ``VFMSUBADDPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 5E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPD_XMM_XMM_XMMM128_XMM: Code = 3967 # type: ignore
+VEX_VFMSUBADDPD_XMM_XMM_XMMM128_XMM: int = 3967
 """
 ``VFMSUBADDPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 5F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPD_YMM_YMM_YMMM256_YMM: Code = 3968 # type: ignore
+VEX_VFMSUBADDPD_YMM_YMM_YMMM256_YMM: int = 3968
 """
 ``VFMSUBADDPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 5F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPD_XMM_XMM_XMM_XMMM128: Code = 3969 # type: ignore
+VEX_VFMSUBADDPD_XMM_XMM_XMM_XMMM128: int = 3969
 """
 ``VFMSUBADDPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 5F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBADDPD_YMM_YMM_YMM_YMMM256: Code = 3970 # type: ignore
+VEX_VFMSUBADDPD_YMM_YMM_YMM_YMMM256: int = 3970
 """
 ``VFMSUBADDPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 5F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-PCMPESTRM_XMM_XMMM128_IMM8: Code = 3971 # type: ignore
+PCMPESTRM_XMM_XMMM128_IMM8: int = 3971
 """
 ``PCMPESTRM xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 60 /r ib``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-PCMPESTRM64_XMM_XMMM128_IMM8: Code = 3972 # type: ignore
+PCMPESTRM64_XMM_XMMM128_IMM8: int = 3972
 """
 ``PCMPESTRM64 xmm1, xmm2/m128, imm8``
 
 ``66 o64 0F 3A 60 /r ib``
 
 ``SSE4.2``
 
 ``64-bit``
 """
-VEX_VPCMPESTRM_XMM_XMMM128_IMM8: Code = 3973 # type: ignore
+VEX_VPCMPESTRM_XMM_XMMM128_IMM8: int = 3973
 """
 ``VPCMPESTRM xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W0 60 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPESTRM64_XMM_XMMM128_IMM8: Code = 3974 # type: ignore
+VEX_VPCMPESTRM64_XMM_XMMM128_IMM8: int = 3974
 """
 ``VPCMPESTRM64 xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W1 60 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-PCMPESTRI_XMM_XMMM128_IMM8: Code = 3975 # type: ignore
+PCMPESTRI_XMM_XMMM128_IMM8: int = 3975
 """
 ``PCMPESTRI xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 61 /r ib``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-PCMPESTRI64_XMM_XMMM128_IMM8: Code = 3976 # type: ignore
+PCMPESTRI64_XMM_XMMM128_IMM8: int = 3976
 """
 ``PCMPESTRI64 xmm1, xmm2/m128, imm8``
 
 ``66 o64 0F 3A 61 /r ib``
 
 ``SSE4.2``
 
 ``64-bit``
 """
-VEX_VPCMPESTRI_XMM_XMMM128_IMM8: Code = 3977 # type: ignore
+VEX_VPCMPESTRI_XMM_XMMM128_IMM8: int = 3977
 """
 ``VPCMPESTRI xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W0 61 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPESTRI64_XMM_XMMM128_IMM8: Code = 3978 # type: ignore
+VEX_VPCMPESTRI64_XMM_XMMM128_IMM8: int = 3978
 """
 ``VPCMPESTRI64 xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.W1 61 /r ib``
 
 ``AVX``
 
 ``64-bit``
 """
-PCMPISTRM_XMM_XMMM128_IMM8: Code = 3979 # type: ignore
+PCMPISTRM_XMM_XMMM128_IMM8: int = 3979
 """
 ``PCMPISTRM xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 62 /r ib``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPISTRM_XMM_XMMM128_IMM8: Code = 3980 # type: ignore
+VEX_VPCMPISTRM_XMM_XMMM128_IMM8: int = 3980
 """
 ``VPCMPISTRM xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 62 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-PCMPISTRI_XMM_XMMM128_IMM8: Code = 3981 # type: ignore
+PCMPISTRI_XMM_XMMM128_IMM8: int = 3981
 """
 ``PCMPISTRI xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A 63 /r ib``
 
 ``SSE4.2``
 
 ``16/32/64-bit``
 """
-VEX_VPCMPISTRI_XMM_XMMM128_IMM8: Code = 3982 # type: ignore
+VEX_VPCMPISTRI_XMM_XMMM128_IMM8: int = 3982
 """
 ``VPCMPISTRI xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG 63 /r ib``
 
 ``AVX``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPS_KR_K1_XMMM128B32_IMM8: Code = 3983 # type: ignore
+EVEX_VFPCLASSPS_KR_K1_XMMM128B32_IMM8: int = 3983
 """
 ``VFPCLASSPS k2 {k1}, xmm2/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 66 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPS_KR_K1_YMMM256B32_IMM8: Code = 3984 # type: ignore
+EVEX_VFPCLASSPS_KR_K1_YMMM256B32_IMM8: int = 3984
 """
 ``VFPCLASSPS k2 {k1}, ymm2/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 66 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPS_KR_K1_ZMMM512B32_IMM8: Code = 3985 # type: ignore
+EVEX_VFPCLASSPS_KR_K1_ZMMM512B32_IMM8: int = 3985
 """
 ``VFPCLASSPS k2 {k1}, zmm2/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 66 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPD_KR_K1_XMMM128B64_IMM8: Code = 3986 # type: ignore
+EVEX_VFPCLASSPD_KR_K1_XMMM128B64_IMM8: int = 3986
 """
 ``VFPCLASSPD k2 {k1}, xmm2/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 66 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPD_KR_K1_YMMM256B64_IMM8: Code = 3987 # type: ignore
+EVEX_VFPCLASSPD_KR_K1_YMMM256B64_IMM8: int = 3987
 """
 ``VFPCLASSPD k2 {k1}, ymm2/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 66 /r ib``
 
 ``AVX512VL and AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSPD_KR_K1_ZMMM512B64_IMM8: Code = 3988 # type: ignore
+EVEX_VFPCLASSPD_KR_K1_ZMMM512B64_IMM8: int = 3988
 """
 ``VFPCLASSPD k2 {k1}, zmm2/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 66 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSSS_KR_K1_XMMM32_IMM8: Code = 3989 # type: ignore
+EVEX_VFPCLASSSS_KR_K1_XMMM32_IMM8: int = 3989
 """
 ``VFPCLASSSS k2 {k1}, xmm2/m32, imm8``
 
 ``EVEX.LIG.66.0F3A.W0 67 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-EVEX_VFPCLASSSD_KR_K1_XMMM64_IMM8: Code = 3990 # type: ignore
+EVEX_VFPCLASSSD_KR_K1_XMMM64_IMM8: int = 3990
 """
 ``VFPCLASSSD k2 {k1}, xmm2/m64, imm8``
 
 ``EVEX.LIG.66.0F3A.W1 67 /r ib``
 
 ``AVX512DQ``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPS_XMM_XMM_XMMM128_XMM: Code = 3991 # type: ignore
+VEX_VFMADDPS_XMM_XMM_XMMM128_XMM: int = 3991
 """
 ``VFMADDPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 68 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPS_YMM_YMM_YMMM256_YMM: Code = 3992 # type: ignore
+VEX_VFMADDPS_YMM_YMM_YMMM256_YMM: int = 3992
 """
 ``VFMADDPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 68 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPS_XMM_XMM_XMM_XMMM128: Code = 3993 # type: ignore
+VEX_VFMADDPS_XMM_XMM_XMM_XMMM128: int = 3993
 """
 ``VFMADDPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 68 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPS_YMM_YMM_YMM_YMMM256: Code = 3994 # type: ignore
+VEX_VFMADDPS_YMM_YMM_YMM_YMMM256: int = 3994
 """
 ``VFMADDPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 68 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPD_XMM_XMM_XMMM128_XMM: Code = 3995 # type: ignore
+VEX_VFMADDPD_XMM_XMM_XMMM128_XMM: int = 3995
 """
 ``VFMADDPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 69 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPD_YMM_YMM_YMMM256_YMM: Code = 3996 # type: ignore
+VEX_VFMADDPD_YMM_YMM_YMMM256_YMM: int = 3996
 """
 ``VFMADDPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 69 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPD_XMM_XMM_XMM_XMMM128: Code = 3997 # type: ignore
+VEX_VFMADDPD_XMM_XMM_XMM_XMMM128: int = 3997
 """
 ``VFMADDPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 69 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDPD_YMM_YMM_YMM_YMMM256: Code = 3998 # type: ignore
+VEX_VFMADDPD_YMM_YMM_YMM_YMMM256: int = 3998
 """
 ``VFMADDPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 69 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSS_XMM_XMM_XMMM32_XMM: Code = 3999 # type: ignore
+VEX_VFMADDSS_XMM_XMM_XMMM32_XMM: int = 3999
 """
 ``VFMADDSS xmm1, xmm2, xmm3/m32, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 6A /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSS_XMM_XMM_XMM_XMMM32: Code = 4000 # type: ignore
+VEX_VFMADDSS_XMM_XMM_XMM_XMMM32: int = 4000
 """
 ``VFMADDSS xmm1, xmm2, xmm3, xmm4/m32``
 
 ``VEX.LIG.66.0F3A.W1 6A /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSD_XMM_XMM_XMMM64_XMM: Code = 4001 # type: ignore
+VEX_VFMADDSD_XMM_XMM_XMMM64_XMM: int = 4001
 """
 ``VFMADDSD xmm1, xmm2, xmm3/m64, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 6B /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMADDSD_XMM_XMM_XMM_XMMM64: Code = 4002 # type: ignore
+VEX_VFMADDSD_XMM_XMM_XMM_XMMM64: int = 4002
 """
 ``VFMADDSD xmm1, xmm2, xmm3, xmm4/m64``
 
 ``VEX.LIG.66.0F3A.W1 6B /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPS_XMM_XMM_XMMM128_XMM: Code = 4003 # type: ignore
+VEX_VFMSUBPS_XMM_XMM_XMMM128_XMM: int = 4003
 """
 ``VFMSUBPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 6C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPS_YMM_YMM_YMMM256_YMM: Code = 4004 # type: ignore
+VEX_VFMSUBPS_YMM_YMM_YMMM256_YMM: int = 4004
 """
 ``VFMSUBPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 6C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPS_XMM_XMM_XMM_XMMM128: Code = 4005 # type: ignore
+VEX_VFMSUBPS_XMM_XMM_XMM_XMMM128: int = 4005
 """
 ``VFMSUBPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 6C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPS_YMM_YMM_YMM_YMMM256: Code = 4006 # type: ignore
+VEX_VFMSUBPS_YMM_YMM_YMM_YMMM256: int = 4006
 """
 ``VFMSUBPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 6C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPD_XMM_XMM_XMMM128_XMM: Code = 4007 # type: ignore
+VEX_VFMSUBPD_XMM_XMM_XMMM128_XMM: int = 4007
 """
 ``VFMSUBPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 6D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPD_YMM_YMM_YMMM256_YMM: Code = 4008 # type: ignore
+VEX_VFMSUBPD_YMM_YMM_YMMM256_YMM: int = 4008
 """
 ``VFMSUBPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 6D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPD_XMM_XMM_XMM_XMMM128: Code = 4009 # type: ignore
+VEX_VFMSUBPD_XMM_XMM_XMM_XMMM128: int = 4009
 """
 ``VFMSUBPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 6D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBPD_YMM_YMM_YMM_YMMM256: Code = 4010 # type: ignore
+VEX_VFMSUBPD_YMM_YMM_YMM_YMMM256: int = 4010
 """
 ``VFMSUBPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 6D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBSS_XMM_XMM_XMMM32_XMM: Code = 4011 # type: ignore
+VEX_VFMSUBSS_XMM_XMM_XMMM32_XMM: int = 4011
 """
 ``VFMSUBSS xmm1, xmm2, xmm3/m32, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 6E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBSS_XMM_XMM_XMM_XMMM32: Code = 4012 # type: ignore
+VEX_VFMSUBSS_XMM_XMM_XMM_XMMM32: int = 4012
 """
 ``VFMSUBSS xmm1, xmm2, xmm3, xmm4/m32``
 
 ``VEX.LIG.66.0F3A.W1 6E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBSD_XMM_XMM_XMMM64_XMM: Code = 4013 # type: ignore
+VEX_VFMSUBSD_XMM_XMM_XMMM64_XMM: int = 4013
 """
 ``VFMSUBSD xmm1, xmm2, xmm3/m64, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 6F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFMSUBSD_XMM_XMM_XMM_XMMM64: Code = 4014 # type: ignore
+VEX_VFMSUBSD_XMM_XMM_XMM_XMMM64: int = 4014
 """
 ``VFMSUBSD xmm1, xmm2, xmm3, xmm4/m64``
 
 ``VEX.LIG.66.0F3A.W1 6F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDW_XMM_K1Z_XMM_XMMM128_IMM8: Code = 4015 # type: ignore
+EVEX_VPSHLDW_XMM_K1Z_XMM_XMMM128_IMM8: int = 4015
 """
 ``VPSHLDW xmm1 {k1}{z}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W1 70 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDW_YMM_K1Z_YMM_YMMM256_IMM8: Code = 4016 # type: ignore
+EVEX_VPSHLDW_YMM_K1Z_YMM_YMMM256_IMM8: int = 4016
 """
 ``VPSHLDW ymm1 {k1}{z}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W1 70 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDW_ZMM_K1Z_ZMM_ZMMM512_IMM8: Code = 4017 # type: ignore
+EVEX_VPSHLDW_ZMM_K1Z_ZMM_ZMMM512_IMM8: int = 4017
 """
 ``VPSHLDW zmm1 {k1}{z}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W1 70 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDD_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 4018 # type: ignore
+EVEX_VPSHLDD_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 4018
 """
 ``VPSHLDD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 71 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDD_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 4019 # type: ignore
+EVEX_VPSHLDD_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 4019
 """
 ``VPSHLDD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 71 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 4020 # type: ignore
+EVEX_VPSHLDD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 4020
 """
 ``VPSHLDD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 71 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDQ_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 4021 # type: ignore
+EVEX_VPSHLDQ_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 4021
 """
 ``VPSHLDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 71 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDQ_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 4022 # type: ignore
+EVEX_VPSHLDQ_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 4022
 """
 ``VPSHLDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 71 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHLDQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 4023 # type: ignore
+EVEX_VPSHLDQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 4023
 """
 ``VPSHLDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 71 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDW_XMM_K1Z_XMM_XMMM128_IMM8: Code = 4024 # type: ignore
+EVEX_VPSHRDW_XMM_K1Z_XMM_XMMM128_IMM8: int = 4024
 """
 ``VPSHRDW xmm1 {k1}{z}, xmm2, xmm3/m128, imm8``
 
 ``EVEX.128.66.0F3A.W1 72 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDW_YMM_K1Z_YMM_YMMM256_IMM8: Code = 4025 # type: ignore
+EVEX_VPSHRDW_YMM_K1Z_YMM_YMMM256_IMM8: int = 4025
 """
 ``VPSHRDW ymm1 {k1}{z}, ymm2, ymm3/m256, imm8``
 
 ``EVEX.256.66.0F3A.W1 72 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDW_ZMM_K1Z_ZMM_ZMMM512_IMM8: Code = 4026 # type: ignore
+EVEX_VPSHRDW_ZMM_K1Z_ZMM_ZMMM512_IMM8: int = 4026
 """
 ``VPSHRDW zmm1 {k1}{z}, zmm2, zmm3/m512, imm8``
 
 ``EVEX.512.66.0F3A.W1 72 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDD_XMM_K1Z_XMM_XMMM128B32_IMM8: Code = 4027 # type: ignore
+EVEX_VPSHRDD_XMM_K1Z_XMM_XMMM128B32_IMM8: int = 4027
 """
 ``VPSHRDD xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst, imm8``
 
 ``EVEX.128.66.0F3A.W0 73 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDD_YMM_K1Z_YMM_YMMM256B32_IMM8: Code = 4028 # type: ignore
+EVEX_VPSHRDD_YMM_K1Z_YMM_YMMM256B32_IMM8: int = 4028
 """
 ``VPSHRDD ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst, imm8``
 
 ``EVEX.256.66.0F3A.W0 73 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: Code = 4029 # type: ignore
+EVEX_VPSHRDD_ZMM_K1Z_ZMM_ZMMM512B32_IMM8: int = 4029
 """
 ``VPSHRDD zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst, imm8``
 
 ``EVEX.512.66.0F3A.W0 73 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDQ_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 4030 # type: ignore
+EVEX_VPSHRDQ_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 4030
 """
 ``VPSHRDQ xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 73 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDQ_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 4031 # type: ignore
+EVEX_VPSHRDQ_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 4031
 """
 ``VPSHRDQ ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 73 /r ib``
 
 ``AVX512VL and AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-EVEX_VPSHRDQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 4032 # type: ignore
+EVEX_VPSHRDQ_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 4032
 """
 ``VPSHRDQ zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 73 /r ib``
 
 ``AVX512_VBMI2``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPS_XMM_XMM_XMMM128_XMM: Code = 4033 # type: ignore
+VEX_VFNMADDPS_XMM_XMM_XMMM128_XMM: int = 4033
 """
 ``VFNMADDPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 78 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPS_YMM_YMM_YMMM256_YMM: Code = 4034 # type: ignore
+VEX_VFNMADDPS_YMM_YMM_YMMM256_YMM: int = 4034
 """
 ``VFNMADDPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 78 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPS_XMM_XMM_XMM_XMMM128: Code = 4035 # type: ignore
+VEX_VFNMADDPS_XMM_XMM_XMM_XMMM128: int = 4035
 """
 ``VFNMADDPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 78 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPS_YMM_YMM_YMM_YMMM256: Code = 4036 # type: ignore
+VEX_VFNMADDPS_YMM_YMM_YMM_YMMM256: int = 4036
 """
 ``VFNMADDPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 78 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPD_XMM_XMM_XMMM128_XMM: Code = 4037 # type: ignore
+VEX_VFNMADDPD_XMM_XMM_XMMM128_XMM: int = 4037
 """
 ``VFNMADDPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 79 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPD_YMM_YMM_YMMM256_YMM: Code = 4038 # type: ignore
+VEX_VFNMADDPD_YMM_YMM_YMMM256_YMM: int = 4038
 """
 ``VFNMADDPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 79 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPD_XMM_XMM_XMM_XMMM128: Code = 4039 # type: ignore
+VEX_VFNMADDPD_XMM_XMM_XMM_XMMM128: int = 4039
 """
 ``VFNMADDPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 79 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDPD_YMM_YMM_YMM_YMMM256: Code = 4040 # type: ignore
+VEX_VFNMADDPD_YMM_YMM_YMM_YMMM256: int = 4040
 """
 ``VFNMADDPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 79 /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDSS_XMM_XMM_XMMM32_XMM: Code = 4041 # type: ignore
+VEX_VFNMADDSS_XMM_XMM_XMMM32_XMM: int = 4041
 """
 ``VFNMADDSS xmm1, xmm2, xmm3/m32, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 7A /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDSS_XMM_XMM_XMM_XMMM32: Code = 4042 # type: ignore
+VEX_VFNMADDSS_XMM_XMM_XMM_XMMM32: int = 4042
 """
 ``VFNMADDSS xmm1, xmm2, xmm3, xmm4/m32``
 
 ``VEX.LIG.66.0F3A.W1 7A /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDSD_XMM_XMM_XMMM64_XMM: Code = 4043 # type: ignore
+VEX_VFNMADDSD_XMM_XMM_XMMM64_XMM: int = 4043
 """
 ``VFNMADDSD xmm1, xmm2, xmm3/m64, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 7B /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMADDSD_XMM_XMM_XMM_XMMM64: Code = 4044 # type: ignore
+VEX_VFNMADDSD_XMM_XMM_XMM_XMMM64: int = 4044
 """
 ``VFNMADDSD xmm1, xmm2, xmm3, xmm4/m64``
 
 ``VEX.LIG.66.0F3A.W1 7B /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPS_XMM_XMM_XMMM128_XMM: Code = 4045 # type: ignore
+VEX_VFNMSUBPS_XMM_XMM_XMMM128_XMM: int = 4045
 """
 ``VFNMSUBPS xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 7C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPS_YMM_YMM_YMMM256_YMM: Code = 4046 # type: ignore
+VEX_VFNMSUBPS_YMM_YMM_YMMM256_YMM: int = 4046
 """
 ``VFNMSUBPS ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 7C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPS_XMM_XMM_XMM_XMMM128: Code = 4047 # type: ignore
+VEX_VFNMSUBPS_XMM_XMM_XMM_XMMM128: int = 4047
 """
 ``VFNMSUBPS xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 7C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPS_YMM_YMM_YMM_YMMM256: Code = 4048 # type: ignore
+VEX_VFNMSUBPS_YMM_YMM_YMM_YMMM256: int = 4048
 """
 ``VFNMSUBPS ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 7C /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPD_XMM_XMM_XMMM128_XMM: Code = 4049 # type: ignore
+VEX_VFNMSUBPD_XMM_XMM_XMMM128_XMM: int = 4049
 """
 ``VFNMSUBPD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``VEX.128.66.0F3A.W0 7D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPD_YMM_YMM_YMMM256_YMM: Code = 4050 # type: ignore
+VEX_VFNMSUBPD_YMM_YMM_YMMM256_YMM: int = 4050
 """
 ``VFNMSUBPD ymm1, ymm2, ymm3/m256, ymm4``
 
 ``VEX.256.66.0F3A.W0 7D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPD_XMM_XMM_XMM_XMMM128: Code = 4051 # type: ignore
+VEX_VFNMSUBPD_XMM_XMM_XMM_XMMM128: int = 4051
 """
 ``VFNMSUBPD xmm1, xmm2, xmm3, xmm4/m128``
 
 ``VEX.128.66.0F3A.W1 7D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBPD_YMM_YMM_YMM_YMMM256: Code = 4052 # type: ignore
+VEX_VFNMSUBPD_YMM_YMM_YMM_YMMM256: int = 4052
 """
 ``VFNMSUBPD ymm1, ymm2, ymm3, ymm4/m256``
 
 ``VEX.256.66.0F3A.W1 7D /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBSS_XMM_XMM_XMMM32_XMM: Code = 4053 # type: ignore
+VEX_VFNMSUBSS_XMM_XMM_XMMM32_XMM: int = 4053
 """
 ``VFNMSUBSS xmm1, xmm2, xmm3/m32, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 7E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBSS_XMM_XMM_XMM_XMMM32: Code = 4054 # type: ignore
+VEX_VFNMSUBSS_XMM_XMM_XMM_XMMM32: int = 4054
 """
 ``VFNMSUBSS xmm1, xmm2, xmm3, xmm4/m32``
 
 ``VEX.LIG.66.0F3A.W1 7E /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBSD_XMM_XMM_XMMM64_XMM: Code = 4055 # type: ignore
+VEX_VFNMSUBSD_XMM_XMM_XMMM64_XMM: int = 4055
 """
 ``VFNMSUBSD xmm1, xmm2, xmm3/m64, xmm4``
 
 ``VEX.LIG.66.0F3A.W0 7F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-VEX_VFNMSUBSD_XMM_XMM_XMM_XMMM64: Code = 4056 # type: ignore
+VEX_VFNMSUBSD_XMM_XMM_XMM_XMMM64: int = 4056
 """
 ``VFNMSUBSD xmm1, xmm2, xmm3, xmm4/m64``
 
 ``VEX.LIG.66.0F3A.W1 7F /r /is4``
 
 ``FMA4``
 
 ``16/32/64-bit``
 """
-SHA1RNDS4_XMM_XMMM128_IMM8: Code = 4057 # type: ignore
+SHA1RNDS4_XMM_XMMM128_IMM8: int = 4057
 """
 ``SHA1RNDS4 xmm1, xmm2/m128, imm8``
 
 ``NP 0F 3A CC /r ib``
 
 ``SHA``
 
 ``16/32/64-bit``
 """
-GF2P8AFFINEQB_XMM_XMMM128_IMM8: Code = 4058 # type: ignore
+GF2P8AFFINEQB_XMM_XMMM128_IMM8: int = 4058
 """
 ``GF2P8AFFINEQB xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A CE /r ib``
 
 ``GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8AFFINEQB_XMM_XMM_XMMM128_IMM8: Code = 4059 # type: ignore
+VEX_VGF2P8AFFINEQB_XMM_XMM_XMMM128_IMM8: int = 4059
 """
 ``VGF2P8AFFINEQB xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.W1 CE /r ib``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8AFFINEQB_YMM_YMM_YMMM256_IMM8: Code = 4060 # type: ignore
+VEX_VGF2P8AFFINEQB_YMM_YMM_YMMM256_IMM8: int = 4060
 """
 ``VGF2P8AFFINEQB ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.W1 CE /r ib``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEQB_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 4061 # type: ignore
+EVEX_VGF2P8AFFINEQB_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 4061
 """
 ``VGF2P8AFFINEQB xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 CE /r ib``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEQB_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 4062 # type: ignore
+EVEX_VGF2P8AFFINEQB_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 4062
 """
 ``VGF2P8AFFINEQB ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 CE /r ib``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEQB_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 4063 # type: ignore
+EVEX_VGF2P8AFFINEQB_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 4063
 """
 ``VGF2P8AFFINEQB zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 CE /r ib``
 
 ``AVX512F and GFNI``
 
 ``16/32/64-bit``
 """
-GF2P8AFFINEINVQB_XMM_XMMM128_IMM8: Code = 4064 # type: ignore
+GF2P8AFFINEINVQB_XMM_XMMM128_IMM8: int = 4064
 """
 ``GF2P8AFFINEINVQB xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A CF /r ib``
 
 ``GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8AFFINEINVQB_XMM_XMM_XMMM128_IMM8: Code = 4065 # type: ignore
+VEX_VGF2P8AFFINEINVQB_XMM_XMM_XMMM128_IMM8: int = 4065
 """
 ``VGF2P8AFFINEINVQB xmm1, xmm2, xmm3/m128, imm8``
 
 ``VEX.128.66.0F3A.W1 CF /r ib``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-VEX_VGF2P8AFFINEINVQB_YMM_YMM_YMMM256_IMM8: Code = 4066 # type: ignore
+VEX_VGF2P8AFFINEINVQB_YMM_YMM_YMMM256_IMM8: int = 4066
 """
 ``VGF2P8AFFINEINVQB ymm1, ymm2, ymm3/m256, imm8``
 
 ``VEX.256.66.0F3A.W1 CF /r ib``
 
 ``AVX and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEINVQB_XMM_K1Z_XMM_XMMM128B64_IMM8: Code = 4067 # type: ignore
+EVEX_VGF2P8AFFINEINVQB_XMM_K1Z_XMM_XMMM128B64_IMM8: int = 4067
 """
 ``VGF2P8AFFINEINVQB xmm1 {k1}{z}, xmm2, xmm3/m128/m64bcst, imm8``
 
 ``EVEX.128.66.0F3A.W1 CF /r ib``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEINVQB_YMM_K1Z_YMM_YMMM256B64_IMM8: Code = 4068 # type: ignore
+EVEX_VGF2P8AFFINEINVQB_YMM_K1Z_YMM_YMMM256B64_IMM8: int = 4068
 """
 ``VGF2P8AFFINEINVQB ymm1 {k1}{z}, ymm2, ymm3/m256/m64bcst, imm8``
 
 ``EVEX.256.66.0F3A.W1 CF /r ib``
 
 ``AVX512VL and GFNI``
 
 ``16/32/64-bit``
 """
-EVEX_VGF2P8AFFINEINVQB_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: Code = 4069 # type: ignore
+EVEX_VGF2P8AFFINEINVQB_ZMM_K1Z_ZMM_ZMMM512B64_IMM8: int = 4069
 """
 ``VGF2P8AFFINEINVQB zmm1 {k1}{z}, zmm2, zmm3/m512/m64bcst, imm8``
 
 ``EVEX.512.66.0F3A.W1 CF /r ib``
 
 ``AVX512F and GFNI``
 
 ``16/32/64-bit``
 """
-AESKEYGENASSIST_XMM_XMMM128_IMM8: Code = 4070 # type: ignore
+AESKEYGENASSIST_XMM_XMMM128_IMM8: int = 4070
 """
 ``AESKEYGENASSIST xmm1, xmm2/m128, imm8``
 
 ``66 0F 3A DF /r ib``
 
 ``AES``
 
 ``16/32/64-bit``
 """
-VEX_VAESKEYGENASSIST_XMM_XMMM128_IMM8: Code = 4071 # type: ignore
+VEX_VAESKEYGENASSIST_XMM_XMMM128_IMM8: int = 4071
 """
 ``VAESKEYGENASSIST xmm1, xmm2/m128, imm8``
 
 ``VEX.128.66.0F3A.WIG DF /r ib``
 
 ``AES and AVX``
 
 ``16/32/64-bit``
 """
-VEX_RORX_R32_RM32_IMM8: Code = 4072 # type: ignore
+VEX_RORX_R32_RM32_IMM8: int = 4072
 """
 ``RORX r32, r/m32, imm8``
 
 ``VEX.LZ.F2.0F3A.W0 F0 /r ib``
 
 ``BMI2``
 
 ``16/32/64-bit``
 """
-VEX_RORX_R64_RM64_IMM8: Code = 4073 # type: ignore
+VEX_RORX_R64_RM64_IMM8: int = 4073
 """
 ``RORX r64, r/m64, imm8``
 
 ``VEX.LZ.F2.0F3A.W1 F0 /r ib``
 
 ``BMI2``
 
 ``64-bit``
 """
-XOP_VPMACSSWW_XMM_XMM_XMMM128_XMM: Code = 4074 # type: ignore
+XOP_VPMACSSWW_XMM_XMM_XMMM128_XMM: int = 4074
 """
 ``VPMACSSWW xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 85 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSSWD_XMM_XMM_XMMM128_XMM: Code = 4075 # type: ignore
+XOP_VPMACSSWD_XMM_XMM_XMMM128_XMM: int = 4075
 """
 ``VPMACSSWD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 86 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSSDQL_XMM_XMM_XMMM128_XMM: Code = 4076 # type: ignore
+XOP_VPMACSSDQL_XMM_XMM_XMMM128_XMM: int = 4076
 """
 ``VPMACSSDQL xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 87 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSSDD_XMM_XMM_XMMM128_XMM: Code = 4077 # type: ignore
+XOP_VPMACSSDD_XMM_XMM_XMMM128_XMM: int = 4077
 """
 ``VPMACSSDD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 8E /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSSDQH_XMM_XMM_XMMM128_XMM: Code = 4078 # type: ignore
+XOP_VPMACSSDQH_XMM_XMM_XMMM128_XMM: int = 4078
 """
 ``VPMACSSDQH xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 8F /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSWW_XMM_XMM_XMMM128_XMM: Code = 4079 # type: ignore
+XOP_VPMACSWW_XMM_XMM_XMMM128_XMM: int = 4079
 """
 ``VPMACSWW xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 95 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSWD_XMM_XMM_XMMM128_XMM: Code = 4080 # type: ignore
+XOP_VPMACSWD_XMM_XMM_XMMM128_XMM: int = 4080
 """
 ``VPMACSWD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 96 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSDQL_XMM_XMM_XMMM128_XMM: Code = 4081 # type: ignore
+XOP_VPMACSDQL_XMM_XMM_XMMM128_XMM: int = 4081
 """
 ``VPMACSDQL xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 97 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSDD_XMM_XMM_XMMM128_XMM: Code = 4082 # type: ignore
+XOP_VPMACSDD_XMM_XMM_XMMM128_XMM: int = 4082
 """
 ``VPMACSDD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 9E /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMACSDQH_XMM_XMM_XMMM128_XMM: Code = 4083 # type: ignore
+XOP_VPMACSDQH_XMM_XMM_XMMM128_XMM: int = 4083
 """
 ``VPMACSDQH xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 9F /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCMOV_XMM_XMM_XMMM128_XMM: Code = 4084 # type: ignore
+XOP_VPCMOV_XMM_XMM_XMMM128_XMM: int = 4084
 """
 ``VPCMOV xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 A2 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCMOV_YMM_YMM_YMMM256_YMM: Code = 4085 # type: ignore
+XOP_VPCMOV_YMM_YMM_YMMM256_YMM: int = 4085
 """
 ``VPCMOV ymm1, ymm2, ymm3/m256, ymm4``
 
 ``XOP.256.X8.W0 A2 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCMOV_XMM_XMM_XMM_XMMM128: Code = 4086 # type: ignore
+XOP_VPCMOV_XMM_XMM_XMM_XMMM128: int = 4086
 """
 ``VPCMOV xmm1, xmm2, xmm3, xmm4/m128``
 
 ``XOP.128.X8.W1 A2 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCMOV_YMM_YMM_YMM_YMMM256: Code = 4087 # type: ignore
+XOP_VPCMOV_YMM_YMM_YMM_YMMM256: int = 4087
 """
 ``VPCMOV ymm1, ymm2, ymm3, ymm4/m256``
 
 ``XOP.256.X8.W1 A2 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPPERM_XMM_XMM_XMMM128_XMM: Code = 4088 # type: ignore
+XOP_VPPERM_XMM_XMM_XMMM128_XMM: int = 4088
 """
 ``VPPERM xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 A3 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPPERM_XMM_XMM_XMM_XMMM128: Code = 4089 # type: ignore
+XOP_VPPERM_XMM_XMM_XMM_XMMM128: int = 4089
 """
 ``VPPERM xmm1, xmm2, xmm3, xmm4/m128``
 
 ``XOP.128.X8.W1 A3 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMADCSSWD_XMM_XMM_XMMM128_XMM: Code = 4090 # type: ignore
+XOP_VPMADCSSWD_XMM_XMM_XMMM128_XMM: int = 4090
 """
 ``VPMADCSSWD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 A6 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPMADCSWD_XMM_XMM_XMMM128_XMM: Code = 4091 # type: ignore
+XOP_VPMADCSWD_XMM_XMM_XMMM128_XMM: int = 4091
 """
 ``VPMADCSWD xmm1, xmm2, xmm3/m128, xmm4``
 
 ``XOP.128.X8.W0 B6 /r /is4``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTB_XMM_XMMM128_IMM8: Code = 4092 # type: ignore
+XOP_VPROTB_XMM_XMMM128_IMM8: int = 4092
 """
 ``VPROTB xmm1, xmm2/m128, imm8``
 
 ``XOP.128.X8.W0 C0 /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTW_XMM_XMMM128_IMM8: Code = 4093 # type: ignore
+XOP_VPROTW_XMM_XMMM128_IMM8: int = 4093
 """
 ``VPROTW xmm1, xmm2/m128, imm8``
 
 ``XOP.128.X8.W0 C1 /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTD_XMM_XMMM128_IMM8: Code = 4094 # type: ignore
+XOP_VPROTD_XMM_XMMM128_IMM8: int = 4094
 """
 ``VPROTD xmm1, xmm2/m128, imm8``
 
 ``XOP.128.X8.W0 C2 /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTQ_XMM_XMMM128_IMM8: Code = 4095 # type: ignore
+XOP_VPROTQ_XMM_XMMM128_IMM8: int = 4095
 """
 ``VPROTQ xmm1, xmm2/m128, imm8``
 
 ``XOP.128.X8.W0 C3 /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMB_XMM_XMM_XMMM128_IMM8: Code = 4096 # type: ignore
+XOP_VPCOMB_XMM_XMM_XMMM128_IMM8: int = 4096
 """
 ``VPCOMB xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 CC /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMW_XMM_XMM_XMMM128_IMM8: Code = 4097 # type: ignore
+XOP_VPCOMW_XMM_XMM_XMMM128_IMM8: int = 4097
 """
 ``VPCOMW xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 CD /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMD_XMM_XMM_XMMM128_IMM8: Code = 4098 # type: ignore
+XOP_VPCOMD_XMM_XMM_XMMM128_IMM8: int = 4098
 """
 ``VPCOMD xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 CE /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMQ_XMM_XMM_XMMM128_IMM8: Code = 4099 # type: ignore
+XOP_VPCOMQ_XMM_XMM_XMMM128_IMM8: int = 4099
 """
 ``VPCOMQ xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 CF /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMUB_XMM_XMM_XMMM128_IMM8: Code = 4100 # type: ignore
+XOP_VPCOMUB_XMM_XMM_XMMM128_IMM8: int = 4100
 """
 ``VPCOMUB xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 EC /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMUW_XMM_XMM_XMMM128_IMM8: Code = 4101 # type: ignore
+XOP_VPCOMUW_XMM_XMM_XMMM128_IMM8: int = 4101
 """
 ``VPCOMUW xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 ED /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMUD_XMM_XMM_XMMM128_IMM8: Code = 4102 # type: ignore
+XOP_VPCOMUD_XMM_XMM_XMMM128_IMM8: int = 4102
 """
 ``VPCOMUD xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 EE /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPCOMUQ_XMM_XMM_XMMM128_IMM8: Code = 4103 # type: ignore
+XOP_VPCOMUQ_XMM_XMM_XMMM128_IMM8: int = 4103
 """
 ``VPCOMUQ xmm1, xmm2, xmm3/m128, imm8``
 
 ``XOP.128.X8.W0 EF /r ib``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_BLCFILL_R32_RM32: Code = 4104 # type: ignore
+XOP_BLCFILL_R32_RM32: int = 4104
 """
 ``BLCFILL r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /1``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLCFILL_R64_RM64: Code = 4105 # type: ignore
+XOP_BLCFILL_R64_RM64: int = 4105
 """
 ``BLCFILL r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /1``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLSFILL_R32_RM32: Code = 4106 # type: ignore
+XOP_BLSFILL_R32_RM32: int = 4106
 """
 ``BLSFILL r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /2``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLSFILL_R64_RM64: Code = 4107 # type: ignore
+XOP_BLSFILL_R64_RM64: int = 4107
 """
 ``BLSFILL r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /2``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLCS_R32_RM32: Code = 4108 # type: ignore
+XOP_BLCS_R32_RM32: int = 4108
 """
 ``BLCS r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /3``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLCS_R64_RM64: Code = 4109 # type: ignore
+XOP_BLCS_R64_RM64: int = 4109
 """
 ``BLCS r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /3``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_TZMSK_R32_RM32: Code = 4110 # type: ignore
+XOP_TZMSK_R32_RM32: int = 4110
 """
 ``TZMSK r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /4``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_TZMSK_R64_RM64: Code = 4111 # type: ignore
+XOP_TZMSK_R64_RM64: int = 4111
 """
 ``TZMSK r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /4``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLCIC_R32_RM32: Code = 4112 # type: ignore
+XOP_BLCIC_R32_RM32: int = 4112
 """
 ``BLCIC r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /5``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLCIC_R64_RM64: Code = 4113 # type: ignore
+XOP_BLCIC_R64_RM64: int = 4113
 """
 ``BLCIC r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /5``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLSIC_R32_RM32: Code = 4114 # type: ignore
+XOP_BLSIC_R32_RM32: int = 4114
 """
 ``BLSIC r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /6``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLSIC_R64_RM64: Code = 4115 # type: ignore
+XOP_BLSIC_R64_RM64: int = 4115
 """
 ``BLSIC r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /6``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_T1MSKC_R32_RM32: Code = 4116 # type: ignore
+XOP_T1MSKC_R32_RM32: int = 4116
 """
 ``T1MSKC r32, r/m32``
 
 ``XOP.L0.X9.W0 01 /7``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_T1MSKC_R64_RM64: Code = 4117 # type: ignore
+XOP_T1MSKC_R64_RM64: int = 4117
 """
 ``T1MSKC r64, r/m64``
 
 ``XOP.L0.X9.W1 01 /7``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLCMSK_R32_RM32: Code = 4118 # type: ignore
+XOP_BLCMSK_R32_RM32: int = 4118
 """
 ``BLCMSK r32, r/m32``
 
 ``XOP.L0.X9.W0 02 /1``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLCMSK_R64_RM64: Code = 4119 # type: ignore
+XOP_BLCMSK_R64_RM64: int = 4119
 """
 ``BLCMSK r64, r/m64``
 
 ``XOP.L0.X9.W1 02 /1``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_BLCI_R32_RM32: Code = 4120 # type: ignore
+XOP_BLCI_R32_RM32: int = 4120
 """
 ``BLCI r32, r/m32``
 
 ``XOP.L0.X9.W0 02 /6``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BLCI_R64_RM64: Code = 4121 # type: ignore
+XOP_BLCI_R64_RM64: int = 4121
 """
 ``BLCI r64, r/m64``
 
 ``XOP.L0.X9.W1 02 /6``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_LLWPCB_R32: Code = 4122 # type: ignore
+XOP_LLWPCB_R32: int = 4122
 """
 ``LLWPCB r32``
 
 ``XOP.L0.X9.W0 12 /0``
 
 ``LWP``
 
 ``16/32/64-bit``
 """
-XOP_LLWPCB_R64: Code = 4123 # type: ignore
+XOP_LLWPCB_R64: int = 4123
 """
 ``LLWPCB r64``
 
 ``XOP.L0.X9.W1 12 /0``
 
 ``LWP``
 
 ``64-bit``
 """
-XOP_SLWPCB_R32: Code = 4124 # type: ignore
+XOP_SLWPCB_R32: int = 4124
 """
 ``SLWPCB r32``
 
 ``XOP.L0.X9.W0 12 /1``
 
 ``LWP``
 
 ``16/32/64-bit``
 """
-XOP_SLWPCB_R64: Code = 4125 # type: ignore
+XOP_SLWPCB_R64: int = 4125
 """
 ``SLWPCB r64``
 
 ``XOP.L0.X9.W1 12 /1``
 
 ``LWP``
 
 ``64-bit``
 """
-XOP_VFRCZPS_XMM_XMMM128: Code = 4126 # type: ignore
+XOP_VFRCZPS_XMM_XMMM128: int = 4126
 """
 ``VFRCZPS xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 80 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VFRCZPS_YMM_YMMM256: Code = 4127 # type: ignore
+XOP_VFRCZPS_YMM_YMMM256: int = 4127
 """
 ``VFRCZPS ymm1, ymm2/m256``
 
 ``XOP.256.X9.W0 80 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VFRCZPD_XMM_XMMM128: Code = 4128 # type: ignore
+XOP_VFRCZPD_XMM_XMMM128: int = 4128
 """
 ``VFRCZPD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 81 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VFRCZPD_YMM_YMMM256: Code = 4129 # type: ignore
+XOP_VFRCZPD_YMM_YMMM256: int = 4129
 """
 ``VFRCZPD ymm1, ymm2/m256``
 
 ``XOP.256.X9.W0 81 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VFRCZSS_XMM_XMMM32: Code = 4130 # type: ignore
+XOP_VFRCZSS_XMM_XMMM32: int = 4130
 """
 ``VFRCZSS xmm1, xmm2/m32``
 
 ``XOP.128.X9.W0 82 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VFRCZSD_XMM_XMMM64: Code = 4131 # type: ignore
+XOP_VFRCZSD_XMM_XMMM64: int = 4131
 """
 ``VFRCZSD xmm1, xmm2/m64``
 
 ``XOP.128.X9.W0 83 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTB_XMM_XMMM128_XMM: Code = 4132 # type: ignore
+XOP_VPROTB_XMM_XMMM128_XMM: int = 4132
 """
 ``VPROTB xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 90 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTB_XMM_XMM_XMMM128: Code = 4133 # type: ignore
+XOP_VPROTB_XMM_XMM_XMMM128: int = 4133
 """
 ``VPROTB xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 90 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTW_XMM_XMMM128_XMM: Code = 4134 # type: ignore
+XOP_VPROTW_XMM_XMMM128_XMM: int = 4134
 """
 ``VPROTW xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 91 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTW_XMM_XMM_XMMM128: Code = 4135 # type: ignore
+XOP_VPROTW_XMM_XMM_XMMM128: int = 4135
 """
 ``VPROTW xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 91 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTD_XMM_XMMM128_XMM: Code = 4136 # type: ignore
+XOP_VPROTD_XMM_XMMM128_XMM: int = 4136
 """
 ``VPROTD xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 92 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTD_XMM_XMM_XMMM128: Code = 4137 # type: ignore
+XOP_VPROTD_XMM_XMM_XMMM128: int = 4137
 """
 ``VPROTD xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 92 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTQ_XMM_XMMM128_XMM: Code = 4138 # type: ignore
+XOP_VPROTQ_XMM_XMMM128_XMM: int = 4138
 """
 ``VPROTQ xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 93 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPROTQ_XMM_XMM_XMMM128: Code = 4139 # type: ignore
+XOP_VPROTQ_XMM_XMM_XMMM128: int = 4139
 """
 ``VPROTQ xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 93 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLB_XMM_XMMM128_XMM: Code = 4140 # type: ignore
+XOP_VPSHLB_XMM_XMMM128_XMM: int = 4140
 """
 ``VPSHLB xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 94 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLB_XMM_XMM_XMMM128: Code = 4141 # type: ignore
+XOP_VPSHLB_XMM_XMM_XMMM128: int = 4141
 """
 ``VPSHLB xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 94 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLW_XMM_XMMM128_XMM: Code = 4142 # type: ignore
+XOP_VPSHLW_XMM_XMMM128_XMM: int = 4142
 """
 ``VPSHLW xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 95 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLW_XMM_XMM_XMMM128: Code = 4143 # type: ignore
+XOP_VPSHLW_XMM_XMM_XMMM128: int = 4143
 """
 ``VPSHLW xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 95 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLD_XMM_XMMM128_XMM: Code = 4144 # type: ignore
+XOP_VPSHLD_XMM_XMMM128_XMM: int = 4144
 """
 ``VPSHLD xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 96 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLD_XMM_XMM_XMMM128: Code = 4145 # type: ignore
+XOP_VPSHLD_XMM_XMM_XMMM128: int = 4145
 """
 ``VPSHLD xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 96 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLQ_XMM_XMMM128_XMM: Code = 4146 # type: ignore
+XOP_VPSHLQ_XMM_XMMM128_XMM: int = 4146
 """
 ``VPSHLQ xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 97 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHLQ_XMM_XMM_XMMM128: Code = 4147 # type: ignore
+XOP_VPSHLQ_XMM_XMM_XMMM128: int = 4147
 """
 ``VPSHLQ xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 97 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAB_XMM_XMMM128_XMM: Code = 4148 # type: ignore
+XOP_VPSHAB_XMM_XMMM128_XMM: int = 4148
 """
 ``VPSHAB xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 98 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAB_XMM_XMM_XMMM128: Code = 4149 # type: ignore
+XOP_VPSHAB_XMM_XMM_XMMM128: int = 4149
 """
 ``VPSHAB xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 98 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAW_XMM_XMMM128_XMM: Code = 4150 # type: ignore
+XOP_VPSHAW_XMM_XMMM128_XMM: int = 4150
 """
 ``VPSHAW xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 99 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAW_XMM_XMM_XMMM128: Code = 4151 # type: ignore
+XOP_VPSHAW_XMM_XMM_XMMM128: int = 4151
 """
 ``VPSHAW xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 99 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAD_XMM_XMMM128_XMM: Code = 4152 # type: ignore
+XOP_VPSHAD_XMM_XMMM128_XMM: int = 4152
 """
 ``VPSHAD xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 9A /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAD_XMM_XMM_XMMM128: Code = 4153 # type: ignore
+XOP_VPSHAD_XMM_XMM_XMMM128: int = 4153
 """
 ``VPSHAD xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 9A /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAQ_XMM_XMMM128_XMM: Code = 4154 # type: ignore
+XOP_VPSHAQ_XMM_XMMM128_XMM: int = 4154
 """
 ``VPSHAQ xmm1, xmm2/m128, xmm3``
 
 ``XOP.128.X9.W0 9B /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPSHAQ_XMM_XMM_XMMM128: Code = 4155 # type: ignore
+XOP_VPSHAQ_XMM_XMM_XMMM128: int = 4155
 """
 ``VPSHAQ xmm1, xmm2, xmm3/m128``
 
 ``XOP.128.X9.W1 9B /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDBW_XMM_XMMM128: Code = 4156 # type: ignore
+XOP_VPHADDBW_XMM_XMMM128: int = 4156
 """
 ``VPHADDBW xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 C1 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDBD_XMM_XMMM128: Code = 4157 # type: ignore
+XOP_VPHADDBD_XMM_XMMM128: int = 4157
 """
 ``VPHADDBD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 C2 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDBQ_XMM_XMMM128: Code = 4158 # type: ignore
+XOP_VPHADDBQ_XMM_XMMM128: int = 4158
 """
 ``VPHADDBQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 C3 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDWD_XMM_XMMM128: Code = 4159 # type: ignore
+XOP_VPHADDWD_XMM_XMMM128: int = 4159
 """
 ``VPHADDWD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 C6 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDWQ_XMM_XMMM128: Code = 4160 # type: ignore
+XOP_VPHADDWQ_XMM_XMMM128: int = 4160
 """
 ``VPHADDWQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 C7 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDDQ_XMM_XMMM128: Code = 4161 # type: ignore
+XOP_VPHADDDQ_XMM_XMMM128: int = 4161
 """
 ``VPHADDDQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 CB /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUBW_XMM_XMMM128: Code = 4162 # type: ignore
+XOP_VPHADDUBW_XMM_XMMM128: int = 4162
 """
 ``VPHADDUBW xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 D1 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUBD_XMM_XMMM128: Code = 4163 # type: ignore
+XOP_VPHADDUBD_XMM_XMMM128: int = 4163
 """
 ``VPHADDUBD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 D2 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUBQ_XMM_XMMM128: Code = 4164 # type: ignore
+XOP_VPHADDUBQ_XMM_XMMM128: int = 4164
 """
 ``VPHADDUBQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 D3 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUWD_XMM_XMMM128: Code = 4165 # type: ignore
+XOP_VPHADDUWD_XMM_XMMM128: int = 4165
 """
 ``VPHADDUWD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 D6 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUWQ_XMM_XMMM128: Code = 4166 # type: ignore
+XOP_VPHADDUWQ_XMM_XMMM128: int = 4166
 """
 ``VPHADDUWQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 D7 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHADDUDQ_XMM_XMMM128: Code = 4167 # type: ignore
+XOP_VPHADDUDQ_XMM_XMMM128: int = 4167
 """
 ``VPHADDUDQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 DB /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHSUBBW_XMM_XMMM128: Code = 4168 # type: ignore
+XOP_VPHSUBBW_XMM_XMMM128: int = 4168
 """
 ``VPHSUBBW xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 E1 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHSUBWD_XMM_XMMM128: Code = 4169 # type: ignore
+XOP_VPHSUBWD_XMM_XMMM128: int = 4169
 """
 ``VPHSUBWD xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 E2 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_VPHSUBDQ_XMM_XMMM128: Code = 4170 # type: ignore
+XOP_VPHSUBDQ_XMM_XMMM128: int = 4170
 """
 ``VPHSUBDQ xmm1, xmm2/m128``
 
 ``XOP.128.X9.W0 E3 /r``
 
 ``XOP``
 
 ``16/32/64-bit``
 """
-XOP_BEXTR_R32_RM32_IMM32: Code = 4171 # type: ignore
+XOP_BEXTR_R32_RM32_IMM32: int = 4171
 """
 ``BEXTR r32, r/m32, imm32``
 
 ``XOP.L0.XA.W0 10 /r id``
 
 ``TBM``
 
 ``16/32/64-bit``
 """
-XOP_BEXTR_R64_RM64_IMM32: Code = 4172 # type: ignore
+XOP_BEXTR_R64_RM64_IMM32: int = 4172
 """
 ``BEXTR r64, r/m64, imm32``
 
 ``XOP.L0.XA.W1 10 /r id``
 
 ``TBM``
 
 ``64-bit``
 """
-XOP_LWPINS_R32_RM32_IMM32: Code = 4173 # type: ignore
+XOP_LWPINS_R32_RM32_IMM32: int = 4173
 """
 ``LWPINS r32, r/m32, imm32``
 
 ``XOP.L0.XA.W0 12 /0 id``
 
 ``LWP``
 
 ``16/32/64-bit``
 """
-XOP_LWPINS_R64_RM32_IMM32: Code = 4174 # type: ignore
+XOP_LWPINS_R64_RM32_IMM32: int = 4174
 """
 ``LWPINS r64, r/m32, imm32``
 
 ``XOP.L0.XA.W1 12 /0 id``
 
 ``LWP``
 
 ``64-bit``
 """
-XOP_LWPVAL_R32_RM32_IMM32: Code = 4175 # type: ignore
+XOP_LWPVAL_R32_RM32_IMM32: int = 4175
 """
 ``LWPVAL r32, r/m32, imm32``
 
 ``XOP.L0.XA.W0 12 /1 id``
 
 ``LWP``
 
 ``16/32/64-bit``
 """
-XOP_LWPVAL_R64_RM32_IMM32: Code = 4176 # type: ignore
+XOP_LWPVAL_R64_RM32_IMM32: int = 4176
 """
 ``LWPVAL r64, r/m32, imm32``
 
 ``XOP.L0.XA.W1 12 /1 id``
 
 ``LWP``
 
 ``64-bit``
 """
-D3NOW_PI2FW_MM_MMM64: Code = 4177 # type: ignore
+D3NOW_PI2FW_MM_MMM64: int = 4177
 """
 ``PI2FW mm, mm/m64``
 
 ``0F 0F /r 0C``
 
 ``3DNOWEXT``
 
 ``16/32/64-bit``
 """
-D3NOW_PI2FD_MM_MMM64: Code = 4178 # type: ignore
+D3NOW_PI2FD_MM_MMM64: int = 4178
 """
 ``PI2FD mm, mm/m64``
 
 ``0F 0F /r 0D``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PF2IW_MM_MMM64: Code = 4179 # type: ignore
+D3NOW_PF2IW_MM_MMM64: int = 4179
 """
 ``PF2IW mm, mm/m64``
 
 ``0F 0F /r 1C``
 
 ``3DNOWEXT``
 
 ``16/32/64-bit``
 """
-D3NOW_PF2ID_MM_MMM64: Code = 4180 # type: ignore
+D3NOW_PF2ID_MM_MMM64: int = 4180
 """
 ``PF2ID mm, mm/m64``
 
 ``0F 0F /r 1D``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRCPV_MM_MMM64: Code = 4181 # type: ignore
+D3NOW_PFRCPV_MM_MMM64: int = 4181
 """
 ``PFRCPV mm, mm/m64``
 
 ``0F 0F /r 86``
 
 ``AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-D3NOW_PFRSQRTV_MM_MMM64: Code = 4182 # type: ignore
+D3NOW_PFRSQRTV_MM_MMM64: int = 4182
 """
 ``PFRSQRTV mm, mm/m64``
 
 ``0F 0F /r 87``
 
 ``AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-D3NOW_PFNACC_MM_MMM64: Code = 4183 # type: ignore
+D3NOW_PFNACC_MM_MMM64: int = 4183
 """
 ``PFNACC mm, mm/m64``
 
 ``0F 0F /r 8A``
 
 ``3DNOWEXT``
 
 ``16/32/64-bit``
 """
-D3NOW_PFPNACC_MM_MMM64: Code = 4184 # type: ignore
+D3NOW_PFPNACC_MM_MMM64: int = 4184
 """
 ``PFPNACC mm, mm/m64``
 
 ``0F 0F /r 8E``
 
 ``3DNOWEXT``
 
 ``16/32/64-bit``
 """
-D3NOW_PFCMPGE_MM_MMM64: Code = 4185 # type: ignore
+D3NOW_PFCMPGE_MM_MMM64: int = 4185
 """
 ``PFCMPGE mm, mm/m64``
 
 ``0F 0F /r 90``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFMIN_MM_MMM64: Code = 4186 # type: ignore
+D3NOW_PFMIN_MM_MMM64: int = 4186
 """
 ``PFMIN mm, mm/m64``
 
 ``0F 0F /r 94``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRCP_MM_MMM64: Code = 4187 # type: ignore
+D3NOW_PFRCP_MM_MMM64: int = 4187
 """
 ``PFRCP mm, mm/m64``
 
 ``0F 0F /r 96``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRSQRT_MM_MMM64: Code = 4188 # type: ignore
+D3NOW_PFRSQRT_MM_MMM64: int = 4188
 """
 ``PFRSQRT mm, mm/m64``
 
 ``0F 0F /r 97``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFSUB_MM_MMM64: Code = 4189 # type: ignore
+D3NOW_PFSUB_MM_MMM64: int = 4189
 """
 ``PFSUB mm, mm/m64``
 
 ``0F 0F /r 9A``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFADD_MM_MMM64: Code = 4190 # type: ignore
+D3NOW_PFADD_MM_MMM64: int = 4190
 """
 ``PFADD mm, mm/m64``
 
 ``0F 0F /r 9E``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFCMPGT_MM_MMM64: Code = 4191 # type: ignore
+D3NOW_PFCMPGT_MM_MMM64: int = 4191
 """
 ``PFCMPGT mm, mm/m64``
 
 ``0F 0F /r A0``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFMAX_MM_MMM64: Code = 4192 # type: ignore
+D3NOW_PFMAX_MM_MMM64: int = 4192
 """
 ``PFMAX mm, mm/m64``
 
 ``0F 0F /r A4``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRCPIT1_MM_MMM64: Code = 4193 # type: ignore
+D3NOW_PFRCPIT1_MM_MMM64: int = 4193
 """
 ``PFRCPIT1 mm, mm/m64``
 
 ``0F 0F /r A6``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRSQIT1_MM_MMM64: Code = 4194 # type: ignore
+D3NOW_PFRSQIT1_MM_MMM64: int = 4194
 """
 ``PFRSQIT1 mm, mm/m64``
 
 ``0F 0F /r A7``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFSUBR_MM_MMM64: Code = 4195 # type: ignore
+D3NOW_PFSUBR_MM_MMM64: int = 4195
 """
 ``PFSUBR mm, mm/m64``
 
 ``0F 0F /r AA``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFACC_MM_MMM64: Code = 4196 # type: ignore
+D3NOW_PFACC_MM_MMM64: int = 4196
 """
 ``PFACC mm, mm/m64``
 
 ``0F 0F /r AE``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFCMPEQ_MM_MMM64: Code = 4197 # type: ignore
+D3NOW_PFCMPEQ_MM_MMM64: int = 4197
 """
 ``PFCMPEQ mm, mm/m64``
 
 ``0F 0F /r B0``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFMUL_MM_MMM64: Code = 4198 # type: ignore
+D3NOW_PFMUL_MM_MMM64: int = 4198
 """
 ``PFMUL mm, mm/m64``
 
 ``0F 0F /r B4``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PFRCPIT2_MM_MMM64: Code = 4199 # type: ignore
+D3NOW_PFRCPIT2_MM_MMM64: int = 4199
 """
 ``PFRCPIT2 mm, mm/m64``
 
 ``0F 0F /r B6``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PMULHRW_MM_MMM64: Code = 4200 # type: ignore
+D3NOW_PMULHRW_MM_MMM64: int = 4200
 """
 ``PMULHRW mm, mm/m64``
 
 ``0F 0F /r B7``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-D3NOW_PSWAPD_MM_MMM64: Code = 4201 # type: ignore
+D3NOW_PSWAPD_MM_MMM64: int = 4201
 """
 ``PSWAPD mm, mm/m64``
 
 ``0F 0F /r BB``
 
 ``3DNOWEXT``
 
 ``16/32/64-bit``
 """
-D3NOW_PAVGUSB_MM_MMM64: Code = 4202 # type: ignore
+D3NOW_PAVGUSB_MM_MMM64: int = 4202
 """
 ``PAVGUSB mm, mm/m64``
 
 ``0F 0F /r BF``
 
 ``3DNOW``
 
 ``16/32/64-bit``
 """
-RMPADJUST: Code = 4203 # type: ignore
+RMPADJUST: int = 4203
 """
 ``RMPADJUST``
 
 ``F3 0F 01 FE``
 
 ``SEV-SNP``
 
 ``64-bit``
 """
-RMPUPDATE: Code = 4204 # type: ignore
+RMPUPDATE: int = 4204
 """
 ``RMPUPDATE``
 
 ``F2 0F 01 FE``
 
 ``SEV-SNP``
 
 ``64-bit``
 """
-PSMASH: Code = 4205 # type: ignore
+PSMASH: int = 4205
 """
 ``PSMASH``
 
 ``F3 0F 01 FF``
 
 ``SEV-SNP``
 
 ``64-bit``
 """
-PVALIDATEW: Code = 4206 # type: ignore
+PVALIDATEW: int = 4206
 """
 ``PVALIDATE``
 
 ``a16 F2 0F 01 FF``
 
 ``SEV-SNP``
 
 ``16/32-bit``
 """
-PVALIDATED: Code = 4207 # type: ignore
+PVALIDATED: int = 4207
 """
 ``PVALIDATE``
 
 ``a32 F2 0F 01 FF``
 
 ``SEV-SNP``
 
 ``16/32/64-bit``
 """
-PVALIDATEQ: Code = 4208 # type: ignore
+PVALIDATEQ: int = 4208
 """
 ``PVALIDATE``
 
 ``a64 F2 0F 01 FF``
 
 ``SEV-SNP``
 
 ``64-bit``
 """
-SERIALIZE: Code = 4209 # type: ignore
+SERIALIZE: int = 4209
 """
 ``SERIALIZE``
 
 ``NP 0F 01 E8``
 
 ``SERIALIZE``
 
 ``16/32/64-bit``
 """
-XSUSLDTRK: Code = 4210 # type: ignore
+XSUSLDTRK: int = 4210
 """
 ``XSUSLDTRK``
 
 ``F2 0F 01 E8``
 
 ``TSXLDTRK``
 
 ``16/32/64-bit``
 """
-XRESLDTRK: Code = 4211 # type: ignore
+XRESLDTRK: int = 4211
 """
 ``XRESLDTRK``
 
 ``F2 0F 01 E9``
 
 ``TSXLDTRK``
 
 ``16/32/64-bit``
 """
-INVLPGBW: Code = 4212 # type: ignore
+INVLPGBW: int = 4212
 """
 ``INVLPGB``
 
 ``a16 NP 0F 01 FE``
 
 ``INVLPGB``
 
 ``16/32-bit``
 """
-INVLPGBD: Code = 4213 # type: ignore
+INVLPGBD: int = 4213
 """
 ``INVLPGB``
 
 ``a32 NP 0F 01 FE``
 
 ``INVLPGB``
 
 ``16/32/64-bit``
 """
-INVLPGBQ: Code = 4214 # type: ignore
+INVLPGBQ: int = 4214
 """
 ``INVLPGB``
 
 ``a64 NP 0F 01 FE``
 
 ``INVLPGB``
 
 ``64-bit``
 """
-TLBSYNC: Code = 4215 # type: ignore
+TLBSYNC: int = 4215
 """
 ``TLBSYNC``
 
 ``NP 0F 01 FF``
 
 ``INVLPGB``
 
 ``16/32/64-bit``
 """
-PREFETCHRESERVED3_M8: Code = 4216 # type: ignore
+PREFETCHRESERVED3_M8: int = 4216
 """
 ``PREFETCHW m8``
 
 ``0F 0D /3``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHRESERVED4_M8: Code = 4217 # type: ignore
+PREFETCHRESERVED4_M8: int = 4217
 """
 ``PREFETCH m8``
 
 ``0F 0D /4``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHRESERVED5_M8: Code = 4218 # type: ignore
+PREFETCHRESERVED5_M8: int = 4218
 """
 ``PREFETCH m8``
 
 ``0F 0D /5``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHRESERVED6_M8: Code = 4219 # type: ignore
+PREFETCHRESERVED6_M8: int = 4219
 """
 ``PREFETCH m8``
 
 ``0F 0D /6``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-PREFETCHRESERVED7_M8: Code = 4220 # type: ignore
+PREFETCHRESERVED7_M8: int = 4220
 """
 ``PREFETCH m8``
 
 ``0F 0D /7``
 
 ``PREFETCHW``
 
 ``16/32/64-bit``
 """
-UD0: Code = 4221 # type: ignore
+UD0: int = 4221
 """
 ``UD0``
 
 ``0F FF``
 
 ``286+``
 
 ``16/32/64-bit``
 """
-VMGEXIT: Code = 4222 # type: ignore
+VMGEXIT: int = 4222
 """
 ``VMGEXIT``
 
 ``F3 0F 01 D9``
 
 ``SEV-ES``
 
 ``16/32/64-bit``
 """
-GETSECQ: Code = 4223 # type: ignore
+GETSECQ: int = 4223
 """
 ``GETSECQ``
 
 ``NP o64 0F 37``
 
 ``SMX``
 
 ``64-bit``
 """
-VEX_LDTILECFG_M512: Code = 4224 # type: ignore
+VEX_LDTILECFG_M512: int = 4224
 """
 ``LDTILECFG m512``
 
 ``VEX.128.0F38.W0 49 !(11):000:bbb``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TILERELEASE: Code = 4225 # type: ignore
+VEX_TILERELEASE: int = 4225
 """
 ``TILERELEASE``
 
 ``VEX.128.0F38.W0 49 C0``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_STTILECFG_M512: Code = 4226 # type: ignore
+VEX_STTILECFG_M512: int = 4226
 """
 ``STTILECFG m512``
 
 ``VEX.128.66.0F38.W0 49 !(11):000:bbb``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TILEZERO_TMM: Code = 4227 # type: ignore
+VEX_TILEZERO_TMM: int = 4227
 """
 ``TILEZERO tmm1``
 
 ``VEX.128.F2.0F38.W0 49 11:rrr:000``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TILELOADDT1_TMM_SIBMEM: Code = 4228 # type: ignore
+VEX_TILELOADDT1_TMM_SIBMEM: int = 4228
 """
 ``TILELOADDT1 tmm1, sibmem``
 
 ``VEX.128.66.0F38.W0 4B !(11):rrr:100``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TILESTORED_SIBMEM_TMM: Code = 4229 # type: ignore
+VEX_TILESTORED_SIBMEM_TMM: int = 4229
 """
 ``TILESTORED sibmem, tmm1``
 
 ``VEX.128.F3.0F38.W0 4B !(11):rrr:100``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TILELOADD_TMM_SIBMEM: Code = 4230 # type: ignore
+VEX_TILELOADD_TMM_SIBMEM: int = 4230
 """
 ``TILELOADD tmm1, sibmem``
 
 ``VEX.128.F2.0F38.W0 4B !(11):rrr:100``
 
 ``AMX-TILE``
 
 ``64-bit``
 """
-VEX_TDPBF16PS_TMM_TMM_TMM: Code = 4231 # type: ignore
+VEX_TDPBF16PS_TMM_TMM_TMM: int = 4231
 """
 ``TDPBF16PS tmm1, tmm2, tmm3``
 
 ``VEX.128.F3.0F38.W0 5C 11:rrr:bbb``
 
 ``AMX-BF16``
 
 ``64-bit``
 """
-VEX_TDPBUUD_TMM_TMM_TMM: Code = 4232 # type: ignore
+VEX_TDPBUUD_TMM_TMM_TMM: int = 4232
 """
 ``TDPBUUD tmm1, tmm2, tmm3``
 
 ``VEX.128.0F38.W0 5E 11:rrr:bbb``
 
 ``AMX-INT8``
 
 ``64-bit``
 """
-VEX_TDPBUSD_TMM_TMM_TMM: Code = 4233 # type: ignore
+VEX_TDPBUSD_TMM_TMM_TMM: int = 4233
 """
 ``TDPBUSD tmm1, tmm2, tmm3``
 
 ``VEX.128.66.0F38.W0 5E 11:rrr:bbb``
 
 ``AMX-INT8``
 
 ``64-bit``
 """
-VEX_TDPBSUD_TMM_TMM_TMM: Code = 4234 # type: ignore
+VEX_TDPBSUD_TMM_TMM_TMM: int = 4234
 """
 ``TDPBSUD tmm1, tmm2, tmm3``
 
 ``VEX.128.F3.0F38.W0 5E 11:rrr:bbb``
 
 ``AMX-INT8``
 
 ``64-bit``
 """
-VEX_TDPBSSD_TMM_TMM_TMM: Code = 4235 # type: ignore
+VEX_TDPBSSD_TMM_TMM_TMM: int = 4235
 """
 ``TDPBSSD tmm1, tmm2, tmm3``
 
 ``VEX.128.F2.0F38.W0 5E 11:rrr:bbb``
 
 ``AMX-INT8``
 
 ``64-bit``
 """
-FNSTDW_AX: Code = 4236 # type: ignore
+FNSTDW_AX: int = 4236
 """
 ``FNSTDW AX``
 
 ``DF E1``
 
 ``387 SL``
 
 ``16/32-bit``
 """
-FNSTSG_AX: Code = 4237 # type: ignore
+FNSTSG_AX: int = 4237
 """
 ``FNSTSG AX``
 
 ``DF E2``
 
 ``387 SL``
 
 ``16/32-bit``
 """
-RDSHR_RM32: Code = 4238 # type: ignore
+RDSHR_RM32: int = 4238
 """
 ``RDSHR r/m32``
 
 ``0F 36 /0``
 
 ``Cyrix 6x86MX, M II, III``
 
 ``16/32-bit``
 """
-WRSHR_RM32: Code = 4239 # type: ignore
+WRSHR_RM32: int = 4239
 """
 ``WRSHR r/m32``
 
 ``0F 37 /0``
 
 ``Cyrix 6x86MX, M II, III``
 
 ``16/32-bit``
 """
-SMINT: Code = 4240 # type: ignore
+SMINT: int = 4240
 """
 ``SMINT``
 
 ``0F 38``
 
 ``Cyrix 6x86MX+, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-DMINT: Code = 4241 # type: ignore
+DMINT: int = 4241
 """
 ``DMINT``
 
 ``0F 39``
 
 ``AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-RDM: Code = 4242 # type: ignore
+RDM: int = 4242
 """
 ``RDM``
 
 ``0F 3A``
 
 ``AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-SVDC_M80_SREG: Code = 4243 # type: ignore
+SVDC_M80_SREG: int = 4243
 """
 ``SVDC m80, Sreg``
 
 ``0F 78 /r``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-RSDC_SREG_M80: Code = 4244 # type: ignore
+RSDC_SREG_M80: int = 4244
 """
 ``RSDC Sreg, m80``
 
 ``0F 79 /r``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-SVLDT_M80: Code = 4245 # type: ignore
+SVLDT_M80: int = 4245
 """
 ``SVLDT m80``
 
 ``0F 7A /0``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-RSLDT_M80: Code = 4246 # type: ignore
+RSLDT_M80: int = 4246
 """
 ``RSLDT m80``
 
 ``0F 7B /0``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-SVTS_M80: Code = 4247 # type: ignore
+SVTS_M80: int = 4247
 """
 ``SVTS m80``
 
 ``0F 7C /0``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-RSTS_M80: Code = 4248 # type: ignore
+RSTS_M80: int = 4248
 """
 ``RSTS m80``
 
 ``0F 7D /0``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-SMINT_0F7E: Code = 4249 # type: ignore
+SMINT_0F7E: int = 4249
 """
 ``SMINT``
 
 ``0F 7E``
 
 ``Cyrix 6x86 or earlier``
 
 ``16/32-bit``
 """
-BB0_RESET: Code = 4250 # type: ignore
+BB0_RESET: int = 4250
 """
 ``BB0_RESET``
 
 ``0F 3A``
 
 ``Cyrix MediaGX, GXm, GXLV, GX1``
 
 ``16/32-bit``
 """
-BB1_RESET: Code = 4251 # type: ignore
+BB1_RESET: int = 4251
 """
 ``BB1_RESET``
 
 ``0F 3B``
 
 ``Cyrix MediaGX, GXm, GXLV, GX1``
 
 ``16/32-bit``
 """
-CPU_WRITE: Code = 4252 # type: ignore
+CPU_WRITE: int = 4252
 """
 ``CPU_WRITE``
 
 ``0F 3C``
 
 ``Cyrix MediaGX, GXm, GXLV, GX1``
 
 ``16/32-bit``
 """
-CPU_READ: Code = 4253 # type: ignore
+CPU_READ: int = 4253
 """
 ``CPU_READ``
 
 ``0F 3D``
 
 ``Cyrix MediaGX, GXm, GXLV, GX1``
 
 ``16/32-bit``
 """
-ALTINST: Code = 4254 # type: ignore
+ALTINST: int = 4254
 """
 ``ALTINST``
 
 ``0F 3F``
 
 ``Centaur AIS``
 
 ``16/32-bit``
 """
-PAVEB_MM_MMM64: Code = 4255 # type: ignore
+PAVEB_MM_MMM64: int = 4255
 """
 ``PAVEB mm, mm/m64``
 
 ``0F 50 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PADDSIW_MM_MMM64: Code = 4256 # type: ignore
+PADDSIW_MM_MMM64: int = 4256
 """
 ``PADDSIW mm, mm/m64``
 
 ``0F 51 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMAGW_MM_MMM64: Code = 4257 # type: ignore
+PMAGW_MM_MMM64: int = 4257
 """
 ``PMAGW mm, mm/m64``
 
 ``0F 52 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PDISTIB_MM_M64: Code = 4258 # type: ignore
+PDISTIB_MM_M64: int = 4258
 """
 ``PDISTIB mm, m64``
 
 ``0F 54 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PSUBSIW_MM_MMM64: Code = 4259 # type: ignore
+PSUBSIW_MM_MMM64: int = 4259
 """
 ``PSUBSIW mm, mm/m64``
 
 ``0F 55 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMVZB_MM_M64: Code = 4260 # type: ignore
+PMVZB_MM_M64: int = 4260
 """
 ``PMVZB mm, m64``
 
 ``0F 58 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMULHRW_MM_MMM64: Code = 4261 # type: ignore
+PMULHRW_MM_MMM64: int = 4261
 """
 ``PMULHRW mm, mm/m64``
 
 ``0F 59 /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMVNZB_MM_M64: Code = 4262 # type: ignore
+PMVNZB_MM_M64: int = 4262
 """
 ``PMVNZB mm, m64``
 
 ``0F 5A /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMVLZB_MM_M64: Code = 4263 # type: ignore
+PMVLZB_MM_M64: int = 4263
 """
 ``PMVLZB mm, m64``
 
 ``0F 5B /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMVGEZB_MM_M64: Code = 4264 # type: ignore
+PMVGEZB_MM_M64: int = 4264
 """
 ``PMVGEZB mm, m64``
 
 ``0F 5C /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMULHRIW_MM_MMM64: Code = 4265 # type: ignore
+PMULHRIW_MM_MMM64: int = 4265
 """
 ``PMULHRIW mm, mm/m64``
 
 ``0F 5D /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-PMACHRIW_MM_M64: Code = 4266 # type: ignore
+PMACHRIW_MM_M64: int = 4266
 """
 ``PMACHRIW mm, m64``
 
 ``0F 5E /r``
 
 ``CYRIX_EMMI``
 
 ``16/32-bit``
 """
-CYRIX_D9D7: Code = 4267 # type: ignore
+CYRIX_D9D7: int = 4267
 """
 ``UNDOC``
 
 ``D9 D7``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_D9E2: Code = 4268 # type: ignore
+CYRIX_D9E2: int = 4268
 """
 ``UNDOC``
 
 ``D9 E2``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-FTSTP: Code = 4269 # type: ignore
+FTSTP: int = 4269
 """
 ``FTSTP``
 
 ``D9 E6``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_D9E7: Code = 4270 # type: ignore
+CYRIX_D9E7: int = 4270
 """
 ``UNDOC``
 
 ``D9 E7``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-FRINT2: Code = 4271 # type: ignore
+FRINT2: int = 4271
 """
 ``FRINT2``
 
 ``DB FC``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-FRICHOP: Code = 4272 # type: ignore
+FRICHOP: int = 4272
 """
 ``FRICHOP``
 
 ``DD FC``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_DED8: Code = 4273 # type: ignore
+CYRIX_DED8: int = 4273
 """
 ``UNDOC``
 
 ``DE D8``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_DEDA: Code = 4274 # type: ignore
+CYRIX_DEDA: int = 4274
 """
 ``UNDOC``
 
 ``DE DA``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_DEDC: Code = 4275 # type: ignore
+CYRIX_DEDC: int = 4275
 """
 ``UNDOC``
 
 ``DE DC``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_DEDD: Code = 4276 # type: ignore
+CYRIX_DEDD: int = 4276
 """
 ``UNDOC``
 
 ``DE DD``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-CYRIX_DEDE: Code = 4277 # type: ignore
+CYRIX_DEDE: int = 4277
 """
 ``UNDOC``
 
 ``DE DE``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-FRINEAR: Code = 4278 # type: ignore
+FRINEAR: int = 4278
 """
 ``FRINEAR``
 
 ``DF FC``
 
 ``Cyrix, AMD Geode GX/LX``
 
 ``16/32-bit``
 """
-TDCALL: Code = 4279 # type: ignore
+TDCALL: int = 4279
 """
 ``TDCALL``
 
 ``66 0F 01 CC``
 
 ``TDX``
 
 ``16/32/64-bit``
 """
-SEAMRET: Code = 4280 # type: ignore
+SEAMRET: int = 4280
 """
 ``SEAMRET``
 
 ``66 0F 01 CD``
 
 ``TDX``
 
 ``64-bit``
 """
-SEAMOPS: Code = 4281 # type: ignore
+SEAMOPS: int = 4281
 """
 ``SEAMOPS``
 
 ``66 0F 01 CE``
 
 ``TDX``
 
 ``64-bit``
 """
-SEAMCALL: Code = 4282 # type: ignore
+SEAMCALL: int = 4282
 """
 ``SEAMCALL``
 
 ``66 0F 01 CF``
 
 ``TDX``
 
 ``64-bit``
 """
-AESENCWIDE128KL_M384: Code = 4283 # type: ignore
+AESENCWIDE128KL_M384: int = 4283
 """
 ``AESENCWIDE128KL m384, <XMM0-7>``
 
 ``F3 0F 38 D8 !(11):000:bbb``
 
 ``AESKLE and WIDE_KL``
 
 ``16/32/64-bit``
 """
-AESDECWIDE128KL_M384: Code = 4284 # type: ignore
+AESDECWIDE128KL_M384: int = 4284
 """
 ``AESDECWIDE128KL m384, <XMM0-7>``
 
 ``F3 0F 38 D8 !(11):001:bbb``
 
 ``AESKLE and WIDE_KL``
 
 ``16/32/64-bit``
 """
-AESENCWIDE256KL_M512: Code = 4285 # type: ignore
+AESENCWIDE256KL_M512: int = 4285
 """
 ``AESENCWIDE256KL m512, <XMM0-7>``
 
 ``F3 0F 38 D8 !(11):010:bbb``
 
 ``AESKLE and WIDE_KL``
 
 ``16/32/64-bit``
 """
-AESDECWIDE256KL_M512: Code = 4286 # type: ignore
+AESDECWIDE256KL_M512: int = 4286
 """
 ``AESDECWIDE256KL m512, <XMM0-7>``
 
 ``F3 0F 38 D8 !(11):011:bbb``
 
 ``AESKLE and WIDE_KL``
 
 ``16/32/64-bit``
 """
-LOADIWKEY_XMM_XMM: Code = 4287 # type: ignore
+LOADIWKEY_XMM_XMM: int = 4287
 """
 ``LOADIWKEY xmm1, xmm2, <EAX>, <XMM0>``
 
 ``F3 0F 38 DC 11:rrr:bbb``
 
 ``KL``
 
 ``16/32/64-bit``
 """
-AESENC128KL_XMM_M384: Code = 4288 # type: ignore
+AESENC128KL_XMM_M384: int = 4288
 """
 ``AESENC128KL xmm, m384``
 
 ``F3 0F 38 DC !(11):rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-AESDEC128KL_XMM_M384: Code = 4289 # type: ignore
+AESDEC128KL_XMM_M384: int = 4289
 """
 ``AESDEC128KL xmm, m384``
 
 ``F3 0F 38 DD !(11):rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-AESENC256KL_XMM_M512: Code = 4290 # type: ignore
+AESENC256KL_XMM_M512: int = 4290
 """
 ``AESENC256KL xmm, m512``
 
 ``F3 0F 38 DE !(11):rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-AESDEC256KL_XMM_M512: Code = 4291 # type: ignore
+AESDEC256KL_XMM_M512: int = 4291
 """
 ``AESDEC256KL xmm, m512``
 
 ``F3 0F 38 DF !(11):rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-ENCODEKEY128_R32_R32: Code = 4292 # type: ignore
+ENCODEKEY128_R32_R32: int = 4292
 """
 ``ENCODEKEY128 r32, r32, <XMM0-2>, <XMM4-6>``
 
 ``F3 0F 38 FA 11:rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-ENCODEKEY256_R32_R32: Code = 4293 # type: ignore
+ENCODEKEY256_R32_R32: int = 4293
 """
 ``ENCODEKEY256 r32, r32, <XMM0-6>``
 
 ``F3 0F 38 FB 11:rrr:bbb``
 
 ``AESKLE``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSS_XMM_XMM: Code = 4294 # type: ignore
+VEX_VBROADCASTSS_XMM_XMM: int = 4294
 """
 ``VBROADCASTSS xmm1, xmm2``
 
 ``VEX.128.66.0F38.W0 18 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSS_YMM_XMM: Code = 4295 # type: ignore
+VEX_VBROADCASTSS_YMM_XMM: int = 4295
 """
 ``VBROADCASTSS ymm1, xmm2``
 
 ``VEX.256.66.0F38.W0 18 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VEX_VBROADCASTSD_YMM_XMM: Code = 4296 # type: ignore
+VEX_VBROADCASTSD_YMM_XMM: int = 4296
 """
 ``VBROADCASTSD ymm1, xmm2``
 
 ``VEX.256.66.0F38.W0 19 /r``
 
 ``AVX2``
 
 ``16/32/64-bit``
 """
-VMGEXIT_F2: Code = 4297 # type: ignore
+VMGEXIT_F2: int = 4297
 """
 ``VMGEXIT``
 
 ``F2 0F 01 D9``
 
 ``SEV-ES``
 
 ``16/32/64-bit``
 """
-UIRET: Code = 4298 # type: ignore
+UIRET: int = 4298
 """
 ``UIRET``
 
 ``F3 0F 01 EC``
 
 ``UINTR``
 
 ``64-bit``
 """
-TESTUI: Code = 4299 # type: ignore
+TESTUI: int = 4299
 """
 ``TESTUI``
 
 ``F3 0F 01 ED``
 
 ``UINTR``
 
 ``64-bit``
 """
-CLUI: Code = 4300 # type: ignore
+CLUI: int = 4300
 """
 ``CLUI``
 
 ``F3 0F 01 EE``
 
 ``UINTR``
 
 ``64-bit``
 """
-STUI: Code = 4301 # type: ignore
+STUI: int = 4301
 """
 ``STUI``
 
 ``F3 0F 01 EF``
 
 ``UINTR``
 
 ``64-bit``
 """
-SENDUIPI_R64: Code = 4302 # type: ignore
+SENDUIPI_R64: int = 4302
 """
 ``SENDUIPI r64``
 
 ``F3 0F C7 /6``
 
 ``UINTR``
 
 ``64-bit``
 """
-HRESET_IMM8: Code = 4303 # type: ignore
+HRESET_IMM8: int = 4303
 """
 ``HRESET imm8, <EAX>``
 
 ``F3 0F 3A F0 C0 ib``
 
 ``HRESET``
 
 ``16/32/64-bit``
 """
-VEX_VPDPBUSD_XMM_XMM_XMMM128: Code = 4304 # type: ignore
+VEX_VPDPBUSD_XMM_XMM_XMMM128: int = 4304
 """
 ``VPDPBUSD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 50 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPBUSD_YMM_YMM_YMMM256: Code = 4305 # type: ignore
+VEX_VPDPBUSD_YMM_YMM_YMMM256: int = 4305
 """
 ``VPDPBUSD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 50 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPBUSDS_XMM_XMM_XMMM128: Code = 4306 # type: ignore
+VEX_VPDPBUSDS_XMM_XMM_XMMM128: int = 4306
 """
 ``VPDPBUSDS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 51 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPBUSDS_YMM_YMM_YMMM256: Code = 4307 # type: ignore
+VEX_VPDPBUSDS_YMM_YMM_YMMM256: int = 4307
 """
 ``VPDPBUSDS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 51 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPWSSD_XMM_XMM_XMMM128: Code = 4308 # type: ignore
+VEX_VPDPWSSD_XMM_XMM_XMMM128: int = 4308
 """
 ``VPDPWSSD xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 52 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPWSSD_YMM_YMM_YMMM256: Code = 4309 # type: ignore
+VEX_VPDPWSSD_YMM_YMM_YMMM256: int = 4309
 """
 ``VPDPWSSD ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 52 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPWSSDS_XMM_XMM_XMMM128: Code = 4310 # type: ignore
+VEX_VPDPWSSDS_XMM_XMM_XMMM128: int = 4310
 """
 ``VPDPWSSDS xmm1, xmm2, xmm3/m128``
 
 ``VEX.128.66.0F38.W0 53 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-VEX_VPDPWSSDS_YMM_YMM_YMMM256: Code = 4311 # type: ignore
+VEX_VPDPWSSDS_YMM_YMM_YMMM256: int = 4311
 """
 ``VPDPWSSDS ymm1, ymm2, ymm3/m256``
 
 ``VEX.256.66.0F38.W0 53 /r``
 
 ``AVX-VNNI``
 
 ``16/32/64-bit``
 """
-CCS_HASH_16: Code = 4312 # type: ignore
+CCS_HASH_16: int = 4312
 """
 ``CCS_HASH``
 
 ``a16 F3 0F A6 E8``
 
 ``PADLOCK_GMI``
 
 ``16/32-bit``
 """
-CCS_HASH_32: Code = 4313 # type: ignore
+CCS_HASH_32: int = 4313
 """
 ``CCS_HASH``
 
 ``a32 F3 0F A6 E8``
 
 ``PADLOCK_GMI``
 
 ``16/32/64-bit``
 """
-CCS_HASH_64: Code = 4314 # type: ignore
+CCS_HASH_64: int = 4314
 """
 ``CCS_HASH``
 
 ``a64 F3 0F A6 E8``
 
 ``PADLOCK_GMI``
 
 ``64-bit``
 """
-CCS_ENCRYPT_16: Code = 4315 # type: ignore
+CCS_ENCRYPT_16: int = 4315
 """
 ``CCS_ENCRYPT``
 
 ``a16 F3 0F A7 F0``
 
 ``PADLOCK_GMI``
 
 ``16/32-bit``
 """
-CCS_ENCRYPT_32: Code = 4316 # type: ignore
+CCS_ENCRYPT_32: int = 4316
 """
 ``CCS_ENCRYPT``
 
 ``a32 F3 0F A7 F0``
 
 ``PADLOCK_GMI``
 
 ``16/32/64-bit``
 """
-CCS_ENCRYPT_64: Code = 4317 # type: ignore
+CCS_ENCRYPT_64: int = 4317
 """
 ``CCS_ENCRYPT``
 
 ``a64 F3 0F A7 F0``
 
 ``PADLOCK_GMI``
 
 ``64-bit``
 """
-LKGS_RM16: Code = 4318 # type: ignore
-"""
-``LKGS r/m16``
-
-``o16 F2 0F 00 /6``
-
-``LKGS``
-
-``64-bit``
-"""
-LKGS_R32M16: Code = 4319 # type: ignore
-"""
-``LKGS r32/m16``
-
-``o32 F2 0F 00 /6``
-
-``LKGS``
-
-``64-bit``
-"""
-LKGS_R64M16: Code = 4320 # type: ignore
-"""
-``LKGS r64/m16``
-
-``F2 o64 0F 00 /6``
-
-``LKGS``
-
-``64-bit``
-"""
-ERETU: Code = 4321 # type: ignore
-"""
-``ERETU``
-
-``F3 0F 01 CA``
-
-``FRED``
-
-``64-bit``
-"""
-ERETS: Code = 4322 # type: ignore
-"""
-``ERETS``
-
-``F2 0F 01 CA``
-
-``FRED``
-
-``64-bit``
-"""
-EVEX_VADDPH_XMM_K1Z_XMM_XMMM128B16: Code = 4323 # type: ignore
-"""
-``VADDPH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.MAP5.W0 58 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VADDPH_YMM_K1Z_YMM_YMMM256B16: Code = 4324 # type: ignore
-"""
-``VADDPH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.MAP5.W0 58 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VADDPH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4325 # type: ignore
-"""
-``VADDPH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.MAP5.W0 58 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VADDSH_XMM_K1Z_XMM_XMMM16_ER: Code = 4326 # type: ignore
-"""
-``VADDSH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W0 58 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCMPPH_KR_K1_XMM_XMMM128B16_IMM8: Code = 4327 # type: ignore
-"""
-``VCMPPH k1 {k2}, xmm2, xmm3/m128/m16bcst, imm8``
-
-``EVEX.128.0F3A.W0 C2 /r ib``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCMPPH_KR_K1_YMM_YMMM256B16_IMM8: Code = 4328 # type: ignore
-"""
-``VCMPPH k1 {k2}, ymm2, ymm3/m256/m16bcst, imm8``
-
-``EVEX.256.0F3A.W0 C2 /r ib``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCMPPH_KR_K1_ZMM_ZMMM512B16_IMM8_SAE: Code = 4329 # type: ignore
-"""
-``VCMPPH k1 {k2}, zmm2, zmm3/m512/m16bcst{sae}, imm8``
-
-``EVEX.512.0F3A.W0 C2 /r ib``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCMPSH_KR_K1_XMM_XMMM16_IMM8_SAE: Code = 4330 # type: ignore
-"""
-``VCMPSH k1 {k2}, xmm2, xmm3/m16{sae}, imm8``
-
-``EVEX.LIG.F3.0F3A.W0 C2 /r ib``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCOMISH_XMM_XMMM16_SAE: Code = 4331 # type: ignore
-"""
-``VCOMISH xmm1, xmm2/m16{sae}``
-
-``EVEX.LIG.MAP5.W0 2F /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTDQ2PH_XMM_K1Z_XMMM128B32: Code = 4332 # type: ignore
-"""
-``VCVTDQ2PH xmm1 {k1}{z}, xmm2/m128/m32bcst``
-
-``EVEX.128.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTDQ2PH_XMM_K1Z_YMMM256B32: Code = 4333 # type: ignore
-"""
-``VCVTDQ2PH xmm1 {k1}{z}, ymm2/m256/m32bcst``
-
-``EVEX.256.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTDQ2PH_YMM_K1Z_ZMMM512B32_ER: Code = 4334 # type: ignore
-"""
-``VCVTDQ2PH ymm1 {k1}{z}, zmm2/m512/m32bcst{er}``
-
-``EVEX.512.MAP5.W0 5B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPD2PH_XMM_K1Z_XMMM128B64: Code = 4335 # type: ignore
-"""
-``VCVTPD2PH xmm1 {k1}{z}, xmm2/m128/m64bcst``
-
-``EVEX.128.66.MAP5.W1 5A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPD2PH_XMM_K1Z_YMMM256B64: Code = 4336 # type: ignore
-"""
-``VCVTPD2PH xmm1 {k1}{z}, ymm2/m256/m64bcst``
-
-``EVEX.256.66.MAP5.W1 5A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPD2PH_XMM_K1Z_ZMMM512B64_ER: Code = 4337 # type: ignore
-"""
-``VCVTPD2PH xmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
-
-``EVEX.512.66.MAP5.W1 5A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2DQ_XMM_K1Z_XMMM64B16: Code = 4338 # type: ignore
-"""
-``VCVTPH2DQ xmm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.128.66.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2DQ_YMM_K1Z_XMMM128B16: Code = 4339 # type: ignore
-"""
-``VCVTPH2DQ ymm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.256.66.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2DQ_ZMM_K1Z_YMMM256B16_ER: Code = 4340 # type: ignore
-"""
-``VCVTPH2DQ zmm1 {k1}{z}, ymm2/m256/m16bcst{er}``
-
-``EVEX.512.66.MAP5.W0 5B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PD_XMM_K1Z_XMMM32B16: Code = 4341 # type: ignore
-"""
-``VCVTPH2PD xmm1 {k1}{z}, xmm2/m32/m16bcst``
-
-``EVEX.128.MAP5.W0 5A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PD_YMM_K1Z_XMMM64B16: Code = 4342 # type: ignore
-"""
-``VCVTPH2PD ymm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.256.MAP5.W0 5A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PD_ZMM_K1Z_XMMM128B16_SAE: Code = 4343 # type: ignore
-"""
-``VCVTPH2PD zmm1 {k1}{z}, xmm2/m128/m16bcst{sae}``
-
-``EVEX.512.MAP5.W0 5A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PSX_XMM_K1Z_XMMM64B16: Code = 4344 # type: ignore
-"""
-``VCVTPH2PSX xmm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.128.66.MAP6.W0 13 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PSX_YMM_K1Z_XMMM128B16: Code = 4345 # type: ignore
-"""
-``VCVTPH2PSX ymm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.256.66.MAP6.W0 13 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2PSX_ZMM_K1Z_YMMM256B16_SAE: Code = 4346 # type: ignore
-"""
-``VCVTPH2PSX zmm1 {k1}{z}, ymm2/m256/m16bcst{sae}``
-
-``EVEX.512.66.MAP6.W0 13 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2QQ_XMM_K1Z_XMMM32B16: Code = 4347 # type: ignore
-"""
-``VCVTPH2QQ xmm1 {k1}{z}, xmm2/m32/m16bcst``
-
-``EVEX.128.66.MAP5.W0 7B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2QQ_YMM_K1Z_XMMM64B16: Code = 4348 # type: ignore
-"""
-``VCVTPH2QQ ymm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.256.66.MAP5.W0 7B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2QQ_ZMM_K1Z_XMMM128B16_ER: Code = 4349 # type: ignore
-"""
-``VCVTPH2QQ zmm1 {k1}{z}, xmm2/m128/m16bcst{er}``
-
-``EVEX.512.66.MAP5.W0 7B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UDQ_XMM_K1Z_XMMM64B16: Code = 4350 # type: ignore
-"""
-``VCVTPH2UDQ xmm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.128.MAP5.W0 79 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UDQ_YMM_K1Z_XMMM128B16: Code = 4351 # type: ignore
-"""
-``VCVTPH2UDQ ymm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.256.MAP5.W0 79 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UDQ_ZMM_K1Z_YMMM256B16_ER: Code = 4352 # type: ignore
-"""
-``VCVTPH2UDQ zmm1 {k1}{z}, ymm2/m256/m16bcst{er}``
-
-``EVEX.512.MAP5.W0 79 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UQQ_XMM_K1Z_XMMM32B16: Code = 4353 # type: ignore
-"""
-``VCVTPH2UQQ xmm1 {k1}{z}, xmm2/m32/m16bcst``
-
-``EVEX.128.66.MAP5.W0 79 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UQQ_YMM_K1Z_XMMM64B16: Code = 4354 # type: ignore
-"""
-``VCVTPH2UQQ ymm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.256.66.MAP5.W0 79 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UQQ_ZMM_K1Z_XMMM128B16_ER: Code = 4355 # type: ignore
-"""
-``VCVTPH2UQQ zmm1 {k1}{z}, xmm2/m128/m16bcst{er}``
-
-``EVEX.512.66.MAP5.W0 79 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UW_XMM_K1Z_XMMM128B16: Code = 4356 # type: ignore
-"""
-``VCVTPH2UW xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UW_YMM_K1Z_YMMM256B16: Code = 4357 # type: ignore
-"""
-``VCVTPH2UW ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2UW_ZMM_K1Z_ZMMM512B16_ER: Code = 4358 # type: ignore
-"""
-``VCVTPH2UW zmm1 {k1}{z}, zmm2/m512/m16bcst{er}``
-
-``EVEX.512.MAP5.W0 7D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2W_XMM_K1Z_XMMM128B16: Code = 4359 # type: ignore
-"""
-``VCVTPH2W xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.66.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2W_YMM_K1Z_YMMM256B16: Code = 4360 # type: ignore
-"""
-``VCVTPH2W ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.66.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPH2W_ZMM_K1Z_ZMMM512B16_ER: Code = 4361 # type: ignore
-"""
-``VCVTPH2W zmm1 {k1}{z}, zmm2/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP5.W0 7D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPS2PHX_XMM_K1Z_XMMM128B32: Code = 4362 # type: ignore
-"""
-``VCVTPS2PHX xmm1 {k1}{z}, xmm2/m128/m32bcst``
-
-``EVEX.128.66.MAP5.W0 1D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPS2PHX_XMM_K1Z_YMMM256B32: Code = 4363 # type: ignore
-"""
-``VCVTPS2PHX xmm1 {k1}{z}, ymm2/m256/m32bcst``
-
-``EVEX.256.66.MAP5.W0 1D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTPS2PHX_YMM_K1Z_ZMMM512B32_ER: Code = 4364 # type: ignore
-"""
-``VCVTPS2PHX ymm1 {k1}{z}, zmm2/m512/m32bcst{er}``
-
-``EVEX.512.66.MAP5.W0 1D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTQQ2PH_XMM_K1Z_XMMM128B64: Code = 4365 # type: ignore
-"""
-``VCVTQQ2PH xmm1 {k1}{z}, xmm2/m128/m64bcst``
-
-``EVEX.128.MAP5.W1 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTQQ2PH_XMM_K1Z_YMMM256B64: Code = 4366 # type: ignore
-"""
-``VCVTQQ2PH xmm1 {k1}{z}, ymm2/m256/m64bcst``
-
-``EVEX.256.MAP5.W1 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTQQ2PH_XMM_K1Z_ZMMM512B64_ER: Code = 4367 # type: ignore
-"""
-``VCVTQQ2PH xmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
-
-``EVEX.512.MAP5.W1 5B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSD2SH_XMM_K1Z_XMM_XMMM64_ER: Code = 4368 # type: ignore
-"""
-``VCVTSD2SH xmm1 {k1}{z}, xmm2, xmm3/m64{er}``
-
-``EVEX.LIG.F2.MAP5.W1 5A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSH2SD_XMM_K1Z_XMM_XMMM16_SAE: Code = 4369 # type: ignore
-"""
-``VCVTSH2SD xmm1 {k1}{z}, xmm2, xmm3/m16{sae}``
-
-``EVEX.LIG.F3.MAP5.W0 5A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSH2SI_R32_XMMM16_ER: Code = 4370 # type: ignore
-"""
-``VCVTSH2SI r32, xmm1/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W0 2D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSH2SI_R64_XMMM16_ER: Code = 4371 # type: ignore
-"""
-``VCVTSH2SI r64, xmm1/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W1 2D /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTSH2SS_XMM_K1Z_XMM_XMMM16_SAE: Code = 4372 # type: ignore
-"""
-``VCVTSH2SS xmm1 {k1}{z}, xmm2, xmm3/m16{sae}``
-
-``EVEX.LIG.MAP6.W0 13 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSH2USI_R32_XMMM16_ER: Code = 4373 # type: ignore
-"""
-``VCVTSH2USI r32, xmm1/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W0 79 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSH2USI_R64_XMMM16_ER: Code = 4374 # type: ignore
-"""
-``VCVTSH2USI r64, xmm1/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W1 79 /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTSI2SH_XMM_XMM_RM32_ER: Code = 4375 # type: ignore
-"""
-``VCVTSI2SH xmm1, xmm2, r/m32{er}``
-
-``EVEX.LIG.F3.MAP5.W0 2A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTSI2SH_XMM_XMM_RM64_ER: Code = 4376 # type: ignore
-"""
-``VCVTSI2SH xmm1, xmm2, r/m64{er}``
-
-``EVEX.LIG.F3.MAP5.W1 2A /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTSS2SH_XMM_K1Z_XMM_XMMM32_ER: Code = 4377 # type: ignore
-"""
-``VCVTSS2SH xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
-
-``EVEX.LIG.MAP5.W0 1D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2DQ_XMM_K1Z_XMMM64B16: Code = 4378 # type: ignore
-"""
-``VCVTTPH2DQ xmm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.128.F3.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2DQ_YMM_K1Z_XMMM128B16: Code = 4379 # type: ignore
-"""
-``VCVTTPH2DQ ymm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.256.F3.MAP5.W0 5B /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2DQ_ZMM_K1Z_YMMM256B16_SAE: Code = 4380 # type: ignore
-"""
-``VCVTTPH2DQ zmm1 {k1}{z}, ymm2/m256/m16bcst{sae}``
-
-``EVEX.512.F3.MAP5.W0 5B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2QQ_XMM_K1Z_XMMM32B16: Code = 4381 # type: ignore
-"""
-``VCVTTPH2QQ xmm1 {k1}{z}, xmm2/m32/m16bcst``
-
-``EVEX.128.66.MAP5.W0 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2QQ_YMM_K1Z_XMMM64B16: Code = 4382 # type: ignore
-"""
-``VCVTTPH2QQ ymm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.256.66.MAP5.W0 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2QQ_ZMM_K1Z_XMMM128B16_SAE: Code = 4383 # type: ignore
-"""
-``VCVTTPH2QQ zmm1 {k1}{z}, xmm2/m128/m16bcst{sae}``
-
-``EVEX.512.66.MAP5.W0 7A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UDQ_XMM_K1Z_XMMM64B16: Code = 4384 # type: ignore
-"""
-``VCVTTPH2UDQ xmm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.128.MAP5.W0 78 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UDQ_YMM_K1Z_XMMM128B16: Code = 4385 # type: ignore
-"""
-``VCVTTPH2UDQ ymm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.256.MAP5.W0 78 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UDQ_ZMM_K1Z_YMMM256B16_SAE: Code = 4386 # type: ignore
-"""
-``VCVTTPH2UDQ zmm1 {k1}{z}, ymm2/m256/m16bcst{sae}``
-
-``EVEX.512.MAP5.W0 78 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UQQ_XMM_K1Z_XMMM32B16: Code = 4387 # type: ignore
-"""
-``VCVTTPH2UQQ xmm1 {k1}{z}, xmm2/m32/m16bcst``
-
-``EVEX.128.66.MAP5.W0 78 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UQQ_YMM_K1Z_XMMM64B16: Code = 4388 # type: ignore
-"""
-``VCVTTPH2UQQ ymm1 {k1}{z}, xmm2/m64/m16bcst``
-
-``EVEX.256.66.MAP5.W0 78 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UQQ_ZMM_K1Z_XMMM128B16_SAE: Code = 4389 # type: ignore
-"""
-``VCVTTPH2UQQ zmm1 {k1}{z}, xmm2/m128/m16bcst{sae}``
-
-``EVEX.512.66.MAP5.W0 78 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UW_XMM_K1Z_XMMM128B16: Code = 4390 # type: ignore
-"""
-``VCVTTPH2UW xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.MAP5.W0 7C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UW_YMM_K1Z_YMMM256B16: Code = 4391 # type: ignore
-"""
-``VCVTTPH2UW ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.MAP5.W0 7C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2UW_ZMM_K1Z_ZMMM512B16_SAE: Code = 4392 # type: ignore
-"""
-``VCVTTPH2UW zmm1 {k1}{z}, zmm2/m512/m16bcst{sae}``
-
-``EVEX.512.MAP5.W0 7C /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2W_XMM_K1Z_XMMM128B16: Code = 4393 # type: ignore
-"""
-``VCVTTPH2W xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.66.MAP5.W0 7C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2W_YMM_K1Z_YMMM256B16: Code = 4394 # type: ignore
-"""
-``VCVTTPH2W ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.66.MAP5.W0 7C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTPH2W_ZMM_K1Z_ZMMM512B16_SAE: Code = 4395 # type: ignore
-"""
-``VCVTTPH2W zmm1 {k1}{z}, zmm2/m512/m16bcst{sae}``
-
-``EVEX.512.66.MAP5.W0 7C /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTSH2SI_R32_XMMM16_SAE: Code = 4396 # type: ignore
-"""
-``VCVTTSH2SI r32, xmm1/m16{sae}``
-
-``EVEX.LIG.F3.MAP5.W0 2C /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTSH2SI_R64_XMMM16_SAE: Code = 4397 # type: ignore
-"""
-``VCVTTSH2SI r64, xmm1/m16{sae}``
-
-``EVEX.LIG.F3.MAP5.W1 2C /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTTSH2USI_R32_XMMM16_SAE: Code = 4398 # type: ignore
-"""
-``VCVTTSH2USI r32, xmm1/m16{sae}``
-
-``EVEX.LIG.F3.MAP5.W0 78 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTTSH2USI_R64_XMMM16_SAE: Code = 4399 # type: ignore
-"""
-``VCVTTSH2USI r64, xmm1/m16{sae}``
-
-``EVEX.LIG.F3.MAP5.W1 78 /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTUDQ2PH_XMM_K1Z_XMMM128B32: Code = 4400 # type: ignore
-"""
-``VCVTUDQ2PH xmm1 {k1}{z}, xmm2/m128/m32bcst``
-
-``EVEX.128.F2.MAP5.W0 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUDQ2PH_XMM_K1Z_YMMM256B32: Code = 4401 # type: ignore
-"""
-``VCVTUDQ2PH xmm1 {k1}{z}, ymm2/m256/m32bcst``
-
-``EVEX.256.F2.MAP5.W0 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUDQ2PH_YMM_K1Z_ZMMM512B32_ER: Code = 4402 # type: ignore
-"""
-``VCVTUDQ2PH ymm1 {k1}{z}, zmm2/m512/m32bcst{er}``
-
-``EVEX.512.F2.MAP5.W0 7A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUQQ2PH_XMM_K1Z_XMMM128B64: Code = 4403 # type: ignore
-"""
-``VCVTUQQ2PH xmm1 {k1}{z}, xmm2/m128/m64bcst``
-
-``EVEX.128.F2.MAP5.W1 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUQQ2PH_XMM_K1Z_YMMM256B64: Code = 4404 # type: ignore
-"""
-``VCVTUQQ2PH xmm1 {k1}{z}, ymm2/m256/m64bcst``
-
-``EVEX.256.F2.MAP5.W1 7A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUQQ2PH_XMM_K1Z_ZMMM512B64_ER: Code = 4405 # type: ignore
-"""
-``VCVTUQQ2PH xmm1 {k1}{z}, zmm2/m512/m64bcst{er}``
-
-``EVEX.512.F2.MAP5.W1 7A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUSI2SH_XMM_XMM_RM32_ER: Code = 4406 # type: ignore
-"""
-``VCVTUSI2SH xmm1, xmm2, r/m32{er}``
-
-``EVEX.LIG.F3.MAP5.W0 7B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUSI2SH_XMM_XMM_RM64_ER: Code = 4407 # type: ignore
-"""
-``VCVTUSI2SH xmm1, xmm2, r/m64{er}``
-
-``EVEX.LIG.F3.MAP5.W1 7B /r``
-
-``AVX512-FP16``
-
-``64-bit``
-"""
-EVEX_VCVTUW2PH_XMM_K1Z_XMMM128B16: Code = 4408 # type: ignore
-"""
-``VCVTUW2PH xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.F2.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUW2PH_YMM_K1Z_YMMM256B16: Code = 4409 # type: ignore
-"""
-``VCVTUW2PH ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.F2.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTUW2PH_ZMM_K1Z_ZMMM512B16_ER: Code = 4410 # type: ignore
-"""
-``VCVTUW2PH zmm1 {k1}{z}, zmm2/m512/m16bcst{er}``
-
-``EVEX.512.F2.MAP5.W0 7D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTW2PH_XMM_K1Z_XMMM128B16: Code = 4411 # type: ignore
-"""
-``VCVTW2PH xmm1 {k1}{z}, xmm2/m128/m16bcst``
-
-``EVEX.128.F3.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTW2PH_YMM_K1Z_YMMM256B16: Code = 4412 # type: ignore
-"""
-``VCVTW2PH ymm1 {k1}{z}, ymm2/m256/m16bcst``
-
-``EVEX.256.F3.MAP5.W0 7D /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VCVTW2PH_ZMM_K1Z_ZMMM512B16_ER: Code = 4413 # type: ignore
-"""
-``VCVTW2PH zmm1 {k1}{z}, zmm2/m512/m16bcst{er}``
-
-``EVEX.512.F3.MAP5.W0 7D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VDIVPH_XMM_K1Z_XMM_XMMM128B16: Code = 4414 # type: ignore
-"""
-``VDIVPH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.MAP5.W0 5E /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VDIVPH_YMM_K1Z_YMM_YMMM256B16: Code = 4415 # type: ignore
-"""
-``VDIVPH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.MAP5.W0 5E /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VDIVPH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4416 # type: ignore
-"""
-``VDIVPH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.MAP5.W0 5E /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VDIVSH_XMM_K1Z_XMM_XMMM16_ER: Code = 4417 # type: ignore
-"""
-``VDIVSH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.F3.MAP5.W0 5E /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMADDCPH_XMM_K1Z_XMM_XMMM128B32: Code = 4418 # type: ignore
-"""
-``VFCMADDCPH xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
-
-``EVEX.128.F2.MAP6.W0 56 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMADDCPH_YMM_K1Z_YMM_YMMM256B32: Code = 4419 # type: ignore
-"""
-``VFCMADDCPH ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
-
-``EVEX.256.F2.MAP6.W0 56 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMADDCPH_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 4420 # type: ignore
-"""
-``VFCMADDCPH zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
-
-``EVEX.512.F2.MAP6.W0 56 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDCPH_XMM_K1Z_XMM_XMMM128B32: Code = 4421 # type: ignore
-"""
-``VFMADDCPH xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
-
-``EVEX.128.F3.MAP6.W0 56 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDCPH_YMM_K1Z_YMM_YMMM256B32: Code = 4422 # type: ignore
-"""
-``VFMADDCPH ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
-
-``EVEX.256.F3.MAP6.W0 56 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDCPH_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 4423 # type: ignore
-"""
-``VFMADDCPH zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
-
-``EVEX.512.F3.MAP6.W0 56 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMADDCSH_XMM_K1Z_XMM_XMMM32_ER: Code = 4424 # type: ignore
-"""
-``VFCMADDCSH xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
-
-``EVEX.LIG.F2.MAP6.W0 57 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDCSH_XMM_K1Z_XMM_XMMM32_ER: Code = 4425 # type: ignore
-"""
-``VFMADDCSH xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
-
-``EVEX.LIG.F3.MAP6.W0 57 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMULCPH_XMM_K1Z_XMM_XMMM128B32: Code = 4426 # type: ignore
-"""
-``VFCMULCPH xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
-
-``EVEX.128.F2.MAP6.W0 D6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMULCPH_YMM_K1Z_YMM_YMMM256B32: Code = 4427 # type: ignore
-"""
-``VFCMULCPH ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
-
-``EVEX.256.F2.MAP6.W0 D6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMULCPH_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 4428 # type: ignore
-"""
-``VFCMULCPH zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
-
-``EVEX.512.F2.MAP6.W0 D6 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMULCPH_XMM_K1Z_XMM_XMMM128B32: Code = 4429 # type: ignore
-"""
-``VFMULCPH xmm1 {k1}{z}, xmm2, xmm3/m128/m32bcst``
-
-``EVEX.128.F3.MAP6.W0 D6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMULCPH_YMM_K1Z_YMM_YMMM256B32: Code = 4430 # type: ignore
-"""
-``VFMULCPH ymm1 {k1}{z}, ymm2, ymm3/m256/m32bcst``
-
-``EVEX.256.F3.MAP6.W0 D6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMULCPH_ZMM_K1Z_ZMM_ZMMM512B32_ER: Code = 4431 # type: ignore
-"""
-``VFMULCPH zmm1 {k1}{z}, zmm2, zmm3/m512/m32bcst{er}``
-
-``EVEX.512.F3.MAP6.W0 D6 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFCMULCSH_XMM_K1Z_XMM_XMMM32_ER: Code = 4432 # type: ignore
-"""
-``VFCMULCSH xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
-
-``EVEX.LIG.F2.MAP6.W0 D7 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMULCSH_XMM_K1Z_XMM_XMMM32_ER: Code = 4433 # type: ignore
-"""
-``VFMULCSH xmm1 {k1}{z}, xmm2, xmm3/m32{er}``
-
-``EVEX.LIG.F3.MAP6.W0 D7 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4434 # type: ignore
-"""
-``VFMADDSUB132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 96 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4435 # type: ignore
-"""
-``VFMADDSUB132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 96 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4436 # type: ignore
-"""
-``VFMADDSUB132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 96 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4437 # type: ignore
-"""
-``VFMADDSUB213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 A6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4438 # type: ignore
-"""
-``VFMADDSUB213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 A6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4439 # type: ignore
-"""
-``VFMADDSUB213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 A6 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4440 # type: ignore
-"""
-``VFMADDSUB231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 B6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4441 # type: ignore
-"""
-``VFMADDSUB231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 B6 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADDSUB231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4442 # type: ignore
-"""
-``VFMADDSUB231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 B6 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4443 # type: ignore
-"""
-``VFMSUBADD132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 97 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4444 # type: ignore
-"""
-``VFMSUBADD132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 97 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4445 # type: ignore
-"""
-``VFMSUBADD132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 97 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4446 # type: ignore
-"""
-``VFMSUBADD213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 A7 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4447 # type: ignore
-"""
-``VFMSUBADD213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 A7 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4448 # type: ignore
-"""
-``VFMSUBADD213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 A7 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4449 # type: ignore
-"""
-``VFMSUBADD231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 B7 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4450 # type: ignore
-"""
-``VFMSUBADD231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 B7 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUBADD231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4451 # type: ignore
-"""
-``VFMSUBADD231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 B7 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4452 # type: ignore
-"""
-``VFMADD132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 98 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4453 # type: ignore
-"""
-``VFMADD132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 98 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4454 # type: ignore
-"""
-``VFMADD132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 98 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4455 # type: ignore
-"""
-``VFMADD213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 A8 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4456 # type: ignore
-"""
-``VFMADD213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 A8 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4457 # type: ignore
-"""
-``VFMADD213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 A8 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4458 # type: ignore
-"""
-``VFMADD231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 B8 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4459 # type: ignore
-"""
-``VFMADD231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 B8 /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4460 # type: ignore
-"""
-``VFMADD231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 B8 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4461 # type: ignore
-"""
-``VFNMADD132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 9C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4462 # type: ignore
-"""
-``VFNMADD132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 9C /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4463 # type: ignore
-"""
-``VFNMADD132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 9C /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4464 # type: ignore
-"""
-``VFNMADD213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 AC /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4465 # type: ignore
-"""
-``VFNMADD213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 AC /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4466 # type: ignore
-"""
-``VFNMADD213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 AC /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4467 # type: ignore
-"""
-``VFNMADD231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 BC /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4468 # type: ignore
-"""
-``VFNMADD231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 BC /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4469 # type: ignore
-"""
-``VFNMADD231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 BC /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD132SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4470 # type: ignore
-"""
-``VFMADD132SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 99 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD213SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4471 # type: ignore
-"""
-``VFMADD213SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 A9 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMADD231SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4472 # type: ignore
-"""
-``VFMADD231SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 B9 /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD132SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4473 # type: ignore
-"""
-``VFNMADD132SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 9D /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD213SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4474 # type: ignore
-"""
-``VFNMADD213SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 AD /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMADD231SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4475 # type: ignore
-"""
-``VFNMADD231SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 BD /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4476 # type: ignore
-"""
-``VFMSUB132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 9A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4477 # type: ignore
-"""
-``VFMSUB132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 9A /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4478 # type: ignore
-"""
-``VFMSUB132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 9A /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4479 # type: ignore
-"""
-``VFMSUB213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 AA /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4480 # type: ignore
-"""
-``VFMSUB213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 AA /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4481 # type: ignore
-"""
-``VFMSUB213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 AA /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4482 # type: ignore
-"""
-``VFMSUB231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 BA /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4483 # type: ignore
-"""
-``VFMSUB231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 BA /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4484 # type: ignore
-"""
-``VFMSUB231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 BA /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB132PH_XMM_K1Z_XMM_XMMM128B16: Code = 4485 # type: ignore
-"""
-``VFNMSUB132PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 9E /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB132PH_YMM_K1Z_YMM_YMMM256B16: Code = 4486 # type: ignore
-"""
-``VFNMSUB132PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 9E /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB132PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4487 # type: ignore
-"""
-``VFNMSUB132PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 9E /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB213PH_XMM_K1Z_XMM_XMMM128B16: Code = 4488 # type: ignore
-"""
-``VFNMSUB213PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 AE /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB213PH_YMM_K1Z_YMM_YMMM256B16: Code = 4489 # type: ignore
-"""
-``VFNMSUB213PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 AE /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB213PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4490 # type: ignore
-"""
-``VFNMSUB213PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 AE /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB231PH_XMM_K1Z_XMM_XMMM128B16: Code = 4491 # type: ignore
-"""
-``VFNMSUB231PH xmm1 {k1}{z}, xmm2, xmm3/m128/m16bcst``
-
-``EVEX.128.66.MAP6.W0 BE /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB231PH_YMM_K1Z_YMM_YMMM256B16: Code = 4492 # type: ignore
-"""
-``VFNMSUB231PH ymm1 {k1}{z}, ymm2, ymm3/m256/m16bcst``
-
-``EVEX.256.66.MAP6.W0 BE /r``
-
-``AVX512VL and AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFNMSUB231PH_ZMM_K1Z_ZMM_ZMMM512B16_ER: Code = 4493 # type: ignore
-"""
-``VFNMSUB231PH zmm1 {k1}{z}, zmm2, zmm3/m512/m16bcst{er}``
-
-``EVEX.512.66.MAP6.W0 BE /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB132SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4494 # type: ignore
-"""
-``VFMSUB132SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 9B /r``
-
-``AVX512-FP16``
-
-``16/32/64-bit``
-"""
-EVEX_VFMSUB213SH_XMM_K1Z_XMM_XMMM16_ER: Code = 4495 # type: ignore
-"""
-``VFMSUB213SH xmm1 {k1}{z}, xmm2, xmm3/m16{er}``
-
-``EVEX.LIG.66.MAP6.W0 AB /r``
-
-``AVX512-FP16``
-
