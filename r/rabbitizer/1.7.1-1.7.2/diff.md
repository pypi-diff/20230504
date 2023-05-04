# Comparing `tmp/rabbitizer-1.7.1.tar.gz` & `tmp/rabbitizer-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.7.1.tar", last modified: Tue May  2 17:02:54 2023, max compression
+gzip compressed data, was "rabbitizer-1.7.2.tar", last modified: Thu May  4 19:19:25 2023, max compression
```

## Comparing `rabbitizer-1.7.1.tar` & `rabbitizer-1.7.2.tar`

### file list

```diff
@@ -1,215 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/include/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerLoPairingInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerRegistersTracker.h
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/analysis/RabbitizerTrackedRegisterState.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi.inc
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Abi_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/RabbitizerConfig.h
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/RabbitizerVersion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/common/Utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType.inc
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/AccessType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory.inc
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrCategory_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrId_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrId_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrIds.inc
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix.inc
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/InstrSuffix_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_enum.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_enum.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/OperandTypes.inc
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerAccessType.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrCategory.h
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrId.h
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstrSuffix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstruction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR3000GTE.h
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR5900.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerInstructionRsp.h
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerOperandType.h
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerRegister.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/RabbitizerRegisterDescriptor.h
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/Registers_enums.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/Registers_enums.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.603278 rabbitizer-1.7.1/include/instructions/instr_id/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1.inc
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/r5900/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special1.inc
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/instr_id/rsp/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_regimm.inc
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_special.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.607278 rabbitizer-1.7.1/include/instructions/operands/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_cpu.inc
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_r3000gte.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_r5900.inc
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_rsp.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.611279 rabbitizer-1.7.1/include/instructions/registers/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprN32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprO32.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspVector.inc
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/include/rabbitizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.611279 rabbitizer-1.7.1/rabbitizer/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Abi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/AccessType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Enum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/InstrCategory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/InstrId.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/LoPairingInfo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/OperandType.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1N32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1N64.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegCop1O32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegGprN32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegGprO32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/RegistersTracker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/TrackedRegisterState.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/enums_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/enums_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_Abi.c
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_AccessType.c
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_type_Enum.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer/enums/registers/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_global_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_module.c
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_module.h
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_submodule_Utils.c
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_Instruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_LoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_RegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/rabbitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 17:02:54.000000 rabbitizer-1.7.1/rabbitizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.599279 rabbitizer-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/src/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerLoPairingInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerRegistersTracker.c
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/analysis/RabbitizerTrackedRegisterState.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.615279 rabbitizer-1.7.1/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/RabbitizerConfig.c
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/RabbitizerVersion.c
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/common/Utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrCategory_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrCategory_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)   113998 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    35672 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrId_Names_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/InstrId_Names_array.table.template
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrCategory.c
--rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrId.c
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstrSuffix.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:02:54.623278 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerRegister.c
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RabbitizerRegisterDescriptor.c
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-02 17:02:47.000000 rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.169613 rabbitizer-1.7.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.169613 rabbitizer-1.7.2/include/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/analysis/RabbitizerLoPairingInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/analysis/RabbitizerRegistersTracker.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/analysis/RabbitizerTrackedRegisterState.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.169613 rabbitizer-1.7.2/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/common/RabbitizerConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/common/RabbitizerVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/common/Utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.173614 rabbitizer-1.7.2/include/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/Abi_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/AccessType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrCategory_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrCategory_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)   113991 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrDescriptor_Descriptors_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrIdType_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrIdType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35665 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrId_Names_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrId_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/InstrSuffix_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/OperandType_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/OperandType_function_declarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/RegisterDescriptor_Descriptors_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29334 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/Registers_Names_arrays.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/Registers_enums.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/generated/instrOpercandCallbacks_array.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.173614 rabbitizer-1.7.2/include/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerAccessType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstrCategory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstrDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstrId.h
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstrIdType.h
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstrSuffix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstruction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstructionR3000GTE.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstructionR5900.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerInstructionRsp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerOperandType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerRegister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/instructions/RabbitizerRegisterDescriptor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/include/rabbitizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.177614 rabbitizer-1.7.2/rabbitizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/Abi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/AccessType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/Config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/Enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/InstrCategory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/InstrId.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/InstrIdType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/LoPairingInfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/OperandType.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegCop1N32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegCop1N64.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegCop1O32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegGprN32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegGprO32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/RegistersTracker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/TrackedRegisterState.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.181614 rabbitizer-1.7.2/rabbitizer/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/enums_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/enums_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_Abi.c
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_AccessType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_InstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_InstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_InstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_type_Enum.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.181614 rabbitizer-1.7.2/rabbitizer/enums/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_global_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_submodule_Utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22974 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_type_Instruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_type_LoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_type_RegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/rabbitizer/rabbitizer_type_TrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.181614 rabbitizer-1.7.2/rabbitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-04 19:19:25.000000 rabbitizer-1.7.2/rabbitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-04 19:19:25.000000 rabbitizer-1.7.2/rabbitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:19:25.000000 rabbitizer-1.7.2/rabbitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 19:19:25.000000 rabbitizer-1.7.2/rabbitizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.165614 rabbitizer-1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.181614 rabbitizer-1.7.2/src/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/analysis/RabbitizerLoPairingInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/analysis/RabbitizerRegistersTracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/analysis/RabbitizerTrackedRegisterState.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.181614 rabbitizer-1.7.2/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/common/RabbitizerConfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/common/RabbitizerVersion.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/common/Utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstrCategory.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21924 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstrDescriptor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstrId.c
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstrIdType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstrSuffix.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17798 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionCpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerRegister.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/src/instructions/RabbitizerRegisterDescriptor.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.185614 rabbitizer-1.7.2/tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/Abi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/AccessType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/InstrCategory.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/InstrIdType.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/InstrIds.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/InstrSuffix.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/OperandTypes.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.189614 rabbitizer-1.7.2/tables/tables/instr_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.189614 rabbitizer-1.7.2/tables/tables/instr_id/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.189614 rabbitizer-1.7.2/tables/tables/instr_id/r3000gte/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.193614 rabbitizer-1.7.2/tables/tables/instr_id/r5900/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_special1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_special2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_1.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_3.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.193614 rabbitizer-1.7.2/tables/tables/instr_id/rsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop2_vu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal_swc2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_regimm.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_special.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.193614 rabbitizer-1.7.2/tables/tables/instr_id_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id_types/InstrIdType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id_types/InstrIdType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id_types/InstrIdType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/instr_id_types/InstrIdType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.193614 rabbitizer-1.7.2/tables/tables/operands/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_cpu.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_r3000gte.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_r5900.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_rsp.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.197614 rabbitizer-1.7.2/tables/tables/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1N32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1N64.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1O32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_GprN32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_GprO32.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_R5900VF.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_R5900VI.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop0.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop2.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspGpr.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspVector.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.169613 rabbitizer-1.7.2/tables/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.197614 rabbitizer-1.7.2/tables/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/Abi_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/AccessType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrCategory_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrCategory_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrDescriptor_Descriptors_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrIdType_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrIdType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrId_Names_array.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrId_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/InstrSuffix_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/OperandType_enum.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/OperandType_function_declarations.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/Registers_Names_arrays.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/Registers_enums.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/c/instrOpercandCallbacks_array.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/tables/templates/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/cplusplus/AccessType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/cplusplus/InstrIdType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/cplusplus/OperandType_enum_class.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/cplusplus/Registers_enum_classes.table.template
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/cplusplus/UniqueId_enum_class.table.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/tables/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/Abi.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/AccessType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/InstrCategory.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/InstrId.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/InstrIdType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/OperandType.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/RegCop1N32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/RegCop1N64.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/RegCop1O32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/RegGprN32.tablepyi.template
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/python/RegGprO32.tablepyi.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/tables/templates/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/abi_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/access_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/instr_category_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/instr_id_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/instr_id_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/instr_suffix_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/operand_type_enum.tablers.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/templates/rust/registers_enum.tablers.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:19:25.201614 rabbitizer-1.7.2/tables/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tools/c_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tools/pyi_table_gen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-05-04 19:19:15.000000 rabbitizer-1.7.2/tables/tools/rs_table_gen.sh
```

### Comparing `rabbitizer-1.7.1/LICENSE` & `rabbitizer-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/PKG-INFO` & `rabbitizer-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.1
+Version: 1.7.2
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.1/README.md` & `rabbitizer-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/analysis/RabbitizerLoPairingInfo.h` & `rabbitizer-1.7.2/include/analysis/RabbitizerLoPairingInfo.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_LO_PAIRING_INFO_H
 #define RABBITIZER_LO_PAIRING_INFO_H
 #pragma once
 
 #include <stdbool.h>
```

### Comparing `rabbitizer-1.7.1/include/analysis/RabbitizerRegistersTracker.h` & `rabbitizer-1.7.2/include/analysis/RabbitizerRegistersTracker.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_REGISTERS_TRACKER_H
 #define RABBITIZER_REGISTERS_TRACKER_H
 #pragma once
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/include/analysis/RabbitizerTrackedRegisterState.h` & `rabbitizer-1.7.2/include/analysis/RabbitizerTrackedRegisterState.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_TRACKED_REGISTER_STATE_H
 #define RABBITIZER_TRACKED_REGISTER_STATE_H
 #pragma once
 
 #include <stdbool.h>
