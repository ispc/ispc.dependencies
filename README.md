ISPC build dependencies
=======================

This repo is hosting [ISPC](https://github.com/ispc/ispc) build dependencies to enable fast and reliable downloads in [Github Actions CI](https://github.com/ispc/ispc/actions). The binaries are hosted in this project's [Releases](https://github.com/ispc/ispc.dependencies/releases).

Specifically, the repo contains:
1. LLVM builds, which are built by [alloy.py](https://github.com/ispc/ispc/blob/main/alloy.py) script form ISPC repo. The builds are produced by `rebuild-llvm*.yml` pipelines, which can be found [here](https://github.com/ispc/ispc/tree/main/.github/workflows). These are vanilla LLVM builds configured to support x86, ARM and WASM targets. For some versions patches backported from LLVM trunk are applied, when there are known bugs affecting ISPC, all these patches are applier by `alloy.py` automatically and all these patches are located in ISPC repo [llvm-patches](https://github.com/ispc/ispc/tree/main/llvm_patches) folder. The license for LLVM project can be found [here](https://github.com/llvm/llvm-project/blob/main/LICENSE.TXT). The source code for LLVM project used for the builds is located [here](https://github.com/ispc/llvm-project).
