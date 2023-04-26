---
date: "2023-04-28T13:00:00"
speaker: Bram Vanhecke
affiliation: University of Vienna, Austria
title: "PEPS optimization with AD: the perils of an easy tool"
type: lunchtalk
abstract: true
---

The past few years it has become clear that the best way to optimize a PEPS wavefunction is through the variational principle. To that end one should be able calculate the gradient of the energy. At first, people developed methods to get an approximation of this gradient #channels, but more recently people have used automatic differentiation (AD) -a programmatic tool developed for AI- to get the exact gradient. While this represents a definite improvement, it also comes with a plethora of difficulties and shortcommings seemingly inate to the approach. We will discuss these issues and show how all of them are mere artefacts of using AD as a black box, and may hence be solved with a slightly more hands on approach. 
