# BuildTasmanian_jll

This repository is for testing and tracking changes in the recipe needed to build Tasmanian_jll

When a new version is ready, copy `build_tarballs.jl` to Yggdrasil.jl/T/Tasmaninan and open a PR

## Open issues:
- link the Tasmanian library with `libblastrampoline_jll` to get accelerate BLAS and LAPACK
- link with CUDA
