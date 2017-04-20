# ![xtensor](http://quantstack.net/assets/images/xtensor.svg)

[![Travis](https://travis-ci.org/QuantStack/xtensor-blas.svg?branch=master)](https://travis-ci.org/QuantStack/xtensor)
[![Appveyor](https://ci.appveyor.com/api/projects/status/quf1hllkedr0rxbk?svg=true)](https://ci.appveyor.com/project/QuantStack/xtensor)
[![Documentation Status](http://readthedocs.org/projects/xtensor/badge/?version=latest)](https://xtensor.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://img.shields.io/badge/launch-binder-brightgreen.svg)](http://mybinder.org/repo/QuantStack/xtensor/notebooks/notebooks/xtensor.ipynb)
[![Join the Gitter Chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/QuantStack/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Introduction

`xtensor-blas` is an extension to the xtensor library, offering bindings to BLAS and LAPACK libraries 
through cxxblas and cxxlapack from the [FLENS](https://github.com/michael-lehn/FLENS) project.

`xtensor-blas` currently provides non-broadcasting `dot`, `norm` (1- and 2-norm), `inverse`, `solve`,
`eig`, and `cross`.
Low-level functions to interface with BLAS or LAPACK with xtensor containers are also offered 
in the `blas` and `lapack` namespace.

`xtensor` and `xtensor-blas` require a modern C++ compiler supporting C++14. The following C++ compilers are supported:

 - On Windows platforms, Visual C++ 2015 Update 2, or more recent
 - On Unix platforms, gcc 4.9 or a recent version of Clang

## Installation

`xtensor-blas` is a header-only library that depends on `xtensor`, `LAPACK` and `BLAS`.
You can directly install it from the sources:

```bash
git clone https://github.com/QuantStack/xtensor-blas
cd xtensor-blas
mkdir build
cd build
cmake .. -D CMAKE_INSTALL_PREFIX=your_install_prefix  # for tests: -DBUILD_TESTS=ON
make install
```

## License

We use a shared copyright model that enables all contributors to maintain the
copyright on their contributions.

This software is licensed under the BSD-3-Clause license. See the [LICENSE](LICENSE) file for details.