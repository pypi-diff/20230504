# Comparing `tmp/qiskit-terra-0.9.0.tar.gz` & `tmp/qiskit-terra-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-terra-0.9.0.tar", last modified: Thu Aug 22 15:20:10 2019, max compression
+gzip compressed data, was "dist/qiskit-terra-0.9.1.tar", last modified: Fri Oct 11 17:08:56 2019, max compression
```

## Comparing `qiskit-terra-0.9.0.tar` & `qiskit-terra-0.9.1.tar`

### file list

```diff
@@ -1,436 +1,436 @@
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      225 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/MANIFEST.in
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1291 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4973 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/README.md
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        6 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/VERSION.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2298 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/assembler/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      725 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/assembler/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6336 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/assembler/assemble_circuits.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7731 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/assembler/assemble_schedules.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5924 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/assembler/disassemble.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      715 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/assembler/models.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1259 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/assembler/run_config.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/circuit/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      969 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2132 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/bit.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1398 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/classicalregister.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5769 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/gate.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12508 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/instruction.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2160 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/circuit/instructionset.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1849 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/measure.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2170 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/parameter.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9549 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/parameterexpression.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1775 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/parametertable.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1570 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/parametervector.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    37260 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/circuit/quantumcircuit.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1385 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/quantumregister.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/circuit/random/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      589 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/random/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4313 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/random/utils.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4136 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/register.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1048 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/circuit/reset.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/compiler/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      617 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/compiler/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15363 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/compiler/assemble.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    17408 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/compiler/transpile.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/converters/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      801 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/converters/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14100 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/converters/ast_to_dag.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1239 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/converters/circuit_to_dag.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3552 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/converters/circuit_to_instruction.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1866 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/converters/dag_to_circuit.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/dagcircuit/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      638 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/dagcircuit/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    52003 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/dagcircuit/dagcircuit.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4125 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/dagcircuit/dagnode.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      930 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/dagcircuit/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1154 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9280 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/execute.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/extensions/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      672 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      941 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/extensions/exceptions.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      743 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5855 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/diag.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9740 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/initializer.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    24792 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/isometry.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5225 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/mcg_up_to_diagonal.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7179 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/squ.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15197 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucg.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7642 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucrot.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3985 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucx.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3928 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucy.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3933 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucz.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/extensions/simulator/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      584 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/extensions/simulator/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5013 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/simulator/snapshot.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1246 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2166 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/barrier.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2821 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/ccx.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2314 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/ch.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1716 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/crz.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1652 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cswap.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1796 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cu1.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2144 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cu3.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1305 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cx.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1359 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cxbase.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1594 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cy.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1847 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/cz.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1628 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/h.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1451 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/iden.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1561 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/rx.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1522 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/ry.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1494 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/rz.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1649 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/rzz.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2513 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/s.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1792 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/swap.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2534 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/t.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1746 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/u0.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1673 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/u1.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2061 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/u2.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1759 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/u3.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2108 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/ubase.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1616 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/x.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1558 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/y.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1536 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/standard/z.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4344 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/extensions/unitary.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/providers/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      870 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3552 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basebackend.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1785 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basejob.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2207 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/baseprovider.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4441 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaerjob.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5016 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaerprovider.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6866 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaertools.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      925 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    26836 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/qasm_simulator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5651 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/statevector_simulator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15061 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/basicaer/unitary_simulator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      938 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1029 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/jobstatus.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/providers/models/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      927 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/models/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12565 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/models/backendconfiguration.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4068 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/models/backendproperties.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2084 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/models/backendstatus.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1567 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/providers/models/jobstatus.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4310 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/models/pulsedefaults.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3633 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/providers/providerutils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/pulse/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1144 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      946 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2621 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/channels.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4329 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/device_specification.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5726 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/pulse_channel_spec.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/pulse_channels.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2523 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/qubit.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1775 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/channels/system_topology.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7173 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/cmd_def.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1015 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5599 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/acquire.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3933 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/command.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2841 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/delay.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2268 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/frame_change.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9477 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/instruction.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2278 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/meas_opts.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2555 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/persistent_value.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1475 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/pulse_decorators.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5325 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/sample_pulse.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2816 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/commands/snapshot.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5555 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/configuration.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      922 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/pulse/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5240 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/interfaces.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3871 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/ops.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9119 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/parser.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      570 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11951 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/continuous.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10503 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/discrete.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      563 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10912 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/decorators.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2503 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/strategies.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    18901 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/schedule.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12095 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/timeslots.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5791 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/pulse/utils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qasm/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      691 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      921 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/exceptions.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qasm/libs/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2444 2018-10-10 21:52:46.000000 qiskit-terra-0.9.0/qiskit/qasm/libs/qelib1.inc
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qasm/node/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1340 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/barrier.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1926 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/binaryop.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1521 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/binaryoperator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1068 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/cnot.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1488 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/creg.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1663 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/customunitary.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1129 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/expressionlist.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2647 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/external.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1285 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/format.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2139 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/gate.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1364 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/gatebody.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2983 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/id.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1084 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/idlist.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1185 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/if_.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1351 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/indexedid.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1689 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/intnode.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1086 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/measure.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1995 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/node.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      882 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/nodeexception.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1971 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/opaque.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1690 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/prefix.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1147 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/primarylist.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1020 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/program.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1488 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/qreg.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1782 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/real.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      966 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/reset.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1446 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/node/unaryoperator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1071 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qasm/node/universalunitary.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2221 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/qasm.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5612 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/qasmlexer.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39170 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qasm/qasmparser.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qobj/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1219 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qobj/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qobj/converters/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      716 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/converters/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4180 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/converters/lo_config.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14854 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/converters/pulse_instruction.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/qobj/models/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      536 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/models/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3793 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/models/base.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7662 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/models/pulse.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3685 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/models/qasm.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5005 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/qobj/qobj.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1206 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/qobj/utils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      973 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/analysis/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      565 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/analysis/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1626 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/analysis/average.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1658 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/analysis/make_observable.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      669 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12345 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/base_operator.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      930 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11425 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/chi.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12576 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/choi.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16465 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/kraus.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11410 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/ptm.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7528 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/quantum_channel.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15788 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/stinespring.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19209 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/superop.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16645 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/transformations.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3244 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/measures.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15468 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/operator.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    18257 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/pauli.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5418 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/predicates.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4474 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/operators/quaternion.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/random/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      646 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/random/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4707 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/random/utils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      661 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14532 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/densitymatrix.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2488 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/measures.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     8398 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/quantum_state.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2004 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/states.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14707 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/states/statevector.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      647 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2706 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/local_invariance.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19961 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/two_qubit_decompose.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2703 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/weyl.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/result/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      612 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/result/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1290 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/result/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3774 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/result/models.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6761 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/result/postprocess.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11351 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/result/result.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/schemas/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15483 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/backend_configuration_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3225 2019-08-05 22:35:58.000000 qiskit-terra-0.9.0/qiskit/schemas/backend_properties_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1115 2019-08-05 22:35:58.000000 qiskit-terra-0.9.0/qiskit/schemas/backend_status_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4477 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/default_pulse_configuration_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3866 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/ibmq_device_qobj_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4521 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/ibmq_simulator_qobj_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      714 2018-10-10 21:52:46.000000 qiskit-terra-0.9.0/qiskit/schemas/job_status_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39944 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/qobj_schema.json
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5581 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/schemas/result_schema.json
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/test/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      759 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/test/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6464 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/test/base.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5993 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/test/decorators.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    17877 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/test/mock.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/test/providers/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      634 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/test/providers/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2470 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/test/providers/backend.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2016 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/test/providers/provider.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1273 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/test/reference_circuits.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2897 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/test/testing_options.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3730 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/test/utils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/tools/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      897 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/tools/events/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      565 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/tools/events/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5956 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/events/progressbar.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5423 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/events/pubsub.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1650 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19063 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/backend_monitor.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12125 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/backend_overview.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2002 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/copyright.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5289 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/job_watcher.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5613 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/job_widgets.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6762 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/jupyter_magics.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5176 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/progressbar.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2595 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/version_table.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2388 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/jupyter/watcher_monitor.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/tools/monitor/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      663 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/tools/monitor/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7259 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/monitor/backend_overview.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2670 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/monitor/job_monitor.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6120 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/parallel.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/tools/qi/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      562 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/qi/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16099 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/tools/qi/qi.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      691 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/tools/visualization.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      918 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3627 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/basepasses.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9158 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/coupling.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1424 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2608 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/fencedobjs.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12185 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      736 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/models.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2372 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10607 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/collect_2q_blocks.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4308 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/commutation_analysis.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6414 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/commutative_cancellation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6244 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/consolidate_blocks.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      819 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/count_ops.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      912 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/count_ops_longest_path.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1862 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/cx_cancellation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1266 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/dag_fixed_point.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      893 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/dag_longest_path.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2194 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/decompose.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      812 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/depth.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1696 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/fixed_point.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      560 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2275 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/apply_layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3034 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/barrier_before_final_measurements.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3953 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/basic_swap.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1990 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/check_cx_direction.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1768 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/check_map.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3362 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cx_direction.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      557 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/__init__.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      572 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)   846796 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.cpp
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7863 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.pyx
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)   955347 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.cpp
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1419 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pxd
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6606 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pyx
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4649 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/dense_layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2105 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/enlarge_with_ancilla.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3499 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/full_ancilla_allocation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11356 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/lookahead_swap.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10259 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/noise_adaptive_layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1114 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/set_layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19640 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/stochastic_swap.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1946 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/trivial_layout.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5839 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/merge_adjacent_barriers.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      890 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/num_qubits.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      887 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/num_tensor_factors.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12470 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/optimize_1q_gates.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2562 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/optimize_swap_before_measure.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1966 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/remove_diagonal_gates_before_measure.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1102 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/remove_reset_in_zero_state.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1329 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/resource_estimation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      807 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/size.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2290 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/unroll_3q_or_more.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3578 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/unroller.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      867 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passes/width.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16409 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/passmanager.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      706 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3951 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level0.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4938 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level1.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5164 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level2.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5739 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level3.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      749 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/propertyset.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/transpiler/synthesis/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      603 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/synthesis/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12752 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/synthesis/graysynth.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2416 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/transpiler/transpile_circuit.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1338 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/transpiler/transpile_config.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4313 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/user_config.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3314 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/util.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/validation/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      664 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    13111 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/validation/base.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1038 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/exceptions.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/validation/fields/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2985 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/fields/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2713 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/fields/containers.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7085 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/validation/fields/custom.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9060 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/validation/fields/polymorphic.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/validation/jsonschema/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      658 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/validation/jsonschema/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1526 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/jsonschema/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7210 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/validation/jsonschema/schema_validation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3194 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/validation/validate.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4569 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/version.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/visualization/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2063 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/visualization/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    26888 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/bloch.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    25047 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/circuit_visualization.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7171 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/counts_visualization.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3250 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/dag_visualization.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      706 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/exceptions.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15177 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/visualization/gate_map.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      830 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3355 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_blochsphere.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3026 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_cities.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2739 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_hinton.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4611 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_histogram.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3175 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_paulivec.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6292 2019-08-20 01:35:33.000000 qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_qsphere.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39974 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/latex.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    40627 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/matplotlib.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6735 2019-08-22 15:19:18.000000 qiskit-terra-0.9.0/qiskit/visualization/pass_manager_visualization.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      502 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1593 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse/interpolation.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    22586 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse/matplotlib.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4149 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse/qcstyle.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3078 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/pulse_visualization.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7162 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/qcstyle.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    27052 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/state_visualization.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39716 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/text.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit/visualization/tools/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      539 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/tools/__init__.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3011 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/tools/pi_check.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6856 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/qiskit/visualization/utils.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1291 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)    13919 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/SOURCES.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/dependency_links.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/not-zip-safe
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      298 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/requires.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        7 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/qiskit_terra.egg-info/top_level.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       38 2019-08-22 15:20:10.000000 qiskit-terra-0.9.0/setup.cfg
--rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     3934 2019-08-22 13:34:00.000000 qiskit-terra-0.9.0/setup.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      225 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/MANIFEST.in
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1291 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/PKG-INFO
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4973 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/README.md
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        6 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/VERSION.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2298 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/assembler/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      725 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/assembler/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6336 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/assembler/assemble_circuits.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7731 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/assembler/assemble_schedules.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5924 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/assembler/disassemble.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      715 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/assembler/models.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1259 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/assembler/run_config.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/circuit/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      969 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2132 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/bit.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1398 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/classicalregister.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5769 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/gate.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12508 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/instruction.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2160 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/instructionset.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1849 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/measure.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2170 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/circuit/parameter.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9549 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/parameterexpression.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1775 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/parametertable.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1570 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/parametervector.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    37260 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/quantumcircuit.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1385 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/quantumregister.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/circuit/random/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      589 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/random/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4313 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/circuit/random/utils.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4136 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/register.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1048 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/circuit/reset.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/compiler/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      617 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/compiler/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15363 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/compiler/assemble.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    17408 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/compiler/transpile.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/converters/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      801 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/converters/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14100 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/converters/ast_to_dag.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1239 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/converters/circuit_to_dag.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3552 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/converters/circuit_to_instruction.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1866 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/converters/dag_to_circuit.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/dagcircuit/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      638 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/dagcircuit/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    52003 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/dagcircuit/dagcircuit.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4125 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/dagcircuit/dagnode.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      930 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/dagcircuit/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1154 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9280 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/execute.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/extensions/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      672 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      941 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/extensions/exceptions.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      743 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5855 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/diag.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9740 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/initializer.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    24792 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/isometry.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5225 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/mcg_up_to_diagonal.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7179 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/squ.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15197 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucg.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7642 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucrot.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3985 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucx.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3928 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucy.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3933 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucz.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/extensions/simulator/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      584 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/extensions/simulator/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5013 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/simulator/snapshot.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1246 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2166 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/barrier.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2821 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/ccx.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2314 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/ch.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1716 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/crz.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1652 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cswap.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1796 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cu1.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2144 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cu3.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1305 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cx.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1359 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cxbase.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1594 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cy.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1847 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/cz.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1628 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/h.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1451 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/iden.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1561 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/rx.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1522 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/ry.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1494 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/rz.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1649 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/rzz.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2513 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/s.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1792 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/swap.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2534 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/t.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1746 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/u0.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1673 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/u1.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2061 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/u2.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1759 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/u3.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2108 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/ubase.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1616 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/x.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1558 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/y.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1536 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/standard/z.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4344 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/extensions/unitary.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/providers/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      870 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3552 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/providers/basebackend.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1785 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basejob.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2207 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/baseprovider.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4441 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaerjob.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5016 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaerprovider.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6866 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaertools.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      925 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    26836 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/qasm_simulator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5651 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/statevector_simulator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15061 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/basicaer/unitary_simulator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      938 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1029 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/jobstatus.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/providers/models/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      927 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/models/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12565 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/models/backendconfiguration.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4068 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/models/backendproperties.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2084 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/models/backendstatus.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1567 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/providers/models/jobstatus.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4310 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/models/pulsedefaults.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3633 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/providers/providerutils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/pulse/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1144 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      946 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2621 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/channels.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4329 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/device_specification.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5726 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/pulse_channel_spec.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/pulse_channels.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2523 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/qubit.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1775 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/channels/system_topology.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7173 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/cmd_def.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1015 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5599 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/acquire.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3933 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/command.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2841 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/delay.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2268 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/frame_change.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9477 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/instruction.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2278 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/meas_opts.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2555 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/persistent_value.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1475 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/pulse_decorators.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5325 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/sample_pulse.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2816 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/commands/snapshot.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5555 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/configuration.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      922 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/pulse/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5240 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/interfaces.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3871 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/ops.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9119 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/parser.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      570 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11951 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/continuous.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10503 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/discrete.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      563 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10912 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/decorators.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2503 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/strategies.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    18901 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/schedule.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12095 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/timeslots.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5791 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/pulse/utils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qasm/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      691 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      921 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/exceptions.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qasm/libs/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2444 2018-10-10 21:52:46.000000 qiskit-terra-0.9.1/qiskit/qasm/libs/qelib1.inc
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qasm/node/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1340 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      965 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/barrier.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1926 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/node/binaryop.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1521 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/node/binaryoperator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1068 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/cnot.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1488 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/creg.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1663 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/customunitary.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1129 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/expressionlist.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2647 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/node/external.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1285 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/node/format.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2139 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/gate.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1364 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/gatebody.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2983 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/node/id.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1084 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/idlist.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1185 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/if_.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1351 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/node/indexedid.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1689 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/node/intnode.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1086 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/measure.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1995 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/node.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      882 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/nodeexception.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1971 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/opaque.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1690 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/node/prefix.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1147 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/primarylist.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1020 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/program.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1488 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/qreg.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1782 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/node/real.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      966 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/reset.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1446 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/node/unaryoperator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1071 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qasm/node/universalunitary.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2221 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qasm/qasm.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5612 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/qasmlexer.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39170 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/qasm/qasmparser.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qobj/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1219 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/qobj/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qobj/converters/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      716 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/converters/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4180 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/qobj/converters/lo_config.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14854 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/converters/pulse_instruction.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/qobj/models/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      536 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/models/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3793 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/models/base.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7662 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/models/pulse.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3685 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/models/qasm.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5005 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/qobj/qobj.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1206 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/qobj/utils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      973 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/analysis/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      565 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/analysis/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1626 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/analysis/average.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1658 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/analysis/make_observable.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      669 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12345 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/base_operator.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      930 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11425 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/chi.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12576 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/choi.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16465 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/kraus.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11410 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/ptm.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7528 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/quantum_channel.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15788 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/stinespring.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19209 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/superop.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16645 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/transformations.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3244 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/measures.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15468 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/operator.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    18257 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/pauli.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5418 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/predicates.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4474 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/operators/quaternion.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/random/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      646 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/random/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4707 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/random/utils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      661 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14532 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/densitymatrix.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2488 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/measures.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     8398 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/quantum_state.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2004 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/states.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    14707 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/states/statevector.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      647 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2706 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/local_invariance.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19961 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/two_qubit_decompose.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2703 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/weyl.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/result/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      612 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/result/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1290 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/result/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3774 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/result/models.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6761 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/result/postprocess.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11351 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/result/result.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/schemas/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15483 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/backend_configuration_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3225 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/backend_properties_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1115 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/backend_status_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4477 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/default_pulse_configuration_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3866 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/ibmq_device_qobj_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4521 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/ibmq_simulator_qobj_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      714 2018-10-10 21:52:46.000000 qiskit-terra-0.9.1/qiskit/schemas/job_status_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39944 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/qobj_schema.json
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5581 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/schemas/result_schema.json
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/test/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      759 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/test/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6464 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/test/base.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5993 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/test/decorators.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    17877 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/test/mock.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/test/providers/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      634 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/test/providers/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2470 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/test/providers/backend.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2016 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/test/providers/provider.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1273 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/test/reference_circuits.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2897 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/test/testing_options.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3730 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/test/utils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/tools/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      897 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/tools/events/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      565 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/tools/events/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5956 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/events/progressbar.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5423 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/events/pubsub.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1650 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19063 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/backend_monitor.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12125 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/backend_overview.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2002 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/copyright.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5289 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/job_watcher.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5613 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/job_widgets.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6762 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/jupyter_magics.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5176 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/progressbar.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2595 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/version_table.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2388 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/jupyter/watcher_monitor.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/tools/monitor/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      663 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/tools/monitor/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7259 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/monitor/backend_overview.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2670 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/monitor/job_monitor.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6120 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/parallel.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/tools/qi/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      562 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/qi/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16099 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/tools/qi/qi.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      691 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/tools/visualization.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      918 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3627 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/basepasses.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9158 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/coupling.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1424 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2608 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/fencedobjs.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12185 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      736 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/models.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2372 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10607 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/collect_2q_blocks.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4308 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/commutation_analysis.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6414 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/commutative_cancellation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6244 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/consolidate_blocks.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      819 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/count_ops.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      912 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/count_ops_longest_path.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1862 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/cx_cancellation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1266 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/dag_fixed_point.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      893 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/dag_longest_path.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2194 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/decompose.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      812 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/depth.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1696 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/fixed_point.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      560 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2275 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/apply_layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3034 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/barrier_before_final_measurements.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3953 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/basic_swap.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1990 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/check_cx_direction.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1768 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/check_map.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3362 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cx_direction.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      557 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/__init__.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      572 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)   844791 2019-10-11 17:08:55.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.cpp
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7863 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.pyx
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)   953122 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.cpp
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1419 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pxd
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6606 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pyx
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4649 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/dense_layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2105 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/enlarge_with_ancilla.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3499 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/full_ancilla_allocation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    11356 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/lookahead_swap.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    10259 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/noise_adaptive_layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1114 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/set_layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    19640 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/stochastic_swap.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1946 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/trivial_layout.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5839 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/merge_adjacent_barriers.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      890 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/num_qubits.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      887 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/num_tensor_factors.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12470 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/optimize_1q_gates.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2562 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/optimize_swap_before_measure.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1966 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/remove_diagonal_gates_before_measure.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1102 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/remove_reset_in_zero_state.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1329 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/resource_estimation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      807 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/size.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2290 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/unroll_3q_or_more.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3578 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/unroller.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      867 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/passes/width.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    16409 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/passmanager.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      706 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3951 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level0.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4938 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level1.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5164 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level2.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5739 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level3.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      749 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/propertyset.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/transpiler/synthesis/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      603 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/synthesis/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    12752 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/synthesis/graysynth.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2416 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/transpiler/transpile_circuit.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1338 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/transpiler/transpile_config.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4313 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/user_config.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3314 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/util.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/validation/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      664 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/validation/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    13111 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/validation/base.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1038 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/validation/exceptions.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/validation/fields/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2985 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/validation/fields/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2713 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/validation/fields/containers.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7085 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/validation/fields/custom.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     9060 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/validation/fields/polymorphic.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/validation/jsonschema/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      658 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/validation/jsonschema/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1526 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/validation/jsonschema/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7210 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/validation/jsonschema/schema_validation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3194 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/validation/validate.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4569 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/version.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/visualization/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2063 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    26888 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/bloch.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    25047 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/circuit_visualization.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7171 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/counts_visualization.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3250 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/dag_visualization.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      706 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/exceptions.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    15177 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/gate_map.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      830 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3355 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_blochsphere.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3026 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_cities.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     2739 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_hinton.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4611 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_histogram.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3175 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_paulivec.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6292 2019-09-13 13:17:49.000000 qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_qsphere.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39974 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/latex.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    41089 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/matplotlib.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6820 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/pass_manager_visualization.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      502 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1593 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse/interpolation.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    22586 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse/matplotlib.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     4149 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse/qcstyle.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3078 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/pulse_visualization.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     7162 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/qcstyle.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    27052 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/state_visualization.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    39716 2019-10-01 20:26:06.000000 qiskit-terra-0.9.1/qiskit/visualization/text.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit/visualization/tools/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      539 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/tools/__init__.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     3011 2019-09-24 21:38:18.000000 qiskit-terra-0.9.1/qiskit/visualization/tools/pi_check.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     6856 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/qiskit/visualization/utils.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1291 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/PKG-INFO
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)    13919 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/SOURCES.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/dependency_links.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/not-zip-safe
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      293 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/requires.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        7 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/qiskit_terra.egg-info/top_level.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)       38 2019-10-11 17:08:56.000000 qiskit-terra-0.9.1/setup.cfg
+-rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     3929 2019-10-11 16:54:26.000000 qiskit-terra-0.9.1/setup.py
```

### Comparing `qiskit-terra-0.9.0/PKG-INFO` & `qiskit-terra-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-terra
-Version: 0.9.0
+Version: 0.9.1
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit-terra
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-terra/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -21,9 +21,9 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
-Provides-Extra: full-featured-simulators
 Provides-Extra: visualization
