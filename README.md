# ParametricOptInterface.jl
GSOC 2020 project


| **Documentation** | **Build Status** | **Coverage** |
|:-----------------:|:-----------------:|:-----------------:|
| [![][docs-dev-img]][docs-dev-url]| [![Build Status][build-img]][build-url] | [![Codecov branch][codecov-img]][codecov-url]|

[build-img]: https://travis-ci.com/jump-dev/ParametricOptInterface.jl.svg?branch=master
[build-url]: https://travis-ci.com/jump-dev/ParametricOptInterface

[codecov-img]: http://codecov.io/github/jump-dev/ParametricOptInterface.jl/coverage.svg?branch=master
[codecov-url]: http://codecov.io/github/jump-dev/ParametricOptInterface.jl?branch=master

[docs-dev-img]: https://img.shields.io/badge/docs-dev-blue.svg
[docs-dev-url]: http://jump.dev/ParametricOptInterface.jl/dev/


Repository with implementation allowing parameters in MathOptInterface.jl problems.


## Benchmarking

In the development of ParametricOptInterface.jl it is useful to benchmark the code performance.
To perform benchmark we recommend you compare the performance of the master branch aggaints your 
implementation. Here we leave an example on how to perform the benchmarks the correct way.

```
git checkout master
julia --project=benchmark benchmark/benchmark.jl --new bench
git checkout approach_1
julia --project=benchmark benchmark/benchmark.jl --compare bench
```
