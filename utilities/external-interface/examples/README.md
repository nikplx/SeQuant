# External interface examples

The driver files in this directory reference input expressions (diagrams) in text form, that will be read in and processed by SeQuant according to the
driver's specification.

Example invocation:
```
./external_interface --driver ccsd.json
```

Available examples:
- [CCSD](./ccsd.json)
- [NEVPT2](./nevpt2.json)
- [MP2](./mp2.json): canonical spin-orbital MP2 energy from antisymmetrized
  ERIs (`mp2/mp2_gd.inp`, `mp2/mp2_energy.inp`), exported both as ITF
  (`mp2.itfaa`) and as runnable NumPy/`einsum` code (`mp2.py`).
  Run-only (no blessed-output comparison).