+Provides-Extra: full-featured-simulators
```

### Comparing `qiskit-terra-0.9.0/README.md` & `qiskit-terra-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/__init__.py` & `qiskit-terra-0.9.1/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/__init__.py` & `qiskit-terra-0.9.1/qiskit/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/assemble_circuits.py` & `qiskit-terra-0.9.1/qiskit/assembler/assemble_circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/assemble_schedules.py` & `qiskit-terra-0.9.1/qiskit/assembler/assemble_schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/disassemble.py` & `qiskit-terra-0.9.1/qiskit/assembler/disassemble.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/models.py` & `qiskit-terra-0.9.1/qiskit/assembler/models.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/assembler/run_config.py` & `qiskit-terra-0.9.1/qiskit/assembler/run_config.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/__init__.py` & `qiskit-terra-0.9.1/qiskit/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/bit.py` & `qiskit-terra-0.9.1/qiskit/circuit/bit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/classicalregister.py` & `qiskit-terra-0.9.1/qiskit/circuit/classicalregister.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/gate.py` & `qiskit-terra-0.9.1/qiskit/circuit/gate.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/instruction.py` & `qiskit-terra-0.9.1/qiskit/circuit/instruction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/instructionset.py` & `qiskit-terra-0.9.1/qiskit/circuit/instructionset.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/measure.py` & `qiskit-terra-0.9.1/qiskit/circuit/measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/parameter.py` & `qiskit-terra-0.9.1/qiskit/circuit/parameter.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/parameterexpression.py` & `qiskit-terra-0.9.1/qiskit/circuit/parameterexpression.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/parametertable.py` & `qiskit-terra-0.9.1/qiskit/circuit/parametertable.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/parametervector.py` & `qiskit-terra-0.9.1/qiskit/circuit/parametervector.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/quantumcircuit.py` & `qiskit-terra-0.9.1/qiskit/circuit/quantumcircuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/quantumregister.py` & `qiskit-terra-0.9.1/qiskit/circuit/quantumregister.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/random/__init__.py` & `qiskit-terra-0.9.1/qiskit/circuit/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/random/utils.py` & `qiskit-terra-0.9.1/qiskit/circuit/random/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/register.py` & `qiskit-terra-0.9.1/qiskit/circuit/register.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/circuit/reset.py` & `qiskit-terra-0.9.1/qiskit/circuit/reset.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/compiler/__init__.py` & `qiskit-terra-0.9.1/qiskit/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/compiler/assemble.py` & `qiskit-terra-0.9.1/qiskit/compiler/assemble.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/compiler/transpile.py` & `qiskit-terra-0.9.1/qiskit/compiler/transpile.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/converters/__init__.py` & `qiskit-terra-0.9.1/qiskit/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/converters/ast_to_dag.py` & `qiskit-terra-0.9.1/qiskit/converters/ast_to_dag.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/converters/circuit_to_dag.py` & `qiskit-terra-0.9.1/qiskit/converters/circuit_to_dag.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/converters/circuit_to_instruction.py` & `qiskit-terra-0.9.1/qiskit/converters/circuit_to_instruction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/converters/dag_to_circuit.py` & `qiskit-terra-0.9.1/qiskit/converters/dag_to_circuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/dagcircuit/__init__.py` & `qiskit-terra-0.9.1/qiskit/dagcircuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/dagcircuit/dagcircuit.py` & `qiskit-terra-0.9.1/qiskit/dagcircuit/dagcircuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/dagcircuit/dagnode.py` & `qiskit-terra-0.9.1/qiskit/dagcircuit/dagnode.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/dagcircuit/exceptions.py` & `qiskit-terra-0.9.1/qiskit/dagcircuit/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/exceptions.py` & `qiskit-terra-0.9.1/qiskit/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/execute.py` & `qiskit-terra-0.9.1/qiskit/execute.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/__init__.py` & `qiskit-terra-0.9.1/qiskit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/exceptions.py` & `qiskit-terra-0.9.1/qiskit/extensions/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/__init__.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/diag.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/diag.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/initializer.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/initializer.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/isometry.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/isometry.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/mcg_up_to_diagonal.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/mcg_up_to_diagonal.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/squ.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/squ.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucg.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucg.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucrot.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucrot.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucx.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucx.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucy.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucy.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/quantum_initializer/ucz.py` & `qiskit-terra-0.9.1/qiskit/extensions/quantum_initializer/ucz.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/simulator/__init__.py` & `qiskit-terra-0.9.1/qiskit/extensions/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/simulator/snapshot.py` & `qiskit-terra-0.9.1/qiskit/extensions/simulator/snapshot.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/__init__.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/barrier.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/barrier.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/ccx.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/ccx.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/ch.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/ch.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/crz.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/crz.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cswap.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cswap.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cu1.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cu1.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cu3.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cu3.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cx.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cx.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cxbase.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cxbase.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cy.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cy.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/cz.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/cz.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/h.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/h.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/iden.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/iden.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/rx.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/rx.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/ry.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/ry.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/rz.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/rz.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/rzz.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/rzz.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/s.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/s.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/swap.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/swap.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/t.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/t.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/u0.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/u0.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/u1.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/u1.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/u2.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/u2.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/u3.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/u3.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/ubase.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/ubase.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/x.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/x.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/y.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/y.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/standard/z.py` & `qiskit-terra-0.9.1/qiskit/extensions/standard/z.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/extensions/unitary.py` & `qiskit-terra-0.9.1/qiskit/extensions/unitary.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/__init__.py` & `qiskit-terra-0.9.1/qiskit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basebackend.py` & `qiskit-terra-0.9.1/qiskit/providers/basebackend.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basejob.py` & `qiskit-terra-0.9.1/qiskit/providers/basejob.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/baseprovider.py` & `qiskit-terra-0.9.1/qiskit/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/__init__.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaerjob.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaerjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaerprovider.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaerprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/basicaertools.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/basicaertools.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/exceptions.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/qasm_simulator.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/statevector_simulator.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/statevector_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/basicaer/unitary_simulator.py` & `qiskit-terra-0.9.1/qiskit/providers/basicaer/unitary_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/exceptions.py` & `qiskit-terra-0.9.1/qiskit/providers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/jobstatus.py` & `qiskit-terra-0.9.1/qiskit/providers/jobstatus.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/__init__.py` & `qiskit-terra-0.9.1/qiskit/providers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/backendconfiguration.py` & `qiskit-terra-0.9.1/qiskit/providers/models/backendconfiguration.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/backendproperties.py` & `qiskit-terra-0.9.1/qiskit/providers/models/backendproperties.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/backendstatus.py` & `qiskit-terra-0.9.1/qiskit/providers/models/backendstatus.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/jobstatus.py` & `qiskit-terra-0.9.1/qiskit/providers/models/jobstatus.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/models/pulsedefaults.py` & `qiskit-terra-0.9.1/qiskit/providers/models/pulsedefaults.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/providers/providerutils.py` & `qiskit-terra-0.9.1/qiskit/providers/providerutils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/__init__.py` & `qiskit-terra-0.9.1/qiskit/pulse/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/__init__.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/channels.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/channels.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/device_specification.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/device_specification.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/pulse_channel_spec.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/pulse_channel_spec.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/pulse_channels.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/pulse_channels.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/qubit.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/qubit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/channels/system_topology.py` & `qiskit-terra-0.9.1/qiskit/pulse/channels/system_topology.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/cmd_def.py` & `qiskit-terra-0.9.1/qiskit/pulse/cmd_def.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/__init__.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/acquire.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/command.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/command.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/delay.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/frame_change.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/frame_change.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/instruction.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/instruction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/meas_opts.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/meas_opts.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/persistent_value.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/persistent_value.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/pulse_decorators.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/pulse_decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/sample_pulse.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/sample_pulse.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/commands/snapshot.py` & `qiskit-terra-0.9.1/qiskit/pulse/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/configuration.py` & `qiskit-terra-0.9.1/qiskit/pulse/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/exceptions.py` & `qiskit-terra-0.9.1/qiskit/pulse/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/interfaces.py` & `qiskit-terra-0.9.1/qiskit/pulse/interfaces.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/ops.py` & `qiskit-terra-0.9.1/qiskit/pulse/ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/parser.py` & `qiskit-terra-0.9.1/qiskit/pulse/parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/__init__.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/continuous.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/continuous.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/discrete.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/discrete.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/__init__.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/decorators.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/pulse_lib/samplers/strategies.py` & `qiskit-terra-0.9.1/qiskit/pulse/pulse_lib/samplers/strategies.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/schedule.py` & `qiskit-terra-0.9.1/qiskit/pulse/schedule.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/timeslots.py` & `qiskit-terra-0.9.1/qiskit/pulse/timeslots.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/pulse/utils.py` & `qiskit-terra-0.9.1/qiskit/pulse/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/__init__.py` & `qiskit-terra-0.9.1/qiskit/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/exceptions.py` & `qiskit-terra-0.9.1/qiskit/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/libs/qelib1.inc` & `qiskit-terra-0.9.1/qiskit/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/__init__.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/barrier.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/binaryop.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/binaryoperator.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/cnot.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/cnot.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/creg.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/customunitary.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/expressionlist.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/external.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/format.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/gate.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/gatebody.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/id.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/idlist.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/if_.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/indexedid.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/intnode.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/measure.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/node.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/nodeexception.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/opaque.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/prefix.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/primarylist.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/program.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/qreg.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/real.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/reset.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/unaryoperator.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/node/universalunitary.py` & `qiskit-terra-0.9.1/qiskit/qasm/node/universalunitary.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/qasm.py` & `qiskit-terra-0.9.1/qiskit/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/qasmlexer.py` & `qiskit-terra-0.9.1/qiskit/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qasm/qasmparser.py` & `qiskit-terra-0.9.1/qiskit/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/__init__.py` & `qiskit-terra-0.9.1/qiskit/qobj/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/converters/__init__.py` & `qiskit-terra-0.9.1/qiskit/qobj/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/converters/lo_config.py` & `qiskit-terra-0.9.1/qiskit/qobj/converters/lo_config.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/converters/pulse_instruction.py` & `qiskit-terra-0.9.1/qiskit/qobj/converters/pulse_instruction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/models/__init__.py` & `qiskit-terra-0.9.1/qiskit/qobj/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/models/base.py` & `qiskit-terra-0.9.1/qiskit/qobj/models/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/models/pulse.py` & `qiskit-terra-0.9.1/qiskit/qobj/models/pulse.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/models/qasm.py` & `qiskit-terra-0.9.1/qiskit/qobj/models/qasm.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/qobj.py` & `qiskit-terra-0.9.1/qiskit/qobj/qobj.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/qobj/utils.py` & `qiskit-terra-0.9.1/qiskit/qobj/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/analysis/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/analysis/average.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/analysis/average.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/analysis/make_observable.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/analysis/make_observable.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/base_operator.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/chi.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/chi.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/choi.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/choi.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/kraus.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/kraus.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/ptm.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/ptm.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/quantum_channel.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/quantum_channel.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/stinespring.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/stinespring.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/superop.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/superop.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/channel/transformations.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/channel/transformations.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/measures.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/measures.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/operator.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/operator.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/pauli.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/pauli.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/predicates.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/predicates.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/operators/quaternion.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/operators/quaternion.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/random/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/random/utils.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/random/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/densitymatrix.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/measures.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/measures.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/quantum_state.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/quantum_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/states.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/states.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/states/statevector.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/states/statevector.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/__init__.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/local_invariance.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/local_invariance.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/two_qubit_decompose.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/two_qubit_decompose.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/quantum_info/synthesis/weyl.py` & `qiskit-terra-0.9.1/qiskit/quantum_info/synthesis/weyl.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/result/__init__.py` & `qiskit-terra-0.9.1/qiskit/result/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/result/exceptions.py` & `qiskit-terra-0.9.1/qiskit/result/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/result/models.py` & `qiskit-terra-0.9.1/qiskit/result/models.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/result/postprocess.py` & `qiskit-terra-0.9.1/qiskit/result/postprocess.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/result/result.py` & `qiskit-terra-0.9.1/qiskit/result/result.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/backend_configuration_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/backend_configuration_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/backend_properties_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/backend_properties_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/backend_status_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/backend_status_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/default_pulse_configuration_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/default_pulse_configuration_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/ibmq_device_qobj_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/ibmq_device_qobj_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/ibmq_simulator_qobj_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/ibmq_simulator_qobj_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/job_status_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/job_status_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/qobj_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/qobj_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/schemas/result_schema.json` & `qiskit-terra-0.9.1/qiskit/schemas/result_schema.json`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/__init__.py` & `qiskit-terra-0.9.1/qiskit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/base.py` & `qiskit-terra-0.9.1/qiskit/test/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/decorators.py` & `qiskit-terra-0.9.1/qiskit/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/mock.py` & `qiskit-terra-0.9.1/qiskit/test/mock.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/providers/__init__.py` & `qiskit-terra-0.9.1/qiskit/test/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/providers/backend.py` & `qiskit-terra-0.9.1/qiskit/test/providers/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/providers/provider.py` & `qiskit-terra-0.9.1/qiskit/test/providers/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/reference_circuits.py` & `qiskit-terra-0.9.1/qiskit/test/reference_circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/testing_options.py` & `qiskit-terra-0.9.1/qiskit/test/testing_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/test/utils.py` & `qiskit-terra-0.9.1/qiskit/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/__init__.py` & `qiskit-terra-0.9.1/qiskit/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/events/__init__.py` & `qiskit-terra-0.9.1/qiskit/tools/events/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/events/progressbar.py` & `qiskit-terra-0.9.1/qiskit/tools/events/progressbar.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/events/pubsub.py` & `qiskit-terra-0.9.1/qiskit/tools/events/pubsub.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/__init__.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/backend_monitor.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/backend_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/backend_overview.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/backend_overview.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/copyright.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/copyright.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/job_watcher.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/job_watcher.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/job_widgets.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/jupyter_magics.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/jupyter_magics.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/progressbar.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/progressbar.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/version_table.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/version_table.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/jupyter/watcher_monitor.py` & `qiskit-terra-0.9.1/qiskit/tools/jupyter/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/monitor/__init__.py` & `qiskit-terra-0.9.1/qiskit/tools/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/monitor/backend_overview.py` & `qiskit-terra-0.9.1/qiskit/tools/monitor/backend_overview.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/monitor/job_monitor.py` & `qiskit-terra-0.9.1/qiskit/tools/monitor/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/parallel.py` & `qiskit-terra-0.9.1/qiskit/tools/parallel.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/qi/__init__.py` & `qiskit-terra-0.9.1/qiskit/tools/qi/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/qi/qi.py` & `qiskit-terra-0.9.1/qiskit/tools/qi/qi.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/tools/visualization.py` & `qiskit-terra-0.9.1/qiskit/tools/visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/basepasses.py` & `qiskit-terra-0.9.1/qiskit/transpiler/basepasses.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/coupling.py` & `qiskit-terra-0.9.1/qiskit/transpiler/coupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/exceptions.py` & `qiskit-terra-0.9.1/qiskit/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/fencedobjs.py` & `qiskit-terra-0.9.1/qiskit/transpiler/fencedobjs.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/models.py` & `qiskit-terra-0.9.1/qiskit/transpiler/models.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/collect_2q_blocks.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/collect_2q_blocks.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/commutation_analysis.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/commutation_analysis.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/commutative_cancellation.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/commutative_cancellation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/consolidate_blocks.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/consolidate_blocks.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/count_ops.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/count_ops.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/count_ops_longest_path.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/count_ops_longest_path.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/cx_cancellation.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/cx_cancellation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/dag_fixed_point.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/dag_fixed_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/dag_longest_path.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/dag_longest_path.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/decompose.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/decompose.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/depth.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/depth.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/fixed_point.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/fixed_point.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/apply_layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/apply_layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/barrier_before_final_measurements.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/barrier_before_final_measurements.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/basic_swap.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/basic_swap.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/check_cx_direction.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/check_cx_direction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/check_map.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/check_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cx_direction.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cx_direction.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.cpp` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.13 */
+/* Generated by Cython 0.29.7 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O2",
@@ -22,16 +22,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_13"
-#define CYTHON_HEX_VERSION 0x001D0DF0
+#define CYTHON_ABI "0_29_7"
+#define CYTHON_HEX_VERSION 0x001D07F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -339,21 +339,16 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
-#else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
-#endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
@@ -1055,15 +1050,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1136,15 +1131,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -1246,15 +1241,15 @@
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs);
 #else
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
@@ -6088,189 +6083,150 @@
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
+ * 
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "View.MemoryView":374
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
+ *         cdef int i
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
     /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- */
