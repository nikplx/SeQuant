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
- [THC-MP2 trace form](./thc_mp2_trace.json): staged tensor-valued results
  (`thc/e2.inp`, `thc/w.inp`, `thc/energy.inp`) expressing the THC-based MP2
  Coulomb term as build-`E2`, single-`W = E2·Z` contraction, trace of `W²`.
  Run-only (no blessed-output comparison).
