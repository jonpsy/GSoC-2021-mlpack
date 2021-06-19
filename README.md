<p align="center">
<a href="https://summerofcode.withgoogle.com/"><img style="padding: 20px;" alt="drawing" src="pics/GSoC_logo.png" height="200"></a>
<a href="https://www.mlpack.org/"><img style="padding: 20px;" alt="drawing" src="pics/mlpack.png" height="200"></a>
</p>

My proposal for **A Framework for Multiobjective optimizers** was selected under **Google Summer of Code 2021**. I'll work with the [mlpack](https://mlpack.org/) organization under the mentorship of **Marcus Edel** ([@zoq](https://github.com/zoq)), **Sayan Goswami** ([@say4n](https://github.com/say4n)), **James Balamuta** ([@coatless](https://github.com/coatless)).

Honoring the rites of mlpack, I will post my progress, results, visualizations over the course of my contribution.
<figure>
  <img src="https://docs.google.com/uc?export=download&id=1OHRslfH6qnT-Sqi5-PWFtEeihef-CeGH" width="400" height="400">
  <figcaption align="centre">Fig. 1: - The truncate operator of SPEA-II </figcaption>
</figure>

<a href="https://github.com/mlpack/ensmallen/pull/293"><img style="padding: 5px;" alt="drawing" src="pics/PBI.jpeg" height="600"></a>

<a href="https://github.com/mlpack/ensmallen/pull/295"><img style="padding: 5px;" alt="drawing" src="pics/das-dennis.png" height="300"></a>


## Motivation

The [ensmallen](https://github.com/mlpack/ensmallen) library comes under the umbrella of ```mlpack``` repository. It's a header-only library written in C++ for numerical optimization.```mlpack``` relies heavily on this library for optimizers, callbacks and utilities.
f
The ```ensmallen``` library boasts an extensive set of optimizers that has focused exclusively on single-objective problem sets in the past. Attempts were made in the past, by [Sayan Goswami](https://github.com/mlpack/ensmallen/pull/149) and [Rahul Prabhu](https://github.com/mlpack/ensmallen/pull/120)  on introducing MultiObjective Optimizer(MOO) to this library. These were met with varying degrees of success. It became clear that the library needed to adapt to tackle this unique challenge.

Building upon this foundation, the proposal aims to add cutting edge MOO optimizers, expand the test framework, add type traits, rework callbacks, write documentations to make the library flexible for MultiObjective use cases. The end product would integrate these features seamlessly into the codebase, to work in coherence with the existing interface.

## Pull Requests

### I. Pre-GSoC

* [Improvise Non Dominated Sorting Algorithm - II (NSGA-II)](https://github.com/mlpack/ensmallen/pull/263).
* [Added Indicators to assess MOO Optimizer performance](https://github.com/mlpack/ensmallen/pull/285).
* [Expand CheckArbitraryFunctionTypeAPI to work for MOO](https://github.com/mlpack/ensmallen/pull/283).
* [ZDT Test Suite](https://github.com/mlpack/ensmallen/pull/273).

### II. Community Bonding

 * [Added utility to generate stocks data](https://github.com/mlpack/examples/pull/152).
 * [Add Portfolio Optimization notebook](https://github.com/mlpack/examples/pull/155).
 * [Expand callbacks for MOO Case](https://github.com/mlpack/ensmallen/pull/289).


 ## A note of thanks

 I would like to thank these people without whom, this project wouldn't have been possible. Shaikh Mohammad Fauz  ([@FieryBlade-313](https://github.com/FieryBlade-313)) for the gif and Sagar Sehgal ([@Sagar](https://github.com/thesagarsehgal)) for the guidance.