-    goto __pyx_L3;
-  }
-
-  /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- */
-  __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
-  if (__pyx_t_2) {
-
-    /* "View.MemoryView":377
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
- *             Py_DECREF(Py_None)
- * 
- */
-    ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
-
-    /* "View.MemoryView":378
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
- * 
- *         cdef int i
- */
-    Py_DECREF(Py_None);
-
-    /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
-  __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":379
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":381
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":384
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":383
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":385
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":387
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
@@ -6283,15 +6239,15 @@
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -6306,107 +6262,107 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":391
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 393, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 397, __pyx_L1_error)
+          else __PYX_ERR(1, 393, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":394
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 398, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 394, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":396
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -6418,15 +6374,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -6453,143 +6409,143 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":401
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":403
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 407, __pyx_L1_error)
+      __PYX_ERR(1, 403, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 403, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 406, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":407
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":409
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 409, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":410
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -6604,15 +6560,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -6637,182 +6593,182 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 418, __pyx_L1_error)
+    __PYX_ERR(1, 414, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":416
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 420, __pyx_L1_error)
+      __PYX_ERR(1, 416, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 416, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 422, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 418, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":419
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 424, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 420, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":421
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":423
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 423, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":425
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -6829,15 +6785,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -6852,26 +6808,26 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -6879,59 +6835,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":431
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 435, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 431, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -6940,30 +6896,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":432
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 432, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":433
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -6972,15 +6928,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -6993,36 +6949,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":435
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -7036,15 +6992,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -7055,58 +7011,58 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 445, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":442
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 446, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 442, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":443
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_4 = __pyx_memoryview_copy_contents((__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice))[0]), (__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice))[0]), __pyx_t_2, __pyx_t_3, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 445, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_copy_contents((__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice))[0]), (__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice))[0]), __pyx_t_2, __pyx_t_3, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -7119,15 +7075,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -7148,203 +7104,203 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":447
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":452
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
   __pyx_v_dst_slice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice));
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
   __pyx_t_1 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":455
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     __pyx_t_1 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":457
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(1, 461, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(1, 457, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":458
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":460
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":462
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":464
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":466
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 470, __pyx_L6_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 466, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     __pyx_t_1 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":471
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_2 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 475, __pyx_L6_error)
+      __pyx_t_2 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 471, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":472
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":475
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -7383,15 +7339,15 @@
       __pyx_t_6 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_3; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_5;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -7404,15 +7360,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -7420,36 +7376,36 @@
   char *__pyx_v_itemp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":478
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 478, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":479
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 483, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -7462,15 +7418,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -7489,39 +7445,39 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   size_t __pyx_t_10;
   int __pyx_t_11;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":484
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":487
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 491, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -7529,24 +7485,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":489
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7555,94 +7511,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":494
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 494, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":495
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -7653,52 +7609,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":490
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 490, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 490, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 491, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __PYX_ERR(1, 491, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -7710,15 +7666,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -7736,15 +7692,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -7767,88 +7723,88 @@
   PyObject *__pyx_t_10 = NULL;
   char *__pyx_t_11;
   char *__pyx_t_12;
   char *__pyx_t_13;
   char *__pyx_t_14;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":500
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":506
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 506, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":508
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -7857,102 +7813,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 508, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(1, 514, __pyx_L1_error)
+    __PYX_ERR(1, 510, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -7972,15 +7928,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -8012,15 +7968,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -8030,268 +7986,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 516, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 520, __pyx_L1_error)
+    __PYX_ERR(1, 516, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":519
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":521
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":524
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":526
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":529
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":531
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":534
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":536
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":538
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":539
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":540
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":541
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":542
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":543
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -8313,15 +8269,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -8342,49 +8298,49 @@
   struct __pyx_memoryviewslice_obj *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":550
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 550, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":551
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 555, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 551, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":552
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -8396,15 +8352,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -8422,42 +8378,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":556
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -8481,41 +8437,41 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":560
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -8527,15 +8483,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -8560,73 +8516,73 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 570, __pyx_L1_error)
+    __PYX_ERR(1, 566, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":568
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -8638,15 +8594,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -8671,77 +8627,77 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__12, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__12, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":575
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -8753,15 +8709,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -8780,29 +8736,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":579
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -8813,15 +8769,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -8840,29 +8796,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":583
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -8873,15 +8829,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -8902,35 +8858,35 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":587
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -8943,15 +8899,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -8977,98 +8933,98 @@
   int __pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":592
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":594
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 594, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":595
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 599, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 595, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":597
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":599
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -9081,15 +9037,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -9108,68 +9064,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":603
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":605
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -9190,64 +9146,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":609
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -9260,15 +9216,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -9288,43 +9244,43 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_14__str__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":612
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -9336,15 +9292,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -9365,38 +9321,38 @@
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":618
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
   __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":619
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 623, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -9407,15 +9363,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -9436,38 +9392,38 @@
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
   __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 629, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -9478,15 +9434,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -9508,57 +9464,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":629
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":631
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":632
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 632, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":637
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -9569,15 +9525,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -9600,57 +9556,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":641
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":643
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":644
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 648, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 644, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":649
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -9768,15 +9724,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -9785,64 +9741,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":654
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":655
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":656
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -9856,54 +9812,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -9926,243 +9882,243 @@
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":668
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 668, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":670
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":672
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 676, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":673
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":674
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 675, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 679, __pyx_L1_error)
+          else __PYX_ERR(1, 675, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":678
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__15);
             __Pyx_GIVEREF(__pyx_slice__15);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__15);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":679
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":681
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__15); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__15); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 681, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":682
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -10174,40 +10130,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":685
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(1, 689, __pyx_L1_error)
+        __PYX_ERR(1, 685, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":687
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -10218,120 +10174,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":688
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 688, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":690
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 694, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 690, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":692
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__15);
         __Pyx_GIVEREF(__pyx_slice__15);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__15);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":694
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -10349,15 +10305,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -10368,60 +10324,60 @@
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":697
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 699, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(1, 703, __pyx_L1_error)
+      __PYX_ERR(1, 699, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -10434,15 +10390,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -10475,529 +10431,529 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":707
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":714
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":718
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 722, __pyx_L1_error)
+      __PYX_ERR(1, 718, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":721
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 725, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 721, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":722
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":724
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":725
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":731
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":732
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":737
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":738
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 742, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 742, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 746, __pyx_L1_error)
+          else __PYX_ERR(1, 742, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":747
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 751, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 747, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":744
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 748, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 744, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":751
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":752
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":753
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":754
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":756
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 756, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 756, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 756, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":757
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 757, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 757, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 757, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":758
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 758, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 758, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 758, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":760
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":761
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 765, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":762
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":764
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 768, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 764, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":770
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":774
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 778, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 774, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":775
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 779, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 775, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 777, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 773, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":779
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 782, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 782, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 778, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -11011,15 +10967,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -11027,95 +10983,95 @@
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":826
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":828
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 828, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":831
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -11126,15 +11082,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -11144,639 +11100,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":834
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":839
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":841
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":844
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":846
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":849
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":851
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":855
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":857
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":859
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":862
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":864
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":867
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":871
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":874
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":877
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":880
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":881
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":882
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":886
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":888
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":893
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":895
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":896
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 899, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 895, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":898
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":900
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -11792,15 +11748,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -11814,280 +11770,280 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":908
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":909
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":913
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     __pyx_v_shape = __Pyx_div_Py_ssize_t(__pyx_v_view->len, __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":914
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":916
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":917
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":919
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":922
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":924
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 928, __pyx_L1_error)
+      __PYX_ERR(1, 924, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":927
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 931, __pyx_L1_error)
+    __PYX_ERR(1, 927, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":929
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":931
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":933
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -12098,15 +12054,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -12123,90 +12079,90 @@
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":940
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":942
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":943
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":947
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = __Pyx_div_long(__pyx_v_ndim, 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":948
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":949
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":950
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -12216,44 +12172,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":953
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 953, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":955
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -12269,15 +12225,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -12292,100 +12248,100 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":973
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":977
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 977, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":979
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 979, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -12396,15 +12352,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -12412,58 +12368,58 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":983
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 987, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 983, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":985
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -12476,15 +12432,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -12502,27 +12458,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":989
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -12636,15 +12592,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -12661,351 +12617,351 @@
   Py_buffer __pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1004
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1009
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1011
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1012
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1014
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1018, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1014, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1015
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1017
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1018
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1019
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1020
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1021
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1024
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1026
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1028
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1029
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1032
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1033
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1035
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1036
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1038
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1039
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1039, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1040
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1042
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1043
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1045
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -13019,15 +12975,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
@@ -13036,79 +12992,79 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1055
+  /* "View.MemoryView":1051
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1052
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1056, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1052, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1053
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
+    /* "View.MemoryView":1051
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1055
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1056
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
@@ -13119,15 +13075,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -13140,158 +13096,158 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1063
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1064
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1065
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1067
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1068
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1070
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1071
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1072
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1073
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
 static PyObject *__pyx_memoryview_copy_object(struct __pyx_memoryview_obj *__pyx_v_memview) {
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1079
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1080
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1080, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -13302,15 +13258,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -13322,99 +13278,99 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *(*__pyx_t_3)(char *);
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1091
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1092
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1094
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1095
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1097
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1099
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1101, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -13425,81 +13381,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1107
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1109
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -13509,187 +13465,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1117
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1118
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1120
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1122
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1123
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1125
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1127
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1128
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1131
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1133
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -13702,61 +13658,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1143
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1144
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1145
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1146
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -13768,195 +13724,195 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1150
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1151
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1153
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1154
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1155
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1156
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1158
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1159
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1163
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1164
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1169
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  */
 
@@ -13965,70 +13921,70 @@
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1180
+  /* "View.MemoryView":1176
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  *     cdef Py_ssize_t size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1182
+  /* "View.MemoryView":1178
  *     cdef Py_ssize_t size = src.memview.view.itemsize
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         size *= src.shape[i]
  * 
  */
   __pyx_t_2 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1183
+    /* "View.MemoryView":1179
  * 
  *     for i in range(ndim):
  *         size *= src.shape[i]             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size * (__pyx_v_src->shape[__pyx_v_i]));
   }
 
-  /* "View.MemoryView":1185
+  /* "View.MemoryView":1181
  *         size *= src.shape[i]
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1188
+/* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -14036,121 +13992,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1197
+  /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1198
+    /* "View.MemoryView":1194
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride = stride * shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1195
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride = stride * shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1200
+      /* "View.MemoryView":1196
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1202
+  /* "View.MemoryView":1198
  *             stride = stride * shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride = stride * shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1199
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride = stride * shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1204
+      /* "View.MemoryView":1200
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1206
+  /* "View.MemoryView":1202
  *             stride = stride * shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1188
+  /* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1209
+/* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -14163,222 +14119,222 @@
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1221
+  /* "View.MemoryView":1217
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1219
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1224
+  /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1225
+    /* "View.MemoryView":1221
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1225, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1221, __pyx_L1_error)
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1224
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1225
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1230
+  /* "View.MemoryView":1226
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1227
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1232
+    /* "View.MemoryView":1228
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1234
+  /* "View.MemoryView":1230
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1238
+  /* "View.MemoryView":1234
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1239
+    /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1240
+      /* "View.MemoryView":1236
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1242
+  /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1243
+    /* "View.MemoryView":1239
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1245
+  /* "View.MemoryView":1241
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1247
+  /* "View.MemoryView":1243
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1209
+  /* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -14394,15 +14350,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1252
+/* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -14414,57 +14370,57 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1255
+  /* "View.MemoryView":1251
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1250
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(1, 1254, __pyx_L1_error)
+  __PYX_ERR(1, 1250, __pyx_L1_error)
 
-  /* "View.MemoryView":1252
+  /* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -14479,15 +14435,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1258
+/* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -14500,26 +14456,26 @@
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1259
+  /* "View.MemoryView":1255
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -14529,22 +14485,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 1259, __pyx_L1_error)
+  __PYX_ERR(1, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -14560,15 +14516,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1262
+/* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -14582,32 +14538,32 @@
   PyObject *__pyx_t_5 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1263
+  /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1264
+    /* "View.MemoryView":1260
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1264, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -14615,43 +14571,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1264, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 1264, __pyx_L1_error)
+    __PYX_ERR(1, 1260, __pyx_L1_error)
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1266
+  /* "View.MemoryView":1262
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(1, 1266, __pyx_L1_error)
+    __PYX_ERR(1, 1262, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -14667,15 +14623,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1269
+/* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -14694,119 +14650,119 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1278
+  /* "View.MemoryView":1274
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1276
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1277
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1282
+  /* "View.MemoryView":1278
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1285
+  /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1282
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1287
+  /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1288
+    /* "View.MemoryView":1284
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1290
+  /* "View.MemoryView":1286
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -14814,420 +14770,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1292
+  /* "View.MemoryView":1288
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1293
+    /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1294
+      /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1291
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1296
+        /* "View.MemoryView":1292
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1298
+      /* "View.MemoryView":1294
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1298, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1294, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1300
+    /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1301
+      /* "View.MemoryView":1297
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1301, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1297, __pyx_L1_error)
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1303
+  /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1305
+    /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1306
+      /* "View.MemoryView":1302
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1304
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1308, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1304, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1309
+    /* "View.MemoryView":1305
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1303
+    /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1311
+  /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1314
+    /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1311
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1316
+    /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1317
+      /* "View.MemoryView":1313
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1319
+    /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1317
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1318
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1319
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1320
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1325
+      /* "View.MemoryView":1321
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1319
+      /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1311
+    /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1327
+  /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1326
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1330, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1326, __pyx_L1_error)
 
-    /* "View.MemoryView":1331
+    /* "View.MemoryView":1327
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1331, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1327, __pyx_L1_error)
 
-    /* "View.MemoryView":1327
+    /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1329
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1330
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1335
+  /* "View.MemoryView":1331
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1333
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1338
+  /* "View.MemoryView":1334
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1269
+  /* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -15243,217 +15199,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1341
+/* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1345
+  /* "View.MemoryView":1341
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1347
+  /* "View.MemoryView":1343
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1344
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1345
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1350
+    /* "View.MemoryView":1346
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1352
+  /* "View.MemoryView":1348
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1349
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1350
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1355
+    /* "View.MemoryView":1351
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1341
+  /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1363
+/* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1367
+  /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1368
+    /* "View.MemoryView":1364
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1363
+  /* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1372
+/* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1375
+  /* "View.MemoryView":1371
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1372
+  /* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1378
+/* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -15462,178 +15418,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1382
+  /* "View.MemoryView":1378
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1383
+    /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1384
+      /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1385
+        /* "View.MemoryView":1381
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1387
+      /* "View.MemoryView":1383
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1389
+    /* "View.MemoryView":1385
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1390
+      /* "View.MemoryView":1386
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1392
+    /* "View.MemoryView":1388
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1378
+  /* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1398
+/* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1397
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1402
+  /* "View.MemoryView":1398
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1404
+  /* "View.MemoryView":1400
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1398
+  /* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1408
+/* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -15642,118 +15598,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1408
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1413
+  /* "View.MemoryView":1409
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1415
+  /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1416
+    /* "View.MemoryView":1412
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1413
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1418
+      /* "View.MemoryView":1414
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1420
+  /* "View.MemoryView":1416
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1421
+      /* "View.MemoryView":1417
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1423
+      /* "View.MemoryView":1419
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1408
+  /* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -16320,17 +16276,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -16431,17 +16384,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -16684,17 +16634,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -16822,17 +16769,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -17005,17 +16949,17 @@
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 39, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 400, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 609, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 828, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -17091,66 +17035,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 418, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 495, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 520, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 570, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__12 = PyTuple_New(1); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_New(1); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 573, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__12, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "(tree fragment)":2
@@ -17168,33 +17112,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "View.MemoryView":682
+  /* "View.MemoryView":678
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__15 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(1, 682, __pyx_L1_error)
+  __pyx_slice__15 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(1, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__15);
   __Pyx_GIVEREF(__pyx_slice__15);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 703, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -17349,61 +17293,53 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
-  #endif
   if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
   if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
   if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -17624,17 +17560,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "qiskit.transpiler.passes.mapping.cython.stochastic_swap.swap_trial")) {
       if (unlikely(PyDict_SetItemString(modules, "qiskit.transpiler.passes.mapping.cython.stochastic_swap.swap_trial", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
   if (unlikely(__Pyx_modinit_type_import_code() != 0)) goto __pyx_L1_error;
   (void)__Pyx_modinit_variable_import_code();
@@ -17771,37 +17707,37 @@
   __pyx_t_2[3] = PyThread_allocate_lock();
   __pyx_t_2[4] = PyThread_allocate_lock();
   __pyx_t_2[5] = PyThread_allocate_lock();
   __pyx_t_2[6] = PyThread_allocate_lock();
   __pyx_t_2[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_2, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":545
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":991
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -18079,15 +18015,15 @@
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
 #endif
@@ -18150,20 +18086,20 @@
     }
     else {
         d = NULL;
         nd = 0;
     }
 #if PY_MAJOR_VERSION >= 3
     result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, kwdefs, closure);
 #else
     result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, closure);
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
```

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.pyx` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/swap_trial.pyx`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.cpp` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.13 */
+/* Generated by Cython 0.29.7 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O2",
@@ -22,16 +22,16 @@
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_13"
-#define CYTHON_HEX_VERSION 0x001D0DF0
+#define CYTHON_ABI "0_29_7"
+#define CYTHON_HEX_VERSION 0x001D07F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -339,21 +339,16 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
-#else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
-#endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
@@ -1052,15 +1047,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1133,15 +1128,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":965
+/* "View.MemoryView":961
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -1251,15 +1246,15 @@
 #endif
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs);
 #else
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
@@ -7932,189 +7927,150 @@
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
+ * 
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "View.MemoryView":374
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
+ *         cdef int i
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
     /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- */
-    goto __pyx_L3;
-  }
-
-  /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- */
-  __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
-  if (__pyx_t_2) {
-
-    /* "View.MemoryView":377
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
- *             Py_DECREF(Py_None)
- * 
- */
-    ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
-
-    /* "View.MemoryView":378
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
- *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
- * 
- *         cdef int i
- */
-    Py_DECREF(Py_None);
-
-    /* "View.MemoryView":375
- *         if self.obj is not None:
- *             __Pyx_ReleaseBuffer(&self.view)
- *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
- * 
- *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
-  __pyx_L3:;
 
-  /* "View.MemoryView":382
+  /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":383
+    /* "View.MemoryView":379
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":384
+      /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":385
+        /* "View.MemoryView":381
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":384
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":387
+          /* "View.MemoryView":383
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":386
+          /* "View.MemoryView":382
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":389
+        /* "View.MemoryView":385
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":384
+        /* "View.MemoryView":380
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":391
+      /* "View.MemoryView":387
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":382
+    /* "View.MemoryView":378
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
@@ -8127,15 +8083,15 @@
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":393
+/* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -8150,107 +8106,107 @@
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":391
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 397, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 393, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 397, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 393, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 397, __pyx_L1_error)
+          else __PYX_ERR(1, 393, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":398
+    /* "View.MemoryView":394
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 398, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 398, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(1, 394, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":397
+    /* "View.MemoryView":393
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":400
+  /* "View.MemoryView":396
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":393
+  /* "View.MemoryView":389
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -8262,15 +8218,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":403
+/* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -8297,143 +8253,143 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":404
+  /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":405
+    /* "View.MemoryView":401
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":404
+    /* "View.MemoryView":400
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":407
+  /* "View.MemoryView":403
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 407, __pyx_L1_error)
+      __PYX_ERR(1, 403, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 407, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 407, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 403, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":410
+  /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 406, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":411
+    /* "View.MemoryView":407
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 411, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":410
+    /* "View.MemoryView":406
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":413
+  /* "View.MemoryView":409
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 413, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(1, 409, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":414
+    /* "View.MemoryView":410
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 414, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":403
+  /* "View.MemoryView":399
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -8448,15 +8404,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":416
+/* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -8481,182 +8437,182 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":417
+  /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":418
+    /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 418, __pyx_L1_error)
+    __PYX_ERR(1, 414, __pyx_L1_error)
 
-    /* "View.MemoryView":417
+    /* "View.MemoryView":413
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":416
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 420, __pyx_L1_error)
+      __PYX_ERR(1, 416, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 420, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(1, 416, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 422, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 418, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":423
+    /* "View.MemoryView":419
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 424, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 420, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":425
+      /* "View.MemoryView":421
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 425, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":424
+      /* "View.MemoryView":420
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":427
+    /* "View.MemoryView":423
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 427, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(1, 423, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":422
+    /* "View.MemoryView":418
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":429
+  /* "View.MemoryView":425
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 429, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":416
+  /* "View.MemoryView":412
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -8673,15 +8629,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":431
+/* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -8696,26 +8652,26 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":432
+  /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":433
+    /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -8723,59 +8679,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":431
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 435, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 431, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":434
+        /* "View.MemoryView":430
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 434, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 430, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":433
+        /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -8784,30 +8740,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":436
+      /* "View.MemoryView":432
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 436, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(1, 432, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":433
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -8816,15 +8772,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":433
+      /* "View.MemoryView":429
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -8837,36 +8793,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":432
+    /* "View.MemoryView":428
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":439
+  /* "View.MemoryView":435
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":427
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -8880,15 +8836,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":441
+/* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -8899,58 +8855,58 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 445, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":446
+  /* "View.MemoryView":442
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 446, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(1, 442, __pyx_L1_error)
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":443
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":445
+  /* "View.MemoryView":441
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_4 = __pyx_memoryview_copy_contents((__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice))[0]), (__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice))[0]), __pyx_t_2, __pyx_t_3, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 445, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_copy_contents((__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice))[0]), (__pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice))[0]), __pyx_t_2, __pyx_t_3, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 441, __pyx_L1_error)
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":437
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -8963,15 +8919,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":449
+/* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -8992,203 +8948,203 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":447
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":456
+  /* "View.MemoryView":452
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
   __pyx_v_dst_slice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice));
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
   __pyx_t_1 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":459
+    /* "View.MemoryView":455
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     __pyx_t_1 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "View.MemoryView":461
+      /* "View.MemoryView":457
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(1, 461, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(1, 457, __pyx_L1_error)
 
-      /* "View.MemoryView":460
+      /* "View.MemoryView":456
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":458
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":458
+    /* "View.MemoryView":454
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":464
+  /* "View.MemoryView":460
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":462
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":467
+    /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":468
+      /* "View.MemoryView":464
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":467
+      /* "View.MemoryView":463
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":470
+    /* "View.MemoryView":466
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 470, __pyx_L6_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 466, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":474
+    /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     __pyx_t_1 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":475
+      /* "View.MemoryView":471
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_2 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 475, __pyx_L6_error)
+      __pyx_t_2 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 471, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "View.MemoryView":474
+      /* "View.MemoryView":470
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":472
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":479
+  /* "View.MemoryView":475
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -9227,15 +9183,15 @@
       __pyx_t_6 = 0; __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0;
       __pyx_lineno = __pyx_t_3; __pyx_clineno = __pyx_t_4; __pyx_filename = __pyx_t_5;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":445
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -9248,15 +9204,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":481
+/* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -9264,36 +9220,36 @@
   char *__pyx_v_itemp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":482
+  /* "View.MemoryView":478
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 482, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(1, 478, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":479
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 483, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":477
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -9306,15 +9262,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":485
+/* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -9333,39 +9289,39 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   size_t __pyx_t_10;
   int __pyx_t_11;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":488
+  /* "View.MemoryView":484
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":491
+  /* "View.MemoryView":487
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 491, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":492
+  /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -9373,24 +9329,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":493
+      /* "View.MemoryView":489
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 493, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 489, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -9399,94 +9355,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 489, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":492
+      /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":497
+    /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":498
+        /* "View.MemoryView":494
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 498, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 494, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":497
+        /* "View.MemoryView":493
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":499
+      /* "View.MemoryView":495
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -9497,52 +9453,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":490
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 494, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 490, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 494, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(1, 490, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 491, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(1, 495, __pyx_L5_except_error)
+      __PYX_ERR(1, 491, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":492
+    /* "View.MemoryView":488
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -9554,15 +9510,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":481
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -9580,15 +9536,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":501
+/* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -9611,88 +9567,88 @@
   PyObject *__pyx_t_10 = NULL;
   char *__pyx_t_11;
   char *__pyx_t_12;
   char *__pyx_t_13;
   char *__pyx_t_14;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":504
+  /* "View.MemoryView":500
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 504, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":509
+  /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":510
+    /* "View.MemoryView":506
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 510, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 506, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":509
+    /* "View.MemoryView":505
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":512
+  /* "View.MemoryView":508
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -9701,102 +9657,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 508, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(1, 514, __pyx_L1_error)
+    __PYX_ERR(1, 510, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":514
+    /* "View.MemoryView":510
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":515
+    /* "View.MemoryView":511
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":501
+  /* "View.MemoryView":497
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -9816,15 +9772,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":518
+/* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -9856,15 +9812,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":519
+  /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -9874,268 +9830,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":520
+    /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 520, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 516, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 520, __pyx_L1_error)
+    __PYX_ERR(1, 516, __pyx_L1_error)
 
-    /* "View.MemoryView":519
+    /* "View.MemoryView":515
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":523
+    /* "View.MemoryView":519
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":518
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":525
+  /* "View.MemoryView":521
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":528
+    /* "View.MemoryView":524
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":527
+    /* "View.MemoryView":523
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":530
+  /* "View.MemoryView":526
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":533
+    /* "View.MemoryView":529
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":532
+    /* "View.MemoryView":528
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":535
+  /* "View.MemoryView":531
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":538
+    /* "View.MemoryView":534
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":537
+    /* "View.MemoryView":533
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":540
+  /* "View.MemoryView":536
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":538
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":543
+  /* "View.MemoryView":539
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":540
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":541
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":542
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":543
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":518
+  /* "View.MemoryView":514
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -10157,15 +10113,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":553
+/* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -10186,49 +10142,49 @@
   struct __pyx_memoryviewslice_obj *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":554
+  /* "View.MemoryView":550
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 554, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 554, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(1, 550, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":551
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 555, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 551, __pyx_L1_error)
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":552
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":553
+  /* "View.MemoryView":549
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -10240,15 +10196,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":559
+/* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -10266,42 +10222,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":560
+  /* "View.MemoryView":556
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":559
+  /* "View.MemoryView":555
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":563
+/* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -10325,41 +10281,41 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":564
+  /* "View.MemoryView":560
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 564, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 560, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 564, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":563
+  /* "View.MemoryView":559
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -10371,15 +10327,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":567
+/* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -10404,73 +10360,73 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":568
+  /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 570, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 570, __pyx_L1_error)
+    __PYX_ERR(1, 566, __pyx_L1_error)
 
-    /* "View.MemoryView":568
+    /* "View.MemoryView":564
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":568
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 572, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(1, 568, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":567
+  /* "View.MemoryView":563
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -10482,15 +10438,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":575
+/* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -10515,77 +10471,77 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":576
+  /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":577
+    /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 573, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":576
+    /* "View.MemoryView":572
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":575
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 579, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(1, 575, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":575
+  /* "View.MemoryView":571
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -10597,15 +10553,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":582
+/* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -10624,29 +10580,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":583
+  /* "View.MemoryView":579
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":582
+  /* "View.MemoryView":578
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -10657,15 +10613,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":586
+/* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -10684,29 +10640,29 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":587
+  /* "View.MemoryView":583
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":586
+  /* "View.MemoryView":582
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -10717,15 +10673,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":590
+/* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -10746,35 +10702,35 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":591
+  /* "View.MemoryView":587
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 591, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":590
+  /* "View.MemoryView":586
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -10787,15 +10743,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":594
+/* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -10821,98 +10777,98 @@
   int __pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":595
+  /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":596
+    /* "View.MemoryView":592
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":594
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 598, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 594, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":599
+      /* "View.MemoryView":595
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 599, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 595, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":601
+    /* "View.MemoryView":597
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":595
+    /* "View.MemoryView":591
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":603
+  /* "View.MemoryView":599
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":594
+  /* "View.MemoryView":590
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -10925,15 +10881,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":605
+/* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -10952,68 +10908,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":606
+  /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":607
+    /* "View.MemoryView":603
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":606
+    /* "View.MemoryView":602
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":609
+  /* "View.MemoryView":605
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":601
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":611
+/* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -11034,64 +10990,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":609
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 613, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":612
+  /* "View.MemoryView":608
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":607
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -11104,15 +11060,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":615
+/* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -11132,43 +11088,43 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_14__str__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":616
+  /* "View.MemoryView":612
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 616, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":611
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -11180,15 +11136,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":619
+/* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -11209,38 +11165,38 @@
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":622
+  /* "View.MemoryView":618
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
   __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":623
+  /* "View.MemoryView":619
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 623, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":619
+  /* "View.MemoryView":615
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -11251,15 +11207,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":625
+/* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -11280,38 +11236,38 @@
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":628
+  /* "View.MemoryView":624
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
   __pyx_v_mslice = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp));
 
-  /* "View.MemoryView":629
+  /* "View.MemoryView":625
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 629, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":621
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -11322,15 +11278,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":631
+/* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -11352,57 +11308,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":629
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":631
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":636
+  /* "View.MemoryView":632
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 632, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":641
+  /* "View.MemoryView":637
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 641, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":627
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -11413,15 +11369,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":643
+/* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -11444,57 +11400,57 @@
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":641
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":643
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":648
+  /* "View.MemoryView":644
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 648, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 644, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":653
+  /* "View.MemoryView":649
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 653, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":639
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -11612,15 +11568,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":657
+/* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -11629,64 +11585,64 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":658
+  /* "View.MemoryView":654
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 658, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":655
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":656
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":657
+  /* "View.MemoryView":653
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -11700,54 +11656,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":663
+/* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":664
+  /* "View.MemoryView":660
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":663
+  /* "View.MemoryView":659
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":666
+/* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -11770,243 +11726,243 @@
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":671
+  /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":672
+    /* "View.MemoryView":668
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 668, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":671
+    /* "View.MemoryView":667
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":674
+  /* "View.MemoryView":670
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":672
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 676, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":677
+  /* "View.MemoryView":673
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":674
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 675, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 675, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 679, __pyx_L1_error)
+          else __PYX_ERR(1, 675, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 679, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 675, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":680
+    /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":681
+      /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":682
+        /* "View.MemoryView":678
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__17);
             __Pyx_GIVEREF(__pyx_slice__17);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 682, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 678, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":679
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":681
+        /* "View.MemoryView":677
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":685
+      /* "View.MemoryView":681
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 685, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 681, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":686
+      /* "View.MemoryView":682
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":680
+      /* "View.MemoryView":676
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":688
+    /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -12018,40 +11974,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":689
+        /* "View.MemoryView":685
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 689, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 685, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(1, 689, __pyx_L1_error)
+        __PYX_ERR(1, 685, __pyx_L1_error)
 
-        /* "View.MemoryView":688
+        /* "View.MemoryView":684
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":691
+      /* "View.MemoryView":687
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -12062,120 +12018,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":692
+      /* "View.MemoryView":688
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 688, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":679
+    /* "View.MemoryView":675
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":694
+  /* "View.MemoryView":690
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 694, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 690, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":695
+  /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":696
+    /* "View.MemoryView":692
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__17);
         __Pyx_GIVEREF(__pyx_slice__17);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 696, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 692, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":695
+    /* "View.MemoryView":691
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":698
+  /* "View.MemoryView":694
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 698, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":662
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -12193,15 +12149,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":700
+/* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -12212,60 +12168,60 @@
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":701
+  /* "View.MemoryView":697
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":702
+    /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":703
+      /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 703, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 699, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(1, 703, __pyx_L1_error)
+      __PYX_ERR(1, 699, __pyx_L1_error)
 
-      /* "View.MemoryView":702
+      /* "View.MemoryView":698
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":696
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -12278,15 +12234,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":710
+/* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -12319,529 +12275,529 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":711
+  /* "View.MemoryView":707
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":718
+  /* "View.MemoryView":714
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":722
+  /* "View.MemoryView":718
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 722, __pyx_L1_error)
+      __PYX_ERR(1, 718, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":725
+    /* "View.MemoryView":721
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 725, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 721, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":722
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":724
+    /* "View.MemoryView":720
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":728
+  /* "View.MemoryView":724
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":729
+    /* "View.MemoryView":725
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":735
+  /* "View.MemoryView":731
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":736
+  /* "View.MemoryView":732
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":741
+  /* "View.MemoryView":737
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":742
+  /* "View.MemoryView":738
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":746
+  /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 742, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 746, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 742, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 742, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 746, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 742, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 746, __pyx_L1_error)
+          else __PYX_ERR(1, 742, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":747
+    /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":751
+      /* "View.MemoryView":747
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 751, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 747, __pyx_L1_error)
 
-      /* "View.MemoryView":748
+      /* "View.MemoryView":744
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 748, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 744, __pyx_L1_error)
 
-      /* "View.MemoryView":747
+      /* "View.MemoryView":743
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":754
+    /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":755
+      /* "View.MemoryView":751
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":752
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":753
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":754
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":754
+      /* "View.MemoryView":750
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":760
+    /* "View.MemoryView":756
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 756, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 760, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 756, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 760, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 756, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":761
+      /* "View.MemoryView":757
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 757, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 761, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 757, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 761, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 757, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":762
+      /* "View.MemoryView":758
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 758, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 758, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 758, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":760
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 760, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":765
+      /* "View.MemoryView":761
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 765, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 761, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":762
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":764
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 768, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 764, __pyx_L1_error)
 
-      /* "View.MemoryView":774
+      /* "View.MemoryView":770
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":746
+    /* "View.MemoryView":742
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":776
+  /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":774
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 778, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 774, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":775
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 779, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(1, 775, __pyx_L1_error) }
 
-    /* "View.MemoryView":777
+    /* "View.MemoryView":773
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 777, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 773, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 777, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 773, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":776
+    /* "View.MemoryView":772
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":782
+  /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":783
+    /* "View.MemoryView":779
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 782, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":782
+    /* "View.MemoryView":778
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 782, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(1, 778, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":710
+  /* "View.MemoryView":706
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -12855,15 +12811,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":807
+/* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -12871,95 +12827,95 @@
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":827
+  /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":830
+      /* "View.MemoryView":826
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":829
+      /* "View.MemoryView":825
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":828
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 832, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 828, __pyx_L1_error)
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":827
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":827
+    /* "View.MemoryView":823
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":835
+  /* "View.MemoryView":831
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -12970,15 +12926,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":837
+    /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -12988,639 +12944,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":838
+      /* "View.MemoryView":834
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 838, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 834, __pyx_L1_error)
 
-      /* "View.MemoryView":837
+      /* "View.MemoryView":833
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":841
+    /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":842
+      /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":843
+        /* "View.MemoryView":839
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":845
+          /* "View.MemoryView":841
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":844
+          /* "View.MemoryView":840
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":842
+        /* "View.MemoryView":838
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":846
+      /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":847
+        /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":848
+          /* "View.MemoryView":844
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":843
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":850
+        /* "View.MemoryView":846
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":842
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":841
+      /* "View.MemoryView":837
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":852
+    /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":853
+        /* "View.MemoryView":849
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":848
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":855
+      /* "View.MemoryView":851
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":857
+    /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":858
+      /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":859
+        /* "View.MemoryView":855
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":861
+          /* "View.MemoryView":857
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":860
+          /* "View.MemoryView":856
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":858
+        /* "View.MemoryView":854
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":862
+      /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":863
+        /* "View.MemoryView":859
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":858
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":853
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":865
+    /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":866
+        /* "View.MemoryView":862
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":861
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":868
+      /* "View.MemoryView":864
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":870
+    /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":871
+      /* "View.MemoryView":867
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":866
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":875
+    /* "View.MemoryView":871
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":878
+      /* "View.MemoryView":874
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":877
+      /* "View.MemoryView":873
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":880
+    /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":881
+      /* "View.MemoryView":877
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":876
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":884
+    /* "View.MemoryView":880
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":885
+    /* "View.MemoryView":881
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":882
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":889
+  /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":890
+    /* "View.MemoryView":886
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":889
+    /* "View.MemoryView":885
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":892
+  /* "View.MemoryView":888
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":895
+    /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":896
+      /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":897
+        /* "View.MemoryView":893
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":896
+        /* "View.MemoryView":892
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":899
+      /* "View.MemoryView":895
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":900
+        /* "View.MemoryView":896
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 899, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 895, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":895
+      /* "View.MemoryView":891
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":902
+    /* "View.MemoryView":898
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":894
+    /* "View.MemoryView":890
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":904
+  /* "View.MemoryView":900
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":807
+  /* "View.MemoryView":803
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -13636,15 +13592,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":910
+/* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -13658,280 +13614,280 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":908
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":913
+  /* "View.MemoryView":909
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":916
+  /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":917
+    /* "View.MemoryView":913
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(1, 917, __pyx_L1_error)
+      __PYX_ERR(1, 913, __pyx_L1_error)
     }
     __pyx_v_shape = __Pyx_div_Py_ssize_t(__pyx_v_view->len, __pyx_v_itemsize);
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":914
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":916
+    /* "View.MemoryView":912
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":920
+  /* "View.MemoryView":916
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":921
+    /* "View.MemoryView":917
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":922
+    /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":923
+      /* "View.MemoryView":919
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":922
+      /* "View.MemoryView":918
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":925
+  /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":926
+    /* "View.MemoryView":922
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":928
+      /* "View.MemoryView":924
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 928, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 924, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 928, __pyx_L1_error)
+      __PYX_ERR(1, 924, __pyx_L1_error)
 
-      /* "View.MemoryView":927
+      /* "View.MemoryView":923
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":925
+    /* "View.MemoryView":921
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":930
+  /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":931
+    /* "View.MemoryView":927
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 931, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 931, __pyx_L1_error)
+    __PYX_ERR(1, 927, __pyx_L1_error)
 
-    /* "View.MemoryView":930
+    /* "View.MemoryView":926
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":933
+  /* "View.MemoryView":929
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":934
+  /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":935
+    /* "View.MemoryView":931
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":934
+    /* "View.MemoryView":930
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":937
+  /* "View.MemoryView":933
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":910
+  /* "View.MemoryView":906
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -13942,15 +13898,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":943
+/* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -13967,90 +13923,90 @@
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
 
-  /* "View.MemoryView":944
+  /* "View.MemoryView":940
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":942
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":947
+  /* "View.MemoryView":943
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":951
+  /* "View.MemoryView":947
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = __Pyx_div_long(__pyx_v_ndim, 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":952
+    /* "View.MemoryView":948
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":953
+    /* "View.MemoryView":949
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":950
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -14060,44 +14016,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":957
+      /* "View.MemoryView":953
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 953, __pyx_L1_error)
 
-      /* "View.MemoryView":956
+      /* "View.MemoryView":952
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":959
+  /* "View.MemoryView":955
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":943
+  /* "View.MemoryView":939
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -14113,15 +14069,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":976
+/* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -14136,100 +14092,100 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":977
+  /* "View.MemoryView":973
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":976
+  /* "View.MemoryView":972
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":979
+/* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":980
+  /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":981
+    /* "View.MemoryView":977
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 981, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 977, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":980
+    /* "View.MemoryView":976
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":983
+  /* "View.MemoryView":979
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 979, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":975
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -14240,15 +14196,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":985
+/* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -14256,58 +14212,58 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":986
+  /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":987
+    /* "View.MemoryView":983
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 987, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(1, 983, __pyx_L1_error)
 
-    /* "View.MemoryView":986
+    /* "View.MemoryView":982
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":989
+  /* "View.MemoryView":985
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 989, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 985, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":981
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -14320,15 +14276,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":992
+/* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -14346,27 +14302,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":993
+  /* "View.MemoryView":989
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":992
+  /* "View.MemoryView":988
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -14480,15 +14436,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":999
+/* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -14505,351 +14461,351 @@
   Py_buffer __pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1007
+  /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1008
+    /* "View.MemoryView":1004
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1007
+    /* "View.MemoryView":1003
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1013
+  /* "View.MemoryView":1009
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1011
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1016
+  /* "View.MemoryView":1012
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1014
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1018, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1014, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1019
+  /* "View.MemoryView":1015
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1017
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1022
+  /* "View.MemoryView":1018
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1019
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1020
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1021
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1028
+    /* "View.MemoryView":1024
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1027
+    /* "View.MemoryView":1023
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1030
+  /* "View.MemoryView":1026
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1028
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1033
+  /* "View.MemoryView":1029
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1036
+  /* "View.MemoryView":1032
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1037
+  /* "View.MemoryView":1033
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1038
+    /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1039
+      /* "View.MemoryView":1035
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1036
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1038
+      /* "View.MemoryView":1034
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1042
+  /* "View.MemoryView":1038
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1043
+  /* "View.MemoryView":1039
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1043, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1039, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1044
+    /* "View.MemoryView":1040
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1044, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 1040, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1046
+  /* "View.MemoryView":1042
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1047
+  /* "View.MemoryView":1043
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1045
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":999
+  /* "View.MemoryView":995
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -14863,15 +14819,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1052
+/* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
@@ -14880,79 +14836,79 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1055
+  /* "View.MemoryView":1051
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1056
+    /* "View.MemoryView":1052
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1056, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(1, 1052, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1053
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1055
+    /* "View.MemoryView":1051
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1059
+  /* "View.MemoryView":1055
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1060
+    /* "View.MemoryView":1056
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1052
+  /* "View.MemoryView":1048
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice):
  *     cdef _memoryviewslice obj
  */
 
@@ -14963,15 +14919,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1063
+/* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -14984,158 +14940,158 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1067
+  /* "View.MemoryView":1063
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1068
+  /* "View.MemoryView":1064
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1065
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1067
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1072
+  /* "View.MemoryView":1068
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1070
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1075
+    /* "View.MemoryView":1071
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1076
+    /* "View.MemoryView":1072
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1073
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1063
+  /* "View.MemoryView":1059
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1080
+/* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
 static PyObject *__pyx_memoryview_copy_object(struct __pyx_memoryview_obj *__pyx_v_memview) {
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1083
+  /* "View.MemoryView":1079
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1084
+  /* "View.MemoryView":1080
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1084, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1080, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1080
+  /* "View.MemoryView":1076
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -15146,15 +15102,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1087
+/* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -15166,99 +15122,99 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *(*__pyx_t_3)(char *);
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1094
+  /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1095
+    /* "View.MemoryView":1091
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1092
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1094
+    /* "View.MemoryView":1090
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1098
+  /* "View.MemoryView":1094
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1099
+    /* "View.MemoryView":1095
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1101
+  /* "View.MemoryView":1097
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1099
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1101, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1097, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1087
+  /* "View.MemoryView":1083
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -15269,81 +15225,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1109
+/* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1110
+  /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1111
+    /* "View.MemoryView":1107
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1110
+    /* "View.MemoryView":1106
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1113
+  /* "View.MemoryView":1109
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1109
+  /* "View.MemoryView":1105
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1116
+/* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -15353,187 +15309,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1121
+  /* "View.MemoryView":1117
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1122
+  /* "View.MemoryView":1118
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1120
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1125
+    /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1126
+      /* "View.MemoryView":1122
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1123
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1125
+      /* "View.MemoryView":1121
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1129
+  /* "View.MemoryView":1125
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1130
+    /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1131
+      /* "View.MemoryView":1127
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1128
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1130
+      /* "View.MemoryView":1126
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1134
+  /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1135
+    /* "View.MemoryView":1131
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1134
+    /* "View.MemoryView":1130
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1137
+  /* "View.MemoryView":1133
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1116
+  /* "View.MemoryView":1112
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1140
+/* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -15546,61 +15502,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1147
+  /* "View.MemoryView":1143
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1148
+  /* "View.MemoryView":1144
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1145
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1146
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -15612,195 +15568,195 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1150
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1153
+    /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1151
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1153
+      /* "View.MemoryView":1149
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1157
+    /* "View.MemoryView":1153
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1158
+        /* "View.MemoryView":1154
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1159
+        /* "View.MemoryView":1155
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1156
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1152
+    /* "View.MemoryView":1148
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1162
+  /* "View.MemoryView":1158
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1163
+      /* "View.MemoryView":1159
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1167
+      /* "View.MemoryView":1163
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1168
+      /* "View.MemoryView":1164
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1140
+  /* "View.MemoryView":1136
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1170
+/* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1173
+  /* "View.MemoryView":1169
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1170
+  /* "View.MemoryView":1166
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1177
+/* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  */
 
@@ -15809,70 +15765,70 @@
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1180
+  /* "View.MemoryView":1176
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  *     cdef Py_ssize_t size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1182
+  /* "View.MemoryView":1178
  *     cdef Py_ssize_t size = src.memview.view.itemsize
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         size *= src.shape[i]
  * 
  */
   __pyx_t_2 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1183
+    /* "View.MemoryView":1179
  * 
  *     for i in range(ndim):
  *         size *= src.shape[i]             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size * (__pyx_v_src->shape[__pyx_v_i]));
   }
 
-  /* "View.MemoryView":1185
+  /* "View.MemoryView":1181
  *         size *= src.shape[i]
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1177
+  /* "View.MemoryView":1173
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef int i
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1188
+/* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -15880,121 +15836,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1197
+  /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1198
+    /* "View.MemoryView":1194
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride = stride * shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1199
+      /* "View.MemoryView":1195
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride = stride * shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1200
+      /* "View.MemoryView":1196
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1197
+    /* "View.MemoryView":1193
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1202
+  /* "View.MemoryView":1198
  *             stride = stride * shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride = stride * shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1203
+      /* "View.MemoryView":1199
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride = stride * shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1204
+      /* "View.MemoryView":1200
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride = stride * shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1206
+  /* "View.MemoryView":1202
  *             stride = stride * shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1188
+  /* "View.MemoryView":1184
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1209
+/* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -16007,222 +15963,222 @@
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
 
-  /* "View.MemoryView":1220
+  /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1221
+  /* "View.MemoryView":1217
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1223
+  /* "View.MemoryView":1219
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1224
+  /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1225
+    /* "View.MemoryView":1221
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1225, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 1221, __pyx_L1_error)
 
-    /* "View.MemoryView":1224
+    /* "View.MemoryView":1220
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1228
+  /* "View.MemoryView":1224
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1225
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1230
+  /* "View.MemoryView":1226
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1231
+    /* "View.MemoryView":1227
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1232
+    /* "View.MemoryView":1228
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1234
+  /* "View.MemoryView":1230
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1238
+  /* "View.MemoryView":1234
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1239
+    /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1240
+      /* "View.MemoryView":1236
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1239
+      /* "View.MemoryView":1235
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1242
+  /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1243
+    /* "View.MemoryView":1239
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1242
+    /* "View.MemoryView":1238
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1245
+  /* "View.MemoryView":1241
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1247
+  /* "View.MemoryView":1243
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1209
+  /* "View.MemoryView":1205
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -16238,15 +16194,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1252
+/* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -16258,57 +16214,57 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1255
+  /* "View.MemoryView":1251
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1254
+  /* "View.MemoryView":1250
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1254, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(1, 1254, __pyx_L1_error)
+  __PYX_ERR(1, 1250, __pyx_L1_error)
 
-  /* "View.MemoryView":1252
+  /* "View.MemoryView":1248
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -16323,15 +16279,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1258
+/* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -16344,26 +16300,26 @@
   PyObject *__pyx_t_4 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1259
+  /* "View.MemoryView":1255
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -16373,22 +16329,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1259, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 1259, __pyx_L1_error)
+  __PYX_ERR(1, 1255, __pyx_L1_error)
 
-  /* "View.MemoryView":1258
+  /* "View.MemoryView":1254
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -16404,15 +16360,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1262
+/* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -16426,32 +16382,32 @@
   PyObject *__pyx_t_5 = NULL;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1263
+  /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1264
+    /* "View.MemoryView":1260
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1264, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -16459,43 +16415,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1264, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 1264, __pyx_L1_error)
+    __PYX_ERR(1, 1260, __pyx_L1_error)
 
-    /* "View.MemoryView":1263
+    /* "View.MemoryView":1259
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1266
+  /* "View.MemoryView":1262
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(1, 1266, __pyx_L1_error)
+    __PYX_ERR(1, 1262, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1262
+  /* "View.MemoryView":1258
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -16511,15 +16467,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1269
+/* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -16538,119 +16494,119 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
 
-  /* "View.MemoryView":1277
+  /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1278
+  /* "View.MemoryView":1274
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1280
+  /* "View.MemoryView":1276
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1277
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1282
+  /* "View.MemoryView":1278
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1285
+  /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1282
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1285
+    /* "View.MemoryView":1281
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1287
+  /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1288
+    /* "View.MemoryView":1284
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1283
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1290
+  /* "View.MemoryView":1286
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -16658,420 +16614,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1292
+  /* "View.MemoryView":1288
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1293
+    /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1294
+      /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1291
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1296
+        /* "View.MemoryView":1292
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1294
+        /* "View.MemoryView":1290
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1298
+      /* "View.MemoryView":1294
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1298, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1294, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1293
+      /* "View.MemoryView":1289
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1300
+    /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1301
+      /* "View.MemoryView":1297
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1301, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 1297, __pyx_L1_error)
 
-      /* "View.MemoryView":1300
+      /* "View.MemoryView":1296
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1303
+  /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1305
+    /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1306
+      /* "View.MemoryView":1302
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1305
+      /* "View.MemoryView":1301
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1308
+    /* "View.MemoryView":1304
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1308, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(1, 1304, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1309
+    /* "View.MemoryView":1305
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1303
+    /* "View.MemoryView":1299
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1311
+  /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1314
+    /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1311
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1314
+      /* "View.MemoryView":1310
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1316
+    /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1317
+      /* "View.MemoryView":1313
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1312
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1319
+    /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1321
+      /* "View.MemoryView":1317
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1318
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1319
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1320
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1325
+      /* "View.MemoryView":1321
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1319
+      /* "View.MemoryView":1315
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1311
+    /* "View.MemoryView":1307
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1327
+  /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1330
+    /* "View.MemoryView":1326
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1330, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1326, __pyx_L1_error)
 
-    /* "View.MemoryView":1331
+    /* "View.MemoryView":1327
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1331, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(1, 1327, __pyx_L1_error)
 
-    /* "View.MemoryView":1327
+    /* "View.MemoryView":1323
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1333
+  /* "View.MemoryView":1329
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1330
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1335
+  /* "View.MemoryView":1331
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1337
+  /* "View.MemoryView":1333
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1338
+  /* "View.MemoryView":1334
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1269
+  /* "View.MemoryView":1265
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -17087,217 +17043,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1341
+/* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1345
+  /* "View.MemoryView":1341
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1347
+  /* "View.MemoryView":1343
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1348
+    /* "View.MemoryView":1344
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1345
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1350
+    /* "View.MemoryView":1346
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1352
+  /* "View.MemoryView":1348
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1353
+    /* "View.MemoryView":1349
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1350
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1355
+    /* "View.MemoryView":1351
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1341
+  /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1363
+/* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1367
+  /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1368
+    /* "View.MemoryView":1364
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1367
+    /* "View.MemoryView":1363
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1363
+  /* "View.MemoryView":1359
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1372
+/* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1375
+  /* "View.MemoryView":1371
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1372
+  /* "View.MemoryView":1368
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1378
+/* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -17306,178 +17262,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1382
+  /* "View.MemoryView":1378
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1383
+    /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1384
+      /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1385
+        /* "View.MemoryView":1381
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1384
+        /* "View.MemoryView":1380
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1387
+      /* "View.MemoryView":1383
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1383
+      /* "View.MemoryView":1379
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1389
+    /* "View.MemoryView":1385
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1390
+      /* "View.MemoryView":1386
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1392
+    /* "View.MemoryView":1388
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1378
+  /* "View.MemoryView":1374
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1398
+/* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1401
+  /* "View.MemoryView":1397
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1402
+  /* "View.MemoryView":1398
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1404
+  /* "View.MemoryView":1400
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1398
+  /* "View.MemoryView":1394
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1408
+/* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -17486,118 +17442,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1412
+  /* "View.MemoryView":1408
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1413
+  /* "View.MemoryView":1409
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1415
+  /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1416
+    /* "View.MemoryView":1412
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1417
+      /* "View.MemoryView":1413
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1418
+      /* "View.MemoryView":1414
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1415
+    /* "View.MemoryView":1411
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1420
+  /* "View.MemoryView":1416
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1421
+      /* "View.MemoryView":1417
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1423
+      /* "View.MemoryView":1419
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1408
+  /* "View.MemoryView":1404
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -18101,17 +18057,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection __pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection;
 
 static PyObject *__pyx_tp_new_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -18206,17 +18159,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -18387,17 +18337,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -18498,17 +18445,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -18751,17 +18695,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18889,17 +18830,14 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
-  0, /*tp_vectorcall*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"nlayout_from_layout", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_1nlayout_from_layout, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_nlayout_from_layout},
   {0, 0, 0, 0}
 };
 
@@ -19068,17 +19006,17 @@
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 58, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 180, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 183, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 133, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 400, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 609, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 828, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -19173,66 +19111,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":414
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 418, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "View.MemoryView":495
+  /* "View.MemoryView":491
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 495, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":516
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 520, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":566
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 570, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":573
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 573, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
@@ -19250,33 +19188,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "View.MemoryView":682
+  /* "View.MemoryView":678
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(1, 682, __pyx_L1_error)
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(1, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__17);
   __Pyx_GIVEREF(__pyx_slice__17);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":699
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 703, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -19434,87 +19372,75 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout = &__pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout;
   __pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.copy = (struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout *(*)(struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout *))__pyx_f_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_7NLayout_copy;
   __pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.swap = (void (*)(struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout *, unsigned int, unsigned int))__pyx_f_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_7NLayout_swap;
   __pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.to_layout = (PyObject *(*)(struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout *, PyObject *, int __pyx_skip_dispatch))__pyx_f_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_7NLayout_to_layout;
   if (PyType_Ready(&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.tp_dictoffset && __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout.tp_dict, __pyx_vtabptr_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_NLayout, (PyObject *)&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
   __pyx_ptype_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout = &__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_NLayout;
   __pyx_vtabptr_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection = &__pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection;
   __pyx_vtable_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.add = (void (*)(struct __pyx_obj_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection *, unsigned int, unsigned int, int __pyx_skip_dispatch))__pyx_f_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_14EdgeCollection_add;
   if (PyType_Ready(&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.tp_dictoffset && __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection.tp_dict, __pyx_vtabptr_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_EdgeCollection, (PyObject *)&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_ptype_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection = &__pyx_type_6qiskit_10transpiler_6passes_7mapping_6cython_15stochastic_swap_5utils_EdgeCollection;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
-  #endif
   if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
   if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
   if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
-  #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 965, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(1, 961, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -19722,17 +19648,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "qiskit.transpiler.passes.mapping.cython.stochastic_swap.utils")) {
       if (unlikely(PyDict_SetItemString(modules, "qiskit.transpiler.passes.mapping.cython.stochastic_swap.utils", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   if (unlikely(__Pyx_modinit_function_export_code() != 0)) goto __pyx_L1_error;
   if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
@@ -19921,37 +19847,37 @@
   __pyx_t_3[3] = PyThread_allocate_lock();
   __pyx_t_3[4] = PyThread_allocate_lock();
   __pyx_t_3[5] = PyThread_allocate_lock();
   __pyx_t_3[6] = PyThread_allocate_lock();
   __pyx_t_3[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_3, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":545
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":991
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 991, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -20093,15 +20019,15 @@
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
 #if 1 || PY_VERSION_HEX < 0x030600B1
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, int nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
 #endif
@@ -20164,20 +20090,20 @@
     }
     else {
         d = NULL;
         nd = 0;
     }
 #if PY_MAJOR_VERSION >= 3
     result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, kwdefs, closure);
 #else
     result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
+                               args, nargs,
                                k, (int)nk,
                                d, (int)nd, closure);
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
```

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pxd` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pxd`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pyx` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/cython/stochastic_swap/utils.pyx`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/dense_layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/dense_layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/enlarge_with_ancilla.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/enlarge_with_ancilla.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/full_ancilla_allocation.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/full_ancilla_allocation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/lookahead_swap.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/lookahead_swap.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/noise_adaptive_layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/noise_adaptive_layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/set_layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/set_layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/stochastic_swap.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/stochastic_swap.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/mapping/trivial_layout.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/mapping/trivial_layout.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/merge_adjacent_barriers.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/merge_adjacent_barriers.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/num_qubits.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/num_qubits.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/num_tensor_factors.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/num_tensor_factors.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/optimize_1q_gates.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/optimize_1q_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/optimize_swap_before_measure.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/optimize_swap_before_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/remove_diagonal_gates_before_measure.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/remove_diagonal_gates_before_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/remove_reset_in_zero_state.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/remove_reset_in_zero_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/resource_estimation.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/resource_estimation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/size.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/size.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/unroll_3q_or_more.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/unroll_3q_or_more.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/unroller.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/unroller.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passes/width.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passes/width.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/passmanager.py` & `qiskit-terra-0.9.1/qiskit/transpiler/passmanager.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level0.py` & `qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level0.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level1.py` & `qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level1.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level2.py` & `qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level2.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/preset_passmanagers/level3.py` & `qiskit-terra-0.9.1/qiskit/transpiler/preset_passmanagers/level3.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/propertyset.py` & `qiskit-terra-0.9.1/qiskit/transpiler/propertyset.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/synthesis/__init__.py` & `qiskit-terra-0.9.1/qiskit/transpiler/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/synthesis/graysynth.py` & `qiskit-terra-0.9.1/qiskit/transpiler/synthesis/graysynth.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/transpile_circuit.py` & `qiskit-terra-0.9.1/qiskit/transpiler/transpile_circuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/transpiler/transpile_config.py` & `qiskit-terra-0.9.1/qiskit/transpiler/transpile_config.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/user_config.py` & `qiskit-terra-0.9.1/qiskit/user_config.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/util.py` & `qiskit-terra-0.9.1/qiskit/util.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/__init__.py` & `qiskit-terra-0.9.1/qiskit/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/base.py` & `qiskit-terra-0.9.1/qiskit/validation/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/exceptions.py` & `qiskit-terra-0.9.1/qiskit/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/fields/__init__.py` & `qiskit-terra-0.9.1/qiskit/validation/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/fields/containers.py` & `qiskit-terra-0.9.1/qiskit/validation/fields/containers.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/fields/custom.py` & `qiskit-terra-0.9.1/qiskit/validation/fields/custom.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/fields/polymorphic.py` & `qiskit-terra-0.9.1/qiskit/validation/fields/polymorphic.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/jsonschema/__init__.py` & `qiskit-terra-0.9.1/qiskit/validation/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/jsonschema/exceptions.py` & `qiskit-terra-0.9.1/qiskit/validation/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/jsonschema/schema_validation.py` & `qiskit-terra-0.9.1/qiskit/validation/jsonschema/schema_validation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/validation/validate.py` & `qiskit-terra-0.9.1/qiskit/validation/validate.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/version.py` & `qiskit-terra-0.9.1/qiskit/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/__init__.py` & `qiskit-terra-0.9.1/qiskit/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/bloch.py` & `qiskit-terra-0.9.1/qiskit/visualization/bloch.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/circuit_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/circuit_visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/counts_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/counts_visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/dag_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/dag_visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/exceptions.py` & `qiskit-terra-0.9.1/qiskit/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/gate_map.py` & `qiskit-terra-0.9.1/qiskit/visualization/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/__init__.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_blochsphere.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_blochsphere.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_cities.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_cities.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_hinton.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_hinton.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_histogram.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_histogram.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_paulivec.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_paulivec.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/interactive/iplot_qsphere.py` & `qiskit-terra-0.9.1/qiskit/visualization/interactive/iplot_qsphere.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/latex.py` & `qiskit-terra-0.9.1/qiskit/visualization/latex.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/matplotlib.py` & `qiskit-terra-0.9.1/qiskit/visualization/matplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,18 @@
         else:
             wid = WID
 
         if fc:
             _fc = fc
         else:
             if self._style.name != 'bw':
-                _fc = self._style.dispcol['multi']
+                if self._style.gc != DefaultStyle().gc:
+                    _fc = self._style.gc
+                else:
+                    _fc = self._style.dispcol['multi']
                 _ec = self._style.dispcol['multi']
             else:
                 _fc = self._style.gc
 
         qubit_span = abs(ypos) - abs(ypos_max) + 1
         height = HIG + (qubit_span - 1)
         box = patches.Rectangle(
@@ -234,14 +237,16 @@
             else:
                 boxes_wide = round(len(text) / 10) or 1
                 wid = WID * 2.2 * boxes_wide
         else:
             wid = WID
         if fc:
             _fc = fc
+        elif self._style.gc != DefaultStyle().gc:
+            _fc = self._style.gc
         elif text and text in self._style.dispcol:
             _fc = self._style.dispcol[text]
         else:
             _fc = self._style.gc
 
         box = patches.Rectangle(
             xy=(xpos - 0.5 * wid, ypos - 0.5 * HIG), width=wid, height=HIG,
@@ -378,26 +383,32 @@
 
         box = patches.Circle(xy=(xpos, ypos), radius=WID * 0.15,
                              fc=_fc, ec=self._style.lc,
                              linewidth=1.5, zorder=PORDER_GATE)
         self.ax.add_patch(box)
 
     def _ctrl_qubit(self, xy, fc=None, ec=None):
+        if self._style.gc != DefaultStyle().gc:
+            fc = self._style.gc
+            ec = self._style.gc
         if fc is None:
             fc = self._style.lc
         if ec is None:
             ec = self._style.lc
         xpos, ypos = xy
         box = patches.Circle(xy=(xpos, ypos), radius=WID * 0.15,
                              fc=fc, ec=ec,
                              linewidth=1.5, zorder=PORDER_GATE)
         self.ax.add_patch(box)
 
     def _tgt_qubit(self, xy, fc=None, ec=None, ac=None,
                    add_width=None):
+        if self._style.gc != DefaultStyle().gc:
+            fc = self._style.gc
+            ec = self._style.gc
         if fc is None:
             fc = self._style.dispcol['target']
         if ec is None:
             ec = self._style.lc
         if ac is None:
             ac = self._style.lc
         if add_width is None:
@@ -585,20 +596,20 @@
                              zorder=PORDER_LINE)
                 self.ax.text(0.5, y + .1, str(this_creg['val']), ha='left',
                              va='bottom',
                              fontsize=0.8 * self._style.fs,
                              color=self._style.tc,
                              clip_on=True,
                              zorder=PORDER_TEXT)
-            self.ax.text(-0.5, y, this_creg['label'], ha='right', va='center',
+            self.ax.text(self.x_offset, y, this_creg['label'], ha='right', va='center',
                          fontsize=1.5*self._style.fs,
                          color=self._style.tc,
                          clip_on=True,
                          zorder=PORDER_TEXT)
-            self._line([0, y], [self._cond['xmax'], y], lc=self._style.cc,
+            self._line([self.x_offset + 0.5, y], [self._cond['xmax'], y], lc=self._style.cc,
                        ls=self._style.cline, zorder=PORDER_REGLINE)
 
         # lf line
         if feedline_r:
             self._linefeed_mark((self._style.fold + 1 - 0.1,
                                  - n_fold * (self._cond['n_lines'] + 1)))
         if feedline_l:
@@ -723,15 +734,15 @@
                     param = None
                 # conditional gate
                 if op.condition:
                     c_xy = [c_anchors[ii].plot_coord(this_anc, layer_width, self.x_offset) for
                             ii in self._creg_dict]
                     mask = 0
                     for index, cbit in enumerate(self._creg):
-                        if cbit.reg == op.condition[0]:
+                        if cbit.register == op.condition[0]:
                             mask |= (1 << index)
                     val = op.condition[1]
                     # cbit list to consider
                     fmt_c = '{{:0{}b}}'.format(len(c_xy))
                     cmask = list(fmt_c.format(mask))[::-1]
                     # value
                     fmt_v = '{{:0{}b}}'.format(cmask.count('1'))
```

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/pass_manager_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/pass_manager_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
+
+# pylint: disable=invalid-name
+
 """
 Visualization function for a pass manager. Passes are grouped based on their
 flow controller, and coloured based on the type of pass.
 """
 import os
 import inspect
 import tempfile
@@ -29,29 +32,14 @@
 from qiskit.visualization import utils
 from qiskit.visualization.exceptions import VisualizationError
 from qiskit.transpiler.basepasses import AnalysisPass, TransformationPass
 
 DEFAULT_STYLE = {AnalysisPass: 'red',
                  TransformationPass: 'blue'}
 
-try:
-    import subprocess
-
-    _PROC = subprocess.Popen(['dot', '-V'], stdout=subprocess.PIPE,
-                             stderr=subprocess.PIPE)
-    _PROC.communicate()
-    if _PROC.returncode != 0:
-        HAS_GRAPHVIZ = False
-    else:
-        HAS_GRAPHVIZ = True
-except Exception:  # pylint: disable=broad-except
-    # this is raised when the dot command cannot be found, which means GraphViz
-    # isn't installed
-    HAS_GRAPHVIZ = False
-
 
 def pass_manager_drawer(pass_manager, filename, style=None, raw=False):
     """
     Draws the pass manager.
 
     This function needs `pydot <https://github.com/erocarrera/pydot>`, which in turn needs
     Graphviz <https://www.graphviz.org/>` to be installed.
@@ -71,14 +59,29 @@
                            no image was generated or PIL is not installed.
     Raises:
         ImportError: when nxpd or pydot not installed.
         VisualizationError: If raw=True and filename=None.
     """
 
     try:
+        import subprocess
+
+        _PROC = subprocess.Popen(['dot', '-V'], stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE)
+        _PROC.communicate()
+        if _PROC.returncode != 0:
+            HAS_GRAPHVIZ = False
+        else:
+            HAS_GRAPHVIZ = True
+    except Exception:  # pylint: disable=broad-except
+        # this is raised when the dot command cannot be found, which means GraphViz
+        # isn't installed
+        HAS_GRAPHVIZ = False
+
+    try:
         import pydot
         if not HAS_GRAPHVIZ:
             raise ImportError
     except ImportError:
         raise ImportError("pass_manager_drawer requires pydot and graphviz. "
                           "Run 'pip install pydot'. "
                           "Graphviz can be installed using 'brew install graphviz' on Mac"
```

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/pulse/interpolation.py` & `qiskit-terra-0.9.1/qiskit/visualization/pulse/interpolation.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/pulse/matplotlib.py` & `qiskit-terra-0.9.1/qiskit/visualization/pulse/matplotlib.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/pulse/qcstyle.py` & `qiskit-terra-0.9.1/qiskit/visualization/pulse/qcstyle.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/pulse_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/pulse_visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/qcstyle.py` & `qiskit-terra-0.9.1/qiskit/visualization/qcstyle.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/state_visualization.py` & `qiskit-terra-0.9.1/qiskit/visualization/state_visualization.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/text.py` & `qiskit-terra-0.9.1/qiskit/visualization/text.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/tools/__init__.py` & `qiskit-terra-0.9.1/qiskit/visualization/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/tools/pi_check.py` & `qiskit-terra-0.9.1/qiskit/visualization/tools/pi_check.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit/visualization/utils.py` & `qiskit-terra-0.9.1/qiskit/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/qiskit_terra.egg-info/PKG-INFO` & `qiskit-terra-0.9.1/qiskit_terra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-terra
-Version: 0.9.0
+Version: 0.9.1
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit-terra
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-terra/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
@@ -21,9 +21,9 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
-Provides-Extra: full-featured-simulators
 Provides-Extra: visualization
+Provides-Extra: full-featured-simulators
```

### Comparing `qiskit-terra-0.9.0/qiskit_terra.egg-info/SOURCES.txt` & `qiskit-terra-0.9.1/qiskit_terra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-terra-0.9.0/setup.py` & `qiskit-terra-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from Cython.Build import cythonize
 except ImportError:
     import subprocess
     subprocess.call([sys.executable, '-m', 'pip', 'install', 'Cython>=0.27.1'])
     from Cython.Build import cythonize
 
 REQUIREMENTS = [
-    "jsonschema>=2.6,<2.7",
+    "jsonschema>=2.6",
     "marshmallow>=2.17.0,<3",
     "marshmallow_polyfield>=3.2,<4",
     "networkx>=2.2",
     "numpy>=1.13",
     "ply>=3.10",
     "psutil>=5",
     "scipy>=1.0",
@@ -66,15 +66,15 @@
                     extra_link_args=LINK_FLAGS,
                     language='c++')
     EXT_MODULES.append(mod)
 
 
 setup(
     name="qiskit-terra",
-    version="0.9.0",
+    version="0.9.1",
     description="Software for developing quantum computing programs",
     long_description="""Terra provides the foundations for Qiskit. It allows the user to write
         quantum circuits easily, and takes care of the constraints of real hardware.""",
     url="https://github.com/Qiskit/qiskit-terra",
     author="Qiskit Development Team",
     author_email="qiskit@qiskit.org",
     license="Apache 2.0",
```

