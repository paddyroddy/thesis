# Slepian Wavelets for the Analysis of Incomplete Manifolds 

[![thesis PDF](https://img.shields.io/badge/thesis-PDF-blue.svg)](https://www.dropbox.com/s/5t3pon5nagnm5tl/patrick_roddy_thesis.pdf?dl=0)
[![deploy](https://github.com/paddyroddy/phd_thesis/actions/workflows/deploy.yml/badge.svg)](https://github.com/paddyroddy/phd_thesis/actions/workflows/deploy.yml)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

## Abstract

Many fields in science and engineering measure data that inherently live on
non-Euclidean geometries, such as the sphere. Techniques developed in the
Euclidean setting must be extended to other geometries. Due to recent interest
in geometric deep learning, analogues of Euclidean techniques must also handle
general manifolds or graphs. Often, data are only observed over partial regions
of manifolds, and thus standard whole-manifold techniques may not yield accurate
predictions. In this thesis, a new wavelet basis is designed for datasets like
these.

Although many definitions of spherical convolutions exist, none fully emulate
the Euclidean definition. A novel spherical convolution is developed, designed
to tackle the shortcomings of existing methods. The so-called sifting
convolution exploits the sifting property of the Dirac delta and follows by the
inner product of a function with the translated version of another. This
translation operator is analogous to the Euclidean translation in harmonic space
and exhibits some useful properties. In particular, the sifting convolution
supports directional kernels; has an output that remains on the sphere; and is
efficient to compute. The convolution is entirely generic and thus may be used
with any set of basis functions. An application of the sifting convolution with
a topographic map of the Earth demonstrates that it supports directional kernels
to perform anisotropic filtering.

Slepian wavelets are built upon the eigenfunctions of the Slepian concentration
problem of the manifold - a set of bandlimited functions which are maximally
concentrated within a given region. Wavelets are constructed through a tiling of
the Slepian harmonic line by leveraging the existing scale-discretised
framework. A straightforward denoising formalism demonstrates a boost in
signal-to-noise for both a spherical and general manifold example. Whilst these
wavelets were inspired by spherical datasets, like in cosmology, the wavelet
construction may be utilised for manifold or graph data.

## Compilation

Simply run `latexmk` at the top level.

## Formatting

To install `pre-commit` hooks locally, execute `pip install pre-commit`
followed by `pre-commit install`. This only needs to be done once per repo,
and from then on checks are made whenever committing. See steps
[here](https://pre-commit.com/#automatically-enabling-pre-commit-on-repositories)
to enable these checks always.
