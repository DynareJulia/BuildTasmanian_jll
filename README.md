# BuildTasmanian_jll

This repository is for testing and tracking changes in the recipe needed to build Tasmanian_jll

When a new version is ready, copy `build_tarballs.jl` Yggdrasil.jl/T/Tasmaninan in your own fork of Yggdrasil and open a PR

## Running the `build_tarballs.jl` script

- Make sure that `BinaryBuilder.jl` is added to Julia default environment
- To (cross-)compile and build for a basic Linux installation on a x86_64 machine, run from the terminal command line
```
  julia --color=yes  build_tarballs.jl x86_64-linux-gnu --debug --verbose
```
- To cross-compile and build for a x86_64 MacOS installation, run from the terminal command line
```
  julia --color=yes  build_tarballs.jl x86_64-apple-darwin --debug --verbose
```
- To cross-compile and build for all plateforms supported by Julia, run from the terminal command line
```
  julia --color=yes  build_tarballs.jl --debug --verbose
```

## Testing the artifact locally

See the [BinaryBuilder documentation](https://docs.binarybuilder.org/stable/building/#Building-a-custom-JLL-package-locally)

## Cleaning up

The above procedure creates the `build` and `products` directories that you can remove after having verified them if necessary.

## Open issues:
- link the Tasmanian library with `libblastrampoline_jll` to get accelerate BLAS and LAPACK
- link with CUDA
