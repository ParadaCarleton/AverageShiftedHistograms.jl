| Docs | Build | Test |
|------|-------|------|
| [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://joshday.github.io/AverageShiftedHistograms.jl/stable) [![](https://img.shields.io/badge/docs-latest-blue.svg)](https://joshday.github.io/AverageShiftedHistograms.jl/latest) | [![CI](https://github.com/joshday/AverageShiftedHistograms.jl/actions/workflows/CI.yml/badge.svg)](https://github.com/joshday/AverageShiftedHistograms.jl/actions/workflows/CI.yml) | [![codecov.io](http://codecov.io/github/joshday/AverageShiftedHistograms.jl/coverage.svg?branch=master)](http://codecov.io/github/joshday/AverageShiftedHistograms.jl?branch=master)



<h1 align="center">
  AverageShiftedHistograms.jl
</h1>

<p align="center">
  <strong>⚡ Lightning fast density estimation in Julia ⚡</strong>
</p>

An Averaged Shifted Histogram (ASH) is essentially Kernel Density Estimation over a fine-partition histogram.  ASH uses **constant memory**, can be constructed on-line via **O(nbins)** updates, and lets you estimate densities for **arbitrarily big data**.

<p align="center">
  <img src="https://user-images.githubusercontent.com/8075494/54132735-20e89600-43eb-11e9-9915-c9d588f64308.gif">
</p>




## Quickstart:

```julia
import Pkg

Pkg.add("AverageShiftedHistograms")

using AverageShiftedHistograms

ash(randn(10^6))
```