```

### Comparing `rabbitizer-1.7.1/include/common/RabbitizerConfig.h` & `rabbitizer-1.7.2/include/common/RabbitizerConfig.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_CONFIG_H
 #define RABBITIZER_CONFIG_H
 
 #include <stdbool.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
-#include "Abi_enum.table.h"
+#include "generated/Abi_enum.h"
 
 RabbitizerAbi RabbitizerAbi_fromStr(const char *name);
 
 
 typedef struct RabbitizerConfig_RegisterNames {
     bool namedRegisters; // Enables using named registers. This option takes precedence over the other named register options
     RabbitizerAbi gprAbiNames; // The ABI names to be used for general purpose registers when disassembling the main processor's instructions
```

### Comparing `rabbitizer-1.7.1/include/common/RabbitizerVersion.h` & `rabbitizer-1.7.2/include/common/RabbitizerVersion.h`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extern "C" {
 #endif
 
 
 // Header version
 #define RAB_VERSION_MAJOR 1
 #define RAB_VERSION_MINOR 7
-#define RAB_VERSION_PATCH 1
+#define RAB_VERSION_PATCH 2
 
 #define RAB_VERSION_STR RAB_STRINGIFY(RAB_VERSION_MAJOR) "." RAB_STRINGIFY(RAB_VERSION_MINOR) "." RAB_STRINGIFY(RAB_VERSION_PATCH)
 
 // Compiled library version
 extern const int RabVersion_Major;
 extern const int RabVersion_Minor;
 extern const int RabVersion_Patch;
```

### Comparing `rabbitizer-1.7.1/include/common/Utils.h` & `rabbitizer-1.7.2/include/common/Utils.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_UTILS_H
 #define RABBITIZER_UTILS_H
 
 #include <stddef.h>
 #include <stdint.h>
```

### Comparing `rabbitizer-1.7.1/include/instructions/InstrId_enum.table.h` & `rabbitizer-1.7.2/include/generated/InstrId_enum.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef InstrId_enum_table_h_automatic
-#define InstrId_enum_table_h_automatic
+#ifndef InstrId_enum_h_automatic
+#define InstrId_enum_h_automatic
 
 typedef enum RabbitizerInstrId {
     RABBITIZER_INSTR_ID_cpu_INVALID,
     RABBITIZER_INSTR_ID_cpu_j,
     RABBITIZER_INSTR_ID_cpu_jal,
     RABBITIZER_INSTR_ID_cpu_beq,
     RABBITIZER_INSTR_ID_cpu_bne,
```

### Comparing `rabbitizer-1.7.1/include/instructions/InstrId_enum.table.template` & `rabbitizer-1.7.2/tables/templates/c/InstrId_enum.table.template`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...) \
     RABBITIZER_INSTR_ID_##prefix##_##name,
 
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 typedef enum RabbitizerInstrId {
-    #include "instructions/InstrIds.inc"
+    #include "InstrIds.inc"
 
     RABBITIZER_INSTR_ID_ALL_MAX = RABBITIZER_DEF_INSTR_ID(r5900, , MAX, )
 } RabbitizerInstrId;
 
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
```

### Comparing `rabbitizer-1.7.1/include/instructions/OperandType_enum.table.h` & `rabbitizer-1.7.2/include/generated/OperandType_enum.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef OperandType_enum_table_h_automatic
-#define OperandType_enum_table_h_automatic
+#ifndef OperandType_enum_h_automatic
+#define OperandType_enum_h_automatic
 
 typedef enum RabbitizerOperandType {
     RAB_OPERAND_ALL_INVALID,
     RAB_OPERAND_cpu_rs,
     RAB_OPERAND_cpu_rt,
     RAB_OPERAND_cpu_rd,
     RAB_OPERAND_cpu_sa,
```

### Comparing `rabbitizer-1.7.1/include/instructions/OperandType_function_declarations.table.h` & `rabbitizer-1.7.2/include/generated/OperandType_function_declarations.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef OperandType_function_declarations_table_h_automatic
-#define OperandType_function_declarations_table_h_automatic
+#ifndef OperandType_function_declarations_h_automatic
+#define OperandType_function_declarations_h_automatic
 
     size_t RabbitizerOperandType_process_cpu_rs (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_cpu_rt (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_cpu_rd (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_cpu_sa (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_cpu_zero (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
     size_t RabbitizerOperandType_process_cpu_cop0d (const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstrDescriptor.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstrDescriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRDESCRIPTOR_H
 #define RABBITIZER_INSTRDESCRIPTOR_H
 #pragma once
 
 #include <stdbool.h>
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstrId.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstrId.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRID_H
 #define RABBITIZER_INSTRID_H
 #pragma once
 
 #include <stdbool.h>
 
 #include "common/Utils.h"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-#include "InstrId_enum.table.h"
+#include "generated/InstrId_enum.h"
 
 extern const char *RabbitizerInstrId_Names[];
 
 
 CONST NODISCARD
 bool RabbitizerInstrId_isValid(RabbitizerInstrId uniqueId);
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstrSuffix.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstrSuffix.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRSUFFIX_H
 #define RABBITIZER_INSTRSUFFIX_H
 #pragma once
 
 #include "common/Utils.h"
@@ -10,15 +10,15 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
 struct RabbitizerInstruction;
 
-#include "InstrSuffix_enum.table.h"
+#include "generated/InstrSuffix_enum.h"
 
 CONST NODISCARD NON_NULL(1)
 size_t RabbitizerInstrSuffix_getSizeForBuffer(const struct RabbitizerInstruction *self, RabbitizerInstrSuffix instrSuffix);
 
 CONST NODISCARD NON_NULL(1, 2)
 size_t RabbitizerInstrSuffix_processSuffix(const struct RabbitizerInstruction *self, char *dst, RabbitizerInstrSuffix instrSuffix);
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstruction.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstruction.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRUCTION_H
 #define RABBITIZER_INSTRUCTION_H
 #pragma once
 
 #include <stdbool.h>
@@ -10,26 +10,28 @@
 #include <stdint.h>
 
 #include "common/Utils.h"
 
 #include "RabbitizerInstrId.h"
 #include "RabbitizerInstrDescriptor.h"
 #include "RabbitizerInstrCategory.h"
+#include "RabbitizerInstrIdType.h"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
 typedef struct RabbitizerInstruction {
     uint32_t word;
     uint32_t _mandatorybits;
 
     RabbitizerInstrId uniqueId;
     const RabbitizerInstrDescriptor *descriptor;
+    RabInstrIdType instrIdType;
 
     uint32_t vram;
     bool _handwrittenCategory;
     bool inHandwrittenFunction;
     RabbitizerInstrCategory category;
 } RabbitizerInstruction;
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR3000GTE.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstructionR3000GTE.h`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionR5900.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstructionR5900.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRUCTION_R5900_H
 #define RABBITIZER_INSTRUCTION_R5900_H
 #pragma once
 
 #include "RabbitizerInstruction.h"
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerInstructionRsp.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerInstructionRsp.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_INSTRUCTION_RSP_H
 #define RABBITIZER_INSTRUCTION_RSP_H
 #pragma once
 
 #include "RabbitizerInstruction.h"
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerOperandType.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerOperandType.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_OPERAND_TYPE_H
 #define RABBITIZER_OPERAND_TYPE_H
 #pragma once
 
 #include <stddef.h>
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-#include "OperandType_enum.table.h"
+#include "generated/OperandType_enum.h"
 
 struct RabbitizerInstruction;
 
 typedef size_t (*OperandCallback)(const struct RabbitizerInstruction *self, char *dst, const char *immOverride, size_t immOverrideLength);
 
 extern const OperandCallback instrOpercandCallbacks[];
 
-#include "OperandType_function_declarations.table.h"
+#include "generated/OperandType_function_declarations.h"
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerRegister.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerRegister.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_REGISTER_H
 #define RABBITIZER_REGISTER_H
 #pragma once
 
 #include <stdint.h>
@@ -12,15 +12,15 @@
 
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
-#include "Registers_enums.table.h"
+#include "generated/Registers_enums.h"
 
 extern const char *RabbitizerRegister_GprO32_Names[][2];
 extern const char *RabbitizerRegister_GprN32_Names[][2];
 extern const char *RabbitizerRegister_Cop0_Names[][2];
 extern const char *RabbitizerRegister_Cop1O32_Names[][2];
 extern const char *RabbitizerRegister_Cop1N32_Names[][2];
 extern const char *RabbitizerRegister_Cop1N64_Names[][2];
```

### Comparing `rabbitizer-1.7.1/include/instructions/RabbitizerRegisterDescriptor.h` & `rabbitizer-1.7.2/include/instructions/RabbitizerRegisterDescriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_REGISTERDESCRIPTOR_H
 #define RABBITIZER_REGISTERDESCRIPTOR_H
 #pragma once
 
 #include <stdbool.h>
```

### Comparing `rabbitizer-1.7.1/include/instructions/Registers_enums.table.h` & `rabbitizer-1.7.2/include/generated/Registers_enums.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef Registers_enums_table_h_automatic
-#define Registers_enums_table_h_automatic
+#ifndef Registers_enums_h_automatic
+#define Registers_enums_h_automatic
 
 typedef enum RabbitizerRegister_GprO32 {
     RABBITIZER_REG_GPR_O32_zero,
     RABBITIZER_REG_GPR_O32_at,
     RABBITIZER_REG_GPR_O32_v0,
     RABBITIZER_REG_GPR_O32_v1,
     RABBITIZER_REG_GPR_O32_a0,
```

### Comparing `rabbitizer-1.7.1/include/instructions/Registers_enums.table.template` & `rabbitizer-1.7.2/tables/templates/c/Registers_enums.table.template`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
     RABBITIZER_REG_##prefix##_##name,
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
     RABBITIZER_REG_##prefix##_##name,
```

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_cpu.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r3000gte.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_r3000gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_r5900.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/RabbitizerInstrId_rsp.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/RabbitizerInstrId_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_bc0.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0_bc0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop0_tlb.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_bc1.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_bc1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_d.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_d.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_l.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_l.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_s.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop1_fpu_w.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop1_fpu_w.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_cop2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_normal.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_regimm.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/cpu/cpu_special.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/cpu/cpu_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r3000gte/r3000gte_cop2_gte.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop0_tlb.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop0_tlb.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop1_fpu_s.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop1_fpu_s.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_bc2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_bc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special1.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_special1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_cop2_special2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_cop2_special2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_0.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_1.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_1.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_mmi_3.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_mmi_3.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_normal.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_regimm.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/r5900/r5900_special.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/r5900/r5900_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop0.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop0.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_cop2_vu.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_cop2_vu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_lwc2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal_lwc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_normal_swc2.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_normal_swc2.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_regimm.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_regimm.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/instr_id/rsp/rsp_special.inc` & `rabbitizer-1.7.2/tables/tables/instr_id/rsp/rsp_special.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_cpu.inc` & `rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_cpu.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_r5900.inc` & `rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_r5900.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/operands/RabbitizerOperandType_rsp.inc` & `rabbitizer-1.7.2/tables/tables/operands/RabbitizerOperandType_rsp.inc`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop0.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop0.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG_NODOLLAR(
         COP0, Index,       0,
         0
     )
     RABBITIZER_DEF_REG_NODOLLAR(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1Control.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1Control.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         COP1_CONTROL,      0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N32.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1N32.inc`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         COP1_N32, fv0,   f0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1N64.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1N64.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         COP1_N64, fv0,   f0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop1O32.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop1O32.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         COP1_O32, fv0,   f0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_Cop2.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_Cop2.inc`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         COP2,  0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprN32.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_GprN32.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         GPR_N32, zero,  0,
         .isZero=true
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_GprO32.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_GprO32.inc`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         GPR_O32, zero,  0,
         .isZero=true
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VF.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_R5900VF.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         R5900_VF,  vf0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_R5900VI.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_R5900VI.inc`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         R5900_VI,  vi0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop0.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop0.inc`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG_NODOLLAR(
         RSP_COP0, SP_MEM_ADDR,   0,
         0
     )
     RABBITIZER_DEF_REG_NODOLLAR(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop2.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         RSP_COP2,  0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspCop2Control.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspCop2Control.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         RSP_COP2_CONTROL,  0,  0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspGpr.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspGpr.inc`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         RSP_GPR, zero,  0,
         .isZero=true
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/instructions/registers/RabbitizerRegister_RspVector.inc` & `rabbitizer-1.7.2/tables/tables/registers/RabbitizerRegister_RspVector.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
     RABBITIZER_DEF_REG(
         RSP_VECTOR, v0,   0,
         0
     )
     RABBITIZER_DEF_REG(
```

### Comparing `rabbitizer-1.7.1/include/rabbitizer.h` & `rabbitizer-1.7.2/include/rabbitizer.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_H
 #define RABBITIZER_H
 #pragma once
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/pyproject.toml` & `rabbitizer-1.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 [project]
 name = "rabbitizer"
 # Version should be synced with include/common/RabbitizerVersion.h
-version = "1.7.1"
+version = "1.7.2"
 description = "MIPS instruction decoder"
 # license = "MIT"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
     { name="Anghelo Carvajal", email="angheloalf95@gmail.com" },
 ]
```

### Comparing `rabbitizer-1.7.1/rabbitizer/Config.pyi` & `rabbitizer-1.7.2/rabbitizer/Config.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from .Enum import Enum
 from .Abi import Abi
```

### Comparing `rabbitizer-1.7.1/rabbitizer/Enum.pyi` & `rabbitizer-1.7.2/rabbitizer/Enum.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 
 class Enum:
     name: str
```

### Comparing `rabbitizer-1.7.1/rabbitizer/InstrId.pyi` & `rabbitizer-1.7.2/rabbitizer/InstrId.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/OperandType.pyi` & `rabbitizer-1.7.2/rabbitizer/OperandType.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegCop1N32.pyi` & `rabbitizer-1.7.2/rabbitizer/RegCop1N32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegCop1N64.pyi` & `rabbitizer-1.7.2/rabbitizer/RegCop1N64.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegCop1O32.pyi` & `rabbitizer-1.7.2/rabbitizer/RegCop1O32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegGprN32.pyi` & `rabbitizer-1.7.2/rabbitizer/RegGprN32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegGprO32.pyi` & `rabbitizer-1.7.2/rabbitizer/RegGprO32.pyi`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/rabbitizer/RegistersTracker.pyi` & `rabbitizer-1.7.2/rabbitizer/RegistersTracker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# SPDX-FileCopyrightText: © 2022 Decompollaborate
+# SPDX-FileCopyrightText: © 2022-2023 Decompollaborate
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from .rabbitizer import Instruction
 from .LoPairingInfo import LoPairingInfo
```

### Comparing `rabbitizer-1.7.1/rabbitizer/__init__.pyi` & `rabbitizer-1.7.2/rabbitizer/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import annotations
 
 from .Utils import *
 
 from .Enum import *
 from .InstrCategory import *
 from .InstrId import *
+from .InstrIdType import *
 from .OperandType import *
 from .AccessType import *
 
 from .RegGprO32 import *
 from .RegGprN32 import *
 
 from .RegCop1O32 import *
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/enums_utils.c` & `rabbitizer-1.7.2/rabbitizer/enums/enums_utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 
 
 int rabbitizer_EnumMetadata_Initialize(PyObject *submodule, RabbitizerEnumMetadata *enumValues) {
     for (size_t i = 0; enumValues[i].enumType != 0; i++) {
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/enums_utils.h` & `rabbitizer-1.7.2/rabbitizer/enums/enums_utils.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #ifndef RABBITIZER_ENUMS_UTILS_H
 #define RABBITIZER_ENUMS_UTILS_H
 #pragma once
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_Abi.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_Abi.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 #include "common/RabbitizerConfig.h"
 #include "common/Utils.h"
 
 
 #define RABBITIZER_DEF_ABI(name) { "Abi", #name, RABBITIZER_ABI_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_Abi_enumvalues[] = {
-    #include "common/Abi.inc"
+    #include "tables/Abi.inc"
     RABBITIZER_DEF_ABI(MAX)
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_ABI
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_AccessType.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_AccessType.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 #include "instructions/RabbitizerAccessType.h"
 
 
 #define RAB_DEF_ACCESSTYPE(name) { "AccessType", #name , RAB_ACCESSTYPE_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_AccessType_enumvalues[] = {
-#include "instructions/AccessType.inc"
+#include "tables/AccessType.inc"
 
     RAB_DEF_ACCESSTYPE(MAX)
 
     { 0 },
 };
 
 #undef RAB_DEF_ACCESSTYPE
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrCategory.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_InstrCategory.c`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include "enums_utils.h"
 #include "instructions/RabbitizerInstruction.h"
 
 
 #define RABBITIZER_DEF_INSTR_CATEGORY(name) { "InstrCategory", #name, RABBITIZER_INSTRCAT_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_InstrCategory_enumvalues[] = {
-    #include "instructions/InstrCategory.inc"
+    #include "tables/InstrCategory.inc"
     RABBITIZER_DEF_INSTR_CATEGORY(MAX)
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_INSTR_CATEGORY
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_InstrId.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_InstrId.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums_utils.h"
 #include "instructions/RabbitizerInstrId.h"
 
 
 #define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...)                   { "InstrId", #prefix "_" #name, RABBITIZER_INSTR_ID_##prefix##_##name, false, NULL },
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...)  RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 RabbitizerEnumMetadata rabbitizer_enum_InstrId_enumvalues[] = {
-    #include "instructions/InstrIds.inc"
+    #include "tables/InstrIds.inc"
 
     RABBITIZER_DEF_INSTR_ID(ALL, , MAX, )
     { 0 },
 };
 
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_enum_OperandType.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_enum_OperandType.c`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 #define RAB_DEF_OPERAND(prefix, operand) { "OperandType", #prefix "_" #operand, RAB_OPERAND_##prefix##_##operand, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_OperandType_enumvalues[] = {
     RAB_DEF_OPERAND(ALL, INVALID)
 
-#include "instructions/OperandTypes.inc"
+#include "tables/OperandTypes.inc"
 
     RAB_DEF_OPERAND(ALL, MAX)
 
     { 0 },
 };
 
 #undef RAB_DEF_OPERAND
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/rabbitizer_type_Enum.c` & `rabbitizer-1.7.2/rabbitizer/enums/rabbitizer_type_Enum.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 #include "enums_utils.h"
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c` & `rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1N32.c`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
     { "RegCop1N32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
     { "RegCop1N32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_RegCop1N32_enumvalues[] = {
-    #include "instructions/registers/RabbitizerRegister_Cop1N32.inc"
+    #include "tables/registers/RabbitizerRegister_Cop1N32.inc"
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c` & `rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1N64.c`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
     { "RegCop1N64", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
     { "RegCop1N64", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_RegCop1N64_enumvalues[] = {
-    #include "instructions/registers/RabbitizerRegister_Cop1N64.inc"
+    #include "tables/registers/RabbitizerRegister_Cop1N64.inc"
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c` & `rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_Cop1O32.c`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
     { "RegCop1O32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
     { "RegCop1O32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 RabbitizerEnumMetadata rabbitizer_enum_RegCop1O32_enumvalues[] = {
-    #include "instructions/registers/RabbitizerRegister_Cop1O32.inc"
+    #include "tables/registers/RabbitizerRegister_Cop1O32.inc"
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c` & `rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums/enums_utils.h"
 #include "instructions/RabbitizerRegister.h"
 
 
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
-    { "RegGprN32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
+    { "RegGprO32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
-    { "RegGprN32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
+    { "RegGprO32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
-RabbitizerEnumMetadata rabbitizer_enum_RegGprN32_enumvalues[] = {
-    #include "instructions/registers/RabbitizerRegister_GprN32.inc"
+RabbitizerEnumMetadata rabbitizer_enum_RegGprO32_enumvalues[] = {
+    #include "tables/registers/RabbitizerRegister_GprO32.inc"
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
 
 
-static PyMethodDef rabbitizer_enum_RegGprN32_methods[] = {
+static PyMethodDef rabbitizer_enum_RegGprO32_methods[] = {
     { 0 },
 };
 
-DEF_ENUM(RegGprN32, "")
+DEF_ENUM(RegGprO32, "")
```

### Comparing `rabbitizer-1.7.1/rabbitizer/enums/registers/rabbitizer_enum_GprO32.c` & `rabbitizer-1.7.2/rabbitizer/enums/registers/rabbitizer_enum_GprN32.c`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "enums/enums_utils.h"
 #include "instructions/RabbitizerRegister.h"
 
 
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
-    { "RegGprO32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
+    { "RegGprN32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
-    { "RegGprO32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
+    { "RegGprN32", #name, RABBITIZER_REG_##prefix##_##name, false, NULL },
 
-RabbitizerEnumMetadata rabbitizer_enum_RegGprO32_enumvalues[] = {
-    #include "instructions/registers/RabbitizerRegister_GprO32.inc"
+RabbitizerEnumMetadata rabbitizer_enum_RegGprN32_enumvalues[] = {
+    #include "tables/registers/RabbitizerRegister_GprN32.inc"
 
     { 0 },
 };
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
 
 
-static PyMethodDef rabbitizer_enum_RegGprO32_methods[] = {
+static PyMethodDef rabbitizer_enum_RegGprN32_methods[] = {
     { 0 },
 };
 
-DEF_ENUM(RegGprO32, "")
+DEF_ENUM(RegGprN32, "")
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer.pyi` & `rabbitizer-1.7.2/rabbitizer/rabbitizer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,19 @@
     Read-only."""
 
     uniqueId: Enum
     """An unique identificator for the opcode of this instruction.
     The type is an `InstrId` enum.
     Read-only."""
 
+    instrIdType: Enum
+    """An identificator for the general type for the opcode of this instruction.
+    The type is an `InstrIdType` enum.
+    Read-only."""
+
     vram: int = 0
     """The vram (virtual ram) address for this instruction"""
     inHandwrittenFunction: bool = False
     """Boolean value indicating if the current instruction is used on a handwritten function. This is intended to be determined by the user."""
 
 
     def __init__(self, word: int, vram: int=0, category: Enum=InstrCategory.CPU) -> None: ...
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_global_config.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_global_config.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /**
  * Wrapper to expose rabbitizer's global configuration
  */
 
 #include "rabbitizer_module.h"
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_module.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_module.c`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     MODULE_ATTRIBUTE_GLOBAL(config),
 
     MODULE_ATTRIBUTE_TYPE(Enum),
     MODULE_ATTRIBUTE_ENUM(Abi),
     MODULE_ATTRIBUTE_ENUM(InstrCategory),
     MODULE_ATTRIBUTE_ENUM(InstrId),
+    MODULE_ATTRIBUTE_ENUM(InstrIdType),
     MODULE_ATTRIBUTE_ENUM(OperandType),
     MODULE_ATTRIBUTE_ENUM(AccessType),
 
     MODULE_ATTRIBUTE_ENUM(RegGprO32),
     MODULE_ATTRIBUTE_ENUM(RegGprN32),
     MODULE_ATTRIBUTE_ENUM(RegCop1O32),
     MODULE_ATTRIBUTE_ENUM(RegCop1N32),
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_module.h` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_module.h`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 extern PyTypeObject rabbitizer_type_LoPairingInfo_TypeObject;
 extern PyTypeObject rabbitizer_type_TrackedRegisterState_TypeObject;
 extern PyTypeObject rabbitizer_type_RegistersTracker_TypeObject;
 
 DECL_ENUM(Abi)
 DECL_ENUM(InstrCategory)
 DECL_ENUM(InstrId)
+DECL_ENUM(InstrIdType)
 DECL_ENUM(OperandType)
 DECL_ENUM(AccessType)
 
 DECL_ENUM(RegGprO32)
 DECL_ENUM(RegGprN32)
 
 DECL_ENUM(RegCop1O32)
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_submodule_Utils.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_submodule_Utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_Instruction.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_type_Instruction.c`

 * *Files 1% similar despite different names*

```diff
@@ -185,28 +185,41 @@
         return NULL;
     }
 
     Py_INCREF(enumInstance);
     return enumInstance;
 }
 
+static PyObject *rabbitizer_type_Instruction_member_get_instrIdType(PyRabbitizerInstruction *self, UNUSED PyObject *closure) {
+    PyObject *enumInstance = rabbitizer_enum_InstrIdType_enumvalues[self->instr.instrIdType].instance;
+
+    if (enumInstance == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "Internal error: invalid instrIdType enum value");
+        return NULL;
+    }
+
+    Py_INCREF(enumInstance);
+    return enumInstance;
+}
+
 #define MEMBER_GET(name, docs, closure)      { #name, (getter) rabbitizer_type_Instruction_member_get_##name, (setter) NULL,                                          PyDoc_STR(docs), closure }
 #define MEMBER_SET(name, docs, closure)      { #name, (getter) NULL,                                          (setter) rabbitizer_type_Instruction_member_set_##name, PyDoc_STR(docs), closure }
 #define MEMBER_GET_SET(name, docs, closure)  { #name, (getter) rabbitizer_type_Instruction_member_get_##name, (setter) rabbitizer_type_Instruction_member_set_##name, PyDoc_STR(docs), closure }
 
 
 static PyGetSetDef rabbitizer_type_Instruction_getsetters[] = {
     MEMBER_GET(rs, "", NULL),
     MEMBER_GET(rt, "", NULL),
     MEMBER_GET(rd, "", NULL),
     MEMBER_GET(sa, "", NULL),
     MEMBER_GET(fs, "", NULL),
     MEMBER_GET(ft, "", NULL),
     MEMBER_GET(fd, "", NULL),
     MEMBER_GET(uniqueId, "", NULL),
+    MEMBER_GET(instrIdType, "", NULL),
 
     { 0 }
 };
 
 
 #define DEF_METHOD_GET_UINT(name) \
     static PyObject *rabbitizer_type_Instruction_##name(PyRabbitizerInstruction *self, UNUSED PyObject *closure) { \
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_LoPairingInfo.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_type_LoPairingInfo.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 
 static void rabbitizer_type_LoPairingInfo_dealloc(PyRabbitizerLoPairingInfo *self) {
     Py_TYPE(self)->tp_free((PyObject *) self);
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_RegistersTracker.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_type_RegistersTracker.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 #include "analysis/RabbitizerRegistersTracker.h"
```

### Comparing `rabbitizer-1.7.1/rabbitizer/rabbitizer_type_TrackedRegisterState.c` & `rabbitizer-1.7.2/rabbitizer/rabbitizer_type_TrackedRegisterState.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "rabbitizer_module.h"
 
 
 static void rabbitizer_type_TrackedRegisterState_dealloc(PyRabbitizerTrackedRegisterState *self) {
     RabbitizerTrackedRegisterState_destroy(&self->registerState);
```

### Comparing `rabbitizer-1.7.1/rabbitizer.egg-info/PKG-INFO` & `rabbitizer-1.7.2/rabbitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitizer
-Version: 1.7.1
+Version: 1.7.2
 Summary: MIPS instruction decoder
 Author-email: Anghelo Carvajal <angheloalf95@gmail.com>
 Project-URL: Homepage, https://github.com/Decompollaborate/rabbitizer
 Project-URL: Bug Tracker, https://github.com/Decompollaborate/rabbitizer/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rabbitizer-1.7.1/setup.py` & `rabbitizer-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,12 +18,12 @@
     extraCompileArgs += ["-Werror"]
 
 setup(
     ext_modules=[
         Extension(
             name="rabbitizer",
             sources=sourcesList,
-            include_dirs=["include", "rabbitizer"],
+            include_dirs=["include", "rabbitizer", "tables"],
             extra_compile_args = extraCompileArgs,
         ),
     ],
 )
```

### Comparing `rabbitizer-1.7.1/src/analysis/RabbitizerRegistersTracker.c` & `rabbitizer-1.7.2/src/analysis/RabbitizerRegistersTracker.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "analysis/RabbitizerRegistersTracker.h"
 
 #include <assert.h>
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/src/analysis/RabbitizerTrackedRegisterState.c` & `rabbitizer-1.7.2/src/analysis/RabbitizerTrackedRegisterState.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "analysis/RabbitizerTrackedRegisterState.h"
 
 #include <assert.h>
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/src/common/RabbitizerConfig.c` & `rabbitizer-1.7.2/src/common/RabbitizerConfig.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "common/RabbitizerConfig.h"
 
 #include <string.h>
 
 RabbitizerAbi RabbitizerAbi_fromStr(const char *name) {
```

### Comparing `rabbitizer-1.7.1/src/common/Utils.c` & `rabbitizer-1.7.2/src/common/Utils.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "common/Utils.h"
 
 #include <stdbool.h>
 #include <string.h>
```

### Comparing `rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.h` & `rabbitizer-1.7.2/include/generated/InstrDescriptor_Descriptors_array.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef InstrDescriptor_Descriptors_array_table_h_automatic
-#define InstrDescriptor_Descriptors_array_table_h_automatic
+#ifndef InstrDescriptor_Descriptors_array_h_automatic
+#define InstrDescriptor_Descriptors_array_h_automatic
 
 const RabbitizerInstrDescriptor RabbitizerInstrDescriptor_Descriptors[] = {
     [RABBITIZER_INSTR_ID_cpu_INVALID] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_immediate} },
     [RABBITIZER_INSTR_ID_cpu_j] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true },
     [RABBITIZER_INSTR_ID_cpu_jal] = { .operands={RAB_OPERAND_cpu_label}, .instrType=RABBITIZER_INSTR_TYPE_J, .isJump=true, .isJumpWithAddress=true, .doesLink=true },
     [RABBITIZER_INSTR_ID_cpu_beq] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
     [RABBITIZER_INSTR_ID_cpu_bne] = { .operands={RAB_OPERAND_cpu_rs, RAB_OPERAND_cpu_rt, RAB_OPERAND_cpu_branch_target_label}, .instrType=RABBITIZER_INSTR_TYPE_I, .isBranch=true, .readsRs=true, .readsRt=true },
```

### Comparing `rabbitizer-1.7.1/src/instructions/InstrDescriptor_Descriptors_array.table.template` & `rabbitizer-1.7.2/tables/templates/c/InstrDescriptor_Descriptors_array.table.template`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...) [RABBITIZER_INSTR_ID_##prefix##_##name] = { __VA_ARGS__ },
 
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 const RabbitizerInstrDescriptor RabbitizerInstrDescriptor_Descriptors[] = {
-    #include "instructions/InstrIds.inc"
+    #include "InstrIds.inc"
 };
 
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
```

### Comparing `rabbitizer-1.7.1/src/instructions/InstrId_Names_array.table.h` & `rabbitizer-1.7.2/include/generated/InstrId_Names_array.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef InstrId_Names_array_table_h_automatic
-#define InstrId_Names_array_table_h_automatic
+#ifndef InstrId_Names_array_h_automatic
+#define InstrId_Names_array_h_automatic
 
 const char *RabbitizerInstrId_Names[] = {
     [RABBITIZER_INSTR_ID_cpu_INVALID] = "INVALID",
     [RABBITIZER_INSTR_ID_cpu_j] = "j",
     [RABBITIZER_INSTR_ID_cpu_jal] = "jal",
     [RABBITIZER_INSTR_ID_cpu_beq] = "beq",
     [RABBITIZER_INSTR_ID_cpu_bne] = "bne",
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstrCategory.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstrCategory.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstrCategory.h"
 
 #include <string.h>
 
-#include "InstrCategory_Names_array.table.h"
+#include "generated/InstrCategory_Names_array.h"
 
 RabbitizerInstrCategory RabbitizerInstrCategory_fromStr(const char *name) {
     if (name == NULL) {
         return (RabbitizerInstrCategory)-2;
     }
 
     for (RabbitizerInstrCategory i = 0; i < RABBITIZER_INSTRCAT_MAX; i++) {
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstrDescriptor.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstrDescriptor.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstrDescriptor.h"
 
 #include <assert.h>
 
 #include "instructions/RabbitizerInstruction.h"
 
-#include "InstrDescriptor_Descriptors_array.table.h"
+#include "generated/InstrDescriptor_Descriptors_array.h"
 
 bool RabbitizerInstrDescriptor_hasSpecificOperand(const RabbitizerInstrDescriptor *self,
                                                   RabbitizerOperandType operand) {
     size_t i;
 
     for (i = 0; i < ARRAY_COUNT(self->operands) && self->operands[i] != RAB_OPERAND_ALL_INVALID; i++) {
         if (self->operands[i] == operand) {
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstrId.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstrId.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstrId.h"
 
 #include <assert.h>
 
-#include "InstrId_Names_array.table.h"
+#include "generated/InstrId_Names_array.h"
 
 bool RabbitizerInstrId_isValid(RabbitizerInstrId uniqueId) {
     switch (uniqueId) {
         case RABBITIZER_INSTR_ID_cpu_INVALID:
         case RABBITIZER_INSTR_ID_rsp_INVALID:
         case RABBITIZER_INSTR_ID_r3000gte_INVALID:
         case RABBITIZER_INSTR_ID_r5900_INVALID:
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstrSuffix.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstrSuffix.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstrSuffix.h"
 
 #include <assert.h>
 
 #include "common/Utils.h"
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include <assert.h>
 
 #include "common/RabbitizerConfig.h"
@@ -13,14 +13,15 @@
 
 void RabbitizerInstruction_init(RabbitizerInstruction *self, uint32_t word, uint32_t vram) {
     self->word = word;
     self->_mandatorybits = 0;
 
     self->uniqueId = RABBITIZER_INSTR_ID_cpu_INVALID;
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
+    self->instrIdType = RAB_INSTR_ID_TYPE_ALL_INVALID;
 
     self->vram = vram;
     self->_handwrittenCategory = false;
     self->inHandwrittenFunction = false;
     self->category = RABBITIZER_INSTRCAT_CPU;
 }
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Disassemble.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include <assert.h>
 #include <string.h>
 #include <stdio.h>
@@ -171,14 +171,16 @@
             RABUTILS_BUFFER_ADVANCE(
                 dst, totalSize,
                 RabbitizerInstruction_disassembleInstruction(self, dst, immOverride, immOverrideLength, extraLJust));
 
             validBits = RabbitizerInstruction_getValidBits(self);
 
             RABUTILS_BUFFER_SPRINTF(dst, totalSize, " # %08X", ((~validBits) & self->word));
+
+            RABUTILS_BUFFER_SPRINTF(dst, totalSize, " <InstrIdType: %s>", RabInstrIdType_getName(self->instrIdType));
         }
 
         return totalSize;
     }
 
     return RabbitizerInstruction_disassembleInstruction(self, dst, immOverride, immOverrideLength, extraLJust);
 }
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Examination.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include <assert.h>
 
 #include "common/RabbitizerConfig.h"
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_Operand.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include <assert.h>
 
-#include "instrOpercandCallbacks_array.table.h"
+#include "generated/instrOpercandCallbacks_array.h"
 
 size_t RabbitizerOperandType_getBufferSize(RabbitizerOperandType operand, const RabbitizerInstruction *instr,
                                            size_t immOverrideLength) {
     char auxBuffer[0x100] = { 0 };
     char immOverride[0x100] = { 0 };
     OperandCallback callback;
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstruction/RabbitizerInstruction_ProcessUniqueId.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include "common/RabbitizerConfig.h"
 #include "instructions/RabbitizerRegister.h"
 
@@ -13,17 +13,18 @@
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 void RabbitizerInstruction_processUniqueId_Normal(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_NORMAL;
 
     switch (opcode) {
-#include "instructions/instr_id/cpu/cpu_normal.inc"
+#include "tables/instr_id/cpu/cpu_normal.inc"
     }
 
     if (RabbitizerConfig_Cfg.pseudos.enablePseudos) {
         switch (self->uniqueId) {
             case RABBITIZER_INSTR_ID_cpu_beq:
                 if (RAB_INSTR_GET_rt(self) == 0) {
                     if (RAB_INSTR_GET_rs(self) == 0) {
@@ -54,17 +55,18 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstruction_processUniqueId_Special(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_SPECIAL;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_special.inc"
+#include "tables/instr_id/cpu/cpu_special.inc"
     }
 
     if (RabbitizerInstruction_isNop(self)) {
         // NOP is special enough
         self->uniqueId = RABBITIZER_INSTR_ID_cpu_nop;
     } else if (RabbitizerConfig_Cfg.pseudos.enablePseudos) {
         switch (self->uniqueId) {
@@ -119,17 +121,18 @@
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Regimm(RabbitizerInstruction *self) {
     uint32_t rt = RAB_INSTR_GET_rt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_rt(self->_mandatorybits, rt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_REGIMM;
 
     switch (rt) {
-#include "instructions/instr_id/cpu/cpu_regimm.inc"
+#include "tables/instr_id/cpu/cpu_regimm.inc"
     }
 
     if (RabbitizerConfig_Cfg.pseudos.enablePseudos) {
         switch (self->uniqueId) {
             case RABBITIZER_INSTR_ID_cpu_bgezal:
                 if (RAB_INSTR_GET_rs(self) == 0) {
                     if (RabbitizerConfig_Cfg.pseudos.pseudoBal) {
@@ -146,38 +149,41 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor0_BC0(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_bc_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_bc_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP0_BC0;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop0_bc0.inc"
+#include "tables/instr_id/cpu/cpu_cop0_bc0.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor0_Tlb(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP0_TLB;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_cop0_tlb.inc"
+#include "tables/instr_id/cpu/cpu_cop0_tlb.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor0(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP0;
     self->_handwrittenCategory = true;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop0.inc"
+#include "tables/instr_id/cpu/cpu_cop0.inc"
 
         case 0x08:
             RabbitizerInstruction_processUniqueId_Coprocessor0_BC0(self);
             break;
 
         case 0x10:
             RabbitizerInstruction_processUniqueId_Coprocessor0_Tlb(self);
@@ -187,67 +193,73 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1_BC1(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_bc_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_bc_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1_BC1;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop1_bc1.inc"
+#include "tables/instr_id/cpu/cpu_cop1_bc1.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1_FpuS(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1_FPUS;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_cop1_fpu_s.inc"
+#include "tables/instr_id/cpu/cpu_cop1_fpu_s.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1_FpuD(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1_FPUD;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_cop1_fpu_d.inc"
+#include "tables/instr_id/cpu/cpu_cop1_fpu_d.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1_FpuW(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1_FPUW;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_cop1_fpu_w.inc"
+#include "tables/instr_id/cpu/cpu_cop1_fpu_w.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1_FpuL(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1_FPUL;
 
     switch (function) {
-#include "instructions/instr_id/cpu/cpu_cop1_fpu_l.inc"
+#include "tables/instr_id/cpu/cpu_cop1_fpu_l.inc"
     }
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor1(RabbitizerInstruction *self) {
     uint8_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP1;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop1.inc"
+#include "tables/instr_id/cpu/cpu_cop1.inc"
 
         case 0x08: // fmt = BC
             RabbitizerInstruction_processUniqueId_Coprocessor1_BC1(self);
             break;
 
         case 0x10:
             RabbitizerInstruction_processUniqueId_Coprocessor1_FpuS(self);
@@ -269,19 +281,20 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor2(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_COP2;
 
     self->_handwrittenCategory = true;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop2.inc"
+#include "tables/instr_id/cpu/cpu_cop2.inc"
 
         default:
             break;
     }
 
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
@@ -291,14 +304,15 @@
 
 void RabbitizerInstruction_processUniqueId(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
 
     self->uniqueId = RABBITIZER_INSTR_ID_cpu_INVALID;
+    self->instrIdType = RAB_INSTR_ID_TYPE_CPU_INVALID;
 
     switch (opcode) {
         default:
             RabbitizerInstruction_processUniqueId_Normal(self);
             break;
         case 0x00:
             RabbitizerInstruction_processUniqueId_Special(self);
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstruction/instrOpercandCallbacks_array.table.h` & `rabbitizer-1.7.2/include/generated/instrOpercandCallbacks_array.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef instrOpercandCallbacks_array_table_h_automatic
-#define instrOpercandCallbacks_array_table_h_automatic
+#ifndef instrOpercandCallbacks_array_h_automatic
+#define instrOpercandCallbacks_array_h_automatic
 
 const OperandCallback instrOpercandCallbacks[] = {
     [RAB_OPERAND_cpu_rs] = RabbitizerOperandType_process_cpu_rs,
     [RAB_OPERAND_cpu_rt] = RabbitizerOperandType_process_cpu_rt,
     [RAB_OPERAND_cpu_rd] = RabbitizerOperandType_process_cpu_rd,
     [RAB_OPERAND_cpu_sa] = RabbitizerOperandType_process_cpu_sa,
     [RAB_OPERAND_cpu_zero] = RabbitizerOperandType_process_cpu_zero,
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionCpu/RabbitizerInstructionCpu_OperandType.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstruction.h"
 
 #include <assert.h>
 #include <string.h>
 #include <stdio.h>
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_OperandType.c`

 * *Files identical despite different names*

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR3000GTE/RabbitizerInstructionR3000GTE_ProcessUniqueId.c`

 * *Files 10% similar despite different names*

```diff
@@ -9,57 +9,69 @@
     case (caseBits):                                            \
         self->uniqueId = RABBITIZER_INSTR_ID_##prefix##_##name; \
         break;
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Normal(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_NORMAL;
+
     RabbitizerInstruction_processUniqueId_Normal(self);
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Special(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_SPECIAL;
+
     RabbitizerInstruction_processUniqueId_Special(self);
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Regimm(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_REGIMM;
+
     RabbitizerInstruction_processUniqueId_Regimm(self);
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Coprocessor0(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_COP0;
+
     RabbitizerInstruction_processUniqueId_Coprocessor0(self);
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Coprocessor1(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_COP1;
+
     RabbitizerInstruction_processUniqueId_Coprocessor1(self);
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Coprocessor2_gte(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_COP2_GTE;
 
     // GTE instructions are weird
     self->_mandatorybits =
         RAB_INSTR_R3000GTE_PACK_FAKE_OPCODE(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_FAKE_OPCODE(self));
     self->_mandatorybits = RAB_INSTR_R3000GTE_PACK_sf(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_sf(self));
     self->_mandatorybits = RAB_INSTR_R3000GTE_PACK_mx(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_mx(self));
     self->_mandatorybits = RAB_INSTR_R3000GTE_PACK_v(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_v(self));
     self->_mandatorybits = RAB_INSTR_R3000GTE_PACK_cv(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_cv(self));
     self->_mandatorybits = RAB_INSTR_R3000GTE_PACK_lm(self->_mandatorybits, RAB_INSTR_R3000GTE_GET_lm(self));
 
     switch (function) {
-#include "instructions/instr_id/r3000gte/r3000gte_cop2_gte.inc"
+#include "tables/instr_id/r3000gte/r3000gte_cop2_gte.inc"
     }
 }
 
 void RabbitizerInstructionR3000GTE_processUniqueId_Coprocessor2(RabbitizerInstruction *self) {
     uint8_t fmt = RAB_INSTR_GET_fmt(self);
     bool fetchDescriptor = true;
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_COP2;
 
     switch (fmt) {
         case 0x10:
         case 0x11:
         case 0x12:
         case 0x13:
         case 0x14:
@@ -89,14 +101,15 @@
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
 
 void RabbitizerInstructionR3000GTE_processUniqueId(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R3000GTE_INVALID;
 
     switch (opcode) {
         default:
             RabbitizerInstructionR3000GTE_processUniqueId_Normal(self);
             break;
         case 0x00:
             RabbitizerInstructionR3000GTE_processUniqueId_Special(self);
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionR5900.h"
 
 void RabbitizerInstructionR5900_init(RabbitizerInstruction *self, uint32_t word, uint32_t vram) {
     RabbitizerInstruction_init(self, word, vram);
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_OperandType.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionR5900.h"
 
 #include <assert.h>
 #include <string.h>
 #include <stdio.h>
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionR5900/RabbitizerInstructionR5900_ProcessUniqueId.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionR5900.h"
 #include "common/RabbitizerConfig.h"
 
 #define RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, ...)    \
     case (caseBits):                                            \
@@ -12,17 +12,18 @@
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 void RabbitizerInstructionR5900_processUniqueId_Normal(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
     bool fetchDescriptor = true;
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_NORMAL;
 
     switch (opcode) {
-#include "instructions/instr_id/r5900/r5900_normal.inc"
+#include "tables/instr_id/r5900/r5900_normal.inc"
 
         default:
             RabbitizerInstruction_processUniqueId_Normal(self);
             fetchDescriptor = false;
             break;
     }
 
@@ -33,17 +34,18 @@
 
 void RabbitizerInstructionR5900_processUniqueId_Special(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
     bool fetchDescriptor = true;
     uint32_t stype;
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_SPECIAL;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_special.inc"
+#include "tables/instr_id/r5900/r5900_special.inc"
 
         default:
             RabbitizerInstruction_processUniqueId_Special(self);
             fetchDescriptor = false;
             break;
     }
 
@@ -67,17 +69,18 @@
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Regimm(RabbitizerInstruction *self) {
     uint32_t rt = RAB_INSTR_GET_rt(self);
     bool fetchDescriptor = true;
 
     self->_mandatorybits = RAB_INSTR_PACK_rt(self->_mandatorybits, rt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_REGIMM;
 
     switch (rt) {
-#include "instructions/instr_id/r5900/r5900_regimm.inc"
+#include "tables/instr_id/r5900/r5900_regimm.inc"
 
         default:
             RabbitizerInstruction_processUniqueId_Regimm(self);
             fetchDescriptor = false;
             break;
     }
 
@@ -86,32 +89,34 @@
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor0_Tlb(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP0_TLB;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_cop0_tlb.inc"
+#include "tables/instr_id/r5900/r5900_cop0_tlb.inc"
 
         default:
             RabbitizerInstruction_processUniqueId_Coprocessor0_Tlb(self);
             break;
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor0(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP0;
     self->_handwrittenCategory = true;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop0.inc"
+#include "tables/instr_id/cpu/cpu_cop0.inc"
 
         case 0x08:
             RabbitizerInstruction_processUniqueId_Coprocessor0_BC0(self);
             break;
 
         case 0x10:
             RabbitizerInstructionR5900_processUniqueId_Coprocessor0_Tlb(self);
@@ -121,31 +126,33 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor1_FpuS(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP1_FPUS;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_cop1_fpu_s.inc"
+#include "tables/instr_id/r5900/r5900_cop1_fpu_s.inc"
 
         default:
             RabbitizerInstruction_processUniqueId_Coprocessor1_FpuS(self);
             break;
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor1(RabbitizerInstruction *self) {
     uint8_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP1;
 
     switch (fmt) {
-#include "instructions/instr_id/cpu/cpu_cop1.inc"
+#include "tables/instr_id/cpu/cpu_cop1.inc"
 
         case 0x08: // fmt = BC
             RabbitizerInstruction_processUniqueId_Coprocessor1_BC1(self);
             break;
 
         case 0x10:
             RabbitizerInstructionR5900_processUniqueId_Coprocessor1_FpuS(self);
@@ -159,54 +166,58 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstruction_processUniqueId_Coprocessor2_BC2(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_bc_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_bc_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP2_BC2;
 
     switch (fmt) {
-#include "instructions/instr_id/r5900/r5900_cop2_bc2.inc"
+#include "tables/instr_id/r5900/r5900_cop2_bc2.inc"
     }
 }
 
-void RabbitizerInstructionR5900_processUniqueId_Coprocessor2_Special2(UNUSED RabbitizerInstruction *self) {
+void RabbitizerInstructionR5900_processUniqueId_Coprocessor2_Special2(RabbitizerInstruction *self) {
     uint32_t fhiflo = RAB_INSTR_R5900_GET_fhi_flo(self);
 
     self->_mandatorybits = RAB_INSTR_R5900_PACK_fhi_flo(self->_mandatorybits, fhiflo);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP2_SPECIAL2;
 
     switch (fhiflo) {
-#include "instructions/instr_id/r5900/r5900_cop2_special2.inc"
+#include "tables/instr_id/r5900/r5900_cop2_special2.inc"
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor2_Special1(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP2_SPECIAL1;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_cop2_special1.inc"
+#include "tables/instr_id/r5900/r5900_cop2_special1.inc"
 
         case 0x3C:
         case 0x3D:
         case 0x3E:
         case 0x3F:
             RabbitizerInstructionR5900_processUniqueId_Coprocessor2_Special2(self);
             break;
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_Coprocessor2(RabbitizerInstruction *self) {
     uint8_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_COP2;
 
     switch (fmt) {
-#include "instructions/instr_id/r5900/r5900_cop2.inc"
+#include "tables/instr_id/r5900/r5900_cop2.inc"
 
         case 0x08:
             RabbitizerInstruction_processUniqueId_Coprocessor2_BC2(self);
             break;
 
         case 0x10:
         case 0x11:
@@ -231,57 +242,62 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstructionR5900_processUniqueId_MMI_0(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_R5900_GET_mmi_function(self);
 
     self->_mandatorybits = RAB_INSTR_R5900_PACK_mmi_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_MMI_0;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_mmi_0.inc"
+#include "tables/instr_id/r5900/r5900_mmi_0.inc"
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_MMI_1(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_R5900_GET_mmi_function(self);
 
     self->_mandatorybits = RAB_INSTR_R5900_PACK_mmi_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_MMI_1;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_mmi_1.inc"
+#include "tables/instr_id/r5900/r5900_mmi_1.inc"
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_MMI_2(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_R5900_GET_mmi_function(self);
 
     self->_mandatorybits = RAB_INSTR_R5900_PACK_mmi_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_MMI_2;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_mmi_2.inc"
+#include "tables/instr_id/r5900/r5900_mmi_2.inc"
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_MMI_3(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_R5900_GET_mmi_function(self);
 
     self->_mandatorybits = RAB_INSTR_R5900_PACK_mmi_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_MMI_3;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_mmi_3.inc"
+#include "tables/instr_id/r5900/r5900_mmi_3.inc"
     }
 }
 
 void RabbitizerInstructionR5900_processUniqueId_MMI(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_MMI;
 
     switch (function) {
-#include "instructions/instr_id/r5900/r5900_mmi.inc"
+#include "tables/instr_id/r5900/r5900_mmi.inc"
 
         case 0x08:
             RabbitizerInstructionR5900_processUniqueId_MMI_0(self);
             break;
         case 0x09:
             RabbitizerInstructionR5900_processUniqueId_MMI_2(self);
             break;
@@ -299,14 +315,15 @@
 #undef RABBITIZER_DEF_INSTR_ID
 #undef RABBITIZER_DEF_INSTR_ID_ALTNAME
 
 void RabbitizerInstructionR5900_processUniqueId(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
+    self->instrIdType = RAB_INSTR_ID_TYPE_R5900_INVALID;
 
     switch (opcode) {
         default:
             RabbitizerInstructionR5900_processUniqueId_Normal(self);
             break;
         case 0x00:
             RabbitizerInstructionR5900_processUniqueId_Special(self);
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionRsp.h"
 
 void RabbitizerInstructionRsp_init(RabbitizerInstruction *self, uint32_t word, uint32_t vram) {
     RabbitizerInstruction_init(self, word, vram);
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_OperandType.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionRsp.h"
 
 #include <assert.h>
 #include <string.h>
 #include <stdio.h>
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerInstructionRsp/RabbitizerInstructionRsp_ProcessUniqueId.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerInstructionRsp.h"
 
 #include "common/RabbitizerConfig.h"
 #include "instructions/RabbitizerRegister.h"
 
@@ -13,28 +13,30 @@
 #define RABBITIZER_DEF_INSTR_ID_ALTNAME(prefix, caseBits, name, altname, ...) \
     RABBITIZER_DEF_INSTR_ID(prefix, caseBits, name, __VA_ARGS__)
 
 void RabbitizerInstructionRsp_processUniqueId_Normal_Lwc2(RabbitizerInstruction *self) {
     uint32_t rd = RAB_INSTR_GET_rd(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_rd(self->_mandatorybits, rd);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_NORMAL_LWC2;
 
     switch (rd) {
-#include "instructions/instr_id/rsp/rsp_normal_lwc2.inc"
+#include "tables/instr_id/rsp/rsp_normal_lwc2.inc"
     }
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Normal_Swc2(RabbitizerInstruction *self) {
     uint32_t rd = RAB_INSTR_GET_rd(self);
     uint32_t elementlow;
 
     self->_mandatorybits = RAB_INSTR_PACK_rd(self->_mandatorybits, rd);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_NORMAL_SWC2;
 
     switch (rd) {
-#include "instructions/instr_id/rsp/rsp_normal_swc2.inc"
+#include "tables/instr_id/rsp/rsp_normal_swc2.inc"
     }
 
     switch (self->uniqueId) {
         case RABBITIZER_INSTR_ID_rsp_suv:
             elementlow = RAB_INSTR_RSP_GET_elementlow(self);
             self->_mandatorybits = RAB_INSTR_RSP_PACK_elementlow(self->_mandatorybits, elementlow);
             if (elementlow != 0) {
@@ -47,17 +49,18 @@
     }
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Normal(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_NORMAL;
 
     switch (opcode) {
-#include "instructions/instr_id/rsp/rsp_normal.inc"
+#include "tables/instr_id/rsp/rsp_normal.inc"
 
         // new rsp stuff
         case 0x32:
             RabbitizerInstructionRsp_processUniqueId_Normal_Lwc2(self);
             break;
 
         case 0x3A:
@@ -88,17 +91,18 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Special(RabbitizerInstruction *self) {
     uint32_t function = RAB_INSTR_GET_function(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_SPECIAL;
 
     switch (function) {
-#include "instructions/instr_id/rsp/rsp_special.inc"
+#include "tables/instr_id/rsp/rsp_special.inc"
     }
 
     if (RabbitizerInstruction_isNop(self)) {
         // NOP is special enough
         self->uniqueId = RABBITIZER_INSTR_ID_rsp_nop;
     } else if (RabbitizerConfig_Cfg.pseudos.enablePseudos) {
         if (RAB_INSTR_GET_rt(self) == 0) {
@@ -123,17 +127,18 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Regimm(RabbitizerInstruction *self) {
     uint32_t rt = RAB_INSTR_GET_rt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_rt(self->_mandatorybits, rt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_REGIMM;
 
     switch (rt) {
-#include "instructions/instr_id/rsp/rsp_regimm.inc"
+#include "tables/instr_id/rsp/rsp_regimm.inc"
     }
 
     if (RabbitizerConfig_Cfg.pseudos.enablePseudos) {
         switch (self->uniqueId) {
             case RABBITIZER_INSTR_ID_rsp_bgezal:
                 if (RAB_INSTR_GET_rs(self) == 0) {
                     if (RabbitizerConfig_Cfg.pseudos.pseudoBal) {
@@ -150,46 +155,56 @@
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Coprocessor0(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_COP0;
 
     switch (fmt) {
-#include "instructions/instr_id/rsp/rsp_cop0.inc"
+#include "tables/instr_id/rsp/rsp_cop0.inc"
     }
 
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
 }
 
+void RabbitizerInstructionRsp_processUniqueId_Coprocessor1(RabbitizerInstruction *self) {
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_COP1;
+
+    self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
+}
+
 void RabbitizerInstructionRsp_processUniqueId_Coprocessor2_Vu(RabbitizerInstruction *self) {
     uint32_t aux = SHIFTR(self->word, 25, 1);
     uint32_t function = RAB_INSTR_GET_function(self);
 
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_COP2_VU;
+
     if (aux != 1) {
         return;
     }
 
     // TODO: name this bit range
     self->_mandatorybits = BITREPACK(self->_mandatorybits, aux, 25, 1);
     self->_mandatorybits = RAB_INSTR_PACK_function(self->_mandatorybits, function);
 
     switch (function) {
-#include "instructions/instr_id/rsp/rsp_cop2_vu.inc"
+#include "tables/instr_id/rsp/rsp_cop2_vu.inc"
     }
 }
 
 void RabbitizerInstructionRsp_processUniqueId_Coprocessor2(RabbitizerInstruction *self) {
     uint32_t fmt = RAB_INSTR_GET_fmt(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_fmt(self->_mandatorybits, fmt);
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_COP2;
 
     switch (fmt) {
-#include "instructions/instr_id/rsp/rsp_cop2.inc"
+#include "tables/instr_id/rsp/rsp_cop2.inc"
 
         default:
             RabbitizerInstructionRsp_processUniqueId_Coprocessor2_Vu(self);
             break;
     }
 
     self->descriptor = &RabbitizerInstrDescriptor_Descriptors[self->uniqueId];
@@ -200,29 +215,30 @@
 
 void RabbitizerInstructionRsp_processUniqueId(RabbitizerInstruction *self) {
     uint32_t opcode = RAB_INSTR_GET_opcode(self);
 
     self->_mandatorybits = RAB_INSTR_PACK_opcode(self->_mandatorybits, opcode);
 
     self->uniqueId = RABBITIZER_INSTR_ID_rsp_INVALID;
+    self->instrIdType = RAB_INSTR_ID_TYPE_RSP_INVALID;
 
     switch (opcode) {
         default:
             RabbitizerInstructionRsp_processUniqueId_Normal(self);
             break;
         case 0x00:
             RabbitizerInstructionRsp_processUniqueId_Special(self);
             break;
         case 0x01:
             RabbitizerInstructionRsp_processUniqueId_Regimm(self);
             break;
         case 0x10:
             RabbitizerInstructionRsp_processUniqueId_Coprocessor0(self);
             break;
-        // case 0x11:
-        //    RabbitizerInstructionRsp_processUniqueId_Coprocessor1(self);
-        //    break;
+        case 0x11:
+            RabbitizerInstructionRsp_processUniqueId_Coprocessor1(self);
+            break;
         case 0x12:
             RabbitizerInstructionRsp_processUniqueId_Coprocessor2(self);
             break;
     }
 }
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerRegister.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerRegister.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerRegister.h"
 
 #include <assert.h>
 
 #include "common/Utils.h"
 #include "common/RabbitizerConfig.h"
 
-#include "Registers_Names_arrays.table.h"
+#include "generated/Registers_Names_arrays.h"
 
 const char *RabbitizerRegister_getNameGpr(uint8_t regValue) {
     assert(regValue < ARRAY_COUNT(RabbitizerRegister_GprO32_Names));
 
     switch (RabbitizerConfig_Cfg.regNames.gprAbiNames) {
         case RABBITIZER_ABI_NUMERIC:
             return RabbitizerRegister_GprO32_Names[regValue][0];
```

### Comparing `rabbitizer-1.7.1/src/instructions/RabbitizerRegisterDescriptor.c` & `rabbitizer-1.7.2/src/instructions/RabbitizerRegisterDescriptor.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #include "instructions/RabbitizerRegisterDescriptor.h"
 
 #include "instructions/RabbitizerRegister.h"
 
-#include "RegisterDescriptor_Descriptors_arrays.table.h"
+#include "generated/RegisterDescriptor_Descriptors_arrays.h"
 
 bool RabbitizerRegisterDescriptor_isClobberedByFuncCall(const RabbitizerRegisterDescriptor *self) {
     return self->isClobberedByFuncCall;
 }
 bool RabbitizerRegisterDescriptor_isReserved(const RabbitizerRegisterDescriptor *self) {
     return self->isReserved;
 }
```

### Comparing `rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.h` & `rabbitizer-1.7.2/include/generated/RegisterDescriptor_Descriptors_arrays.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef RegisterDescriptor_Descriptors_arrays_table_h_automatic
-#define RegisterDescriptor_Descriptors_arrays_table_h_automatic
+#ifndef RegisterDescriptor_Descriptors_arrays_h_automatic
+#define RegisterDescriptor_Descriptors_arrays_h_automatic
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_GprO32_Descriptors[] = {
     [RABBITIZER_REG_GPR_O32_zero] = { .isZero=true },
     [RABBITIZER_REG_GPR_O32_at] = { .isClobberedByFuncCall=true, .isAt=true },
     [RABBITIZER_REG_GPR_O32_v0] = { .isClobberedByFuncCall=true, .isReturnReg=true },
     [RABBITIZER_REG_GPR_O32_v1] = { .isClobberedByFuncCall=true, .isReturnReg=true },
     [RABBITIZER_REG_GPR_O32_a0] = { .isClobberedByFuncCall=true, .isArg=true },
```

### Comparing `rabbitizer-1.7.1/src/instructions/RegisterDescriptor_Descriptors_arrays.table.template` & `rabbitizer-1.7.2/tables/templates/c/RegisterDescriptor_Descriptors_arrays.table.template`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 #define RABBITIZER_DEF_REG(prefix, name, numeric, ...) \
     [RABBITIZER_REG_##prefix##_##name] = { __VA_ARGS__ },
 
 #define RABBITIZER_DEF_REG_NODOLLAR(prefix, name, numeric, ...) \
     RABBITIZER_DEF_REG(prefix, name, numeric, __VA_ARGS__)
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_GprO32_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_GprO32.inc"
+#include "registers/RabbitizerRegister_GprO32.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_GprN32_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_GprN32.inc"
+#include "registers/RabbitizerRegister_GprN32.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop0_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop0.inc"
+#include "registers/RabbitizerRegister_Cop0.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop1O32_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop1O32.inc"
+#include "registers/RabbitizerRegister_Cop1O32.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop1N32_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop1N32.inc"
+#include "registers/RabbitizerRegister_Cop1N32.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop1N64_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop1N64.inc"
+#include "registers/RabbitizerRegister_Cop1N64.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop1Control_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop1Control.inc"
+#include "registers/RabbitizerRegister_Cop1Control.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_Cop2_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_Cop2.inc"
+#include "registers/RabbitizerRegister_Cop2.inc"
 };
 
 /* RSP */
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_RspGpr_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_RspGpr.inc"
+#include "registers/RabbitizerRegister_RspGpr.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_RspCop0_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_RspCop0.inc"
+#include "registers/RabbitizerRegister_RspCop0.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_RspCop2_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_RspCop2.inc"
+#include "registers/RabbitizerRegister_RspCop2.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_RspCop2Control_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_RspCop2Control.inc"
+#include "registers/RabbitizerRegister_RspCop2Control.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_RspVector_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_RspVector.inc"
+#include "registers/RabbitizerRegister_RspVector.inc"
 };
 
 /* RSP */
 
 /* R5900 */
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_R5900VF_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_R5900VF.inc"
+#include "registers/RabbitizerRegister_R5900VF.inc"
 };
 
 const RabbitizerRegisterDescriptor RabbitizerRegister_R5900VI_Descriptors[] = {
-#include "instructions/registers/RabbitizerRegister_R5900VI.inc"
+#include "registers/RabbitizerRegister_R5900VI.inc"
 };
 
 /* R5900 */
 
 #undef RABBITIZER_DEF_REG
 #undef RABBITIZER_DEF_REG_NODOLLAR
```

### Comparing `rabbitizer-1.7.1/src/instructions/Registers_Names_arrays.table.h` & `rabbitizer-1.7.2/include/generated/Registers_Names_arrays.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* SPDX-FileCopyrightText: © 2022 Decompollaborate */
+/* SPDX-FileCopyrightText: © 2022-2023 Decompollaborate */
 /* SPDX-License-Identifier: MIT */
 
 /* Automatically generated. DO NOT MODIFY */
 
-#ifndef Registers_Names_arrays_table_h_automatic
-#define Registers_Names_arrays_table_h_automatic
+#ifndef Registers_Names_arrays_h_automatic
+#define Registers_Names_arrays_h_automatic
 
 const char *RabbitizerRegister_GprO32_Names[][2] = {
     [RABBITIZER_REG_GPR_O32_zero] = { "$" "0", "$" "zero" },
     [RABBITIZER_REG_GPR_O32_at] = { "$" "1", "$" "at" },
     [RABBITIZER_REG_GPR_O32_v0] = { "$" "2", "$" "v0" },
     [RABBITIZER_REG_GPR_O32_v1] = { "$" "3", "$" "v1" },
     [RABBITIZER_REG_GPR_O32_a0] = { "$" "4", "$" "a0" },
```

