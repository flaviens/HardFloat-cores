# HardFloat Cores

This repository contains FuseSoC cores for [the HardFloat repository](https://github.com/bsg-external/HardFloat).
The goal is to provide a simpler and more reliable dependency system than git submodules.
In the future, testing could also be converted to FuseSoC.

## How to test the cores?

1. Make sure to have fusesoc installed.

```
pip install fusesoc
```

2. Clone the directory

```
git clone https://github.com/flaviens/HardFloat-cores
cd HardFloat-cores
```

3. Add the local dir as a FuseSoC library

```
fusesoc library add hardfloat_cores .
```

4. Run the lint test (this test is far from comprehensive). This requires Verilator to be installed.

```
fusesoc run --target=lint_compareRecFN hardfloat_riscv
```
