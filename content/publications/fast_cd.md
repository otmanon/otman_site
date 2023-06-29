+++
categories = []
comments = false
date = "2016-10-02T15:59:13-04:00"
draft = false
showpagemeta = false
showcomments = false
slug = ""
tags = ["publication"]
title = "Fast Complementary Dynamics via Skinning Eigenmodes"
description = ""
+++
###### ACM Transactions on Graphics (SIGGRAPH North America), 2023
 **Otman Benchekroun**, [Jiayi Eris Zhang](https://eriszhang.github.io/) , [Siddhartha Chaudhuri](https://www.cse.iitb.ac.in/~sidch/), [Eitan Grinspun](https://www.dgp.toronto.edu/~eitan/), [Yi Zhou](https://zhouyisjtu.github.io/), [Alec Jacobson](https://www.cs.toronto.edu/~jacobson/)
{{< figure src=/publications/fast_cd/aquarium.jpg width=600 width=600 >}}

We propose a reduced-space elasto-dynamic solver that is well suited for augmenting rigged 
character animations with secondary motion. At the core of our method is a novel deformation
subspace based on Linear Blend Skinning that overcomes many of the shortcomings prior subspace 
methods face. Our skinning subspace is parameterized entirely by a set of scalar weights, which
we can obtain through a small, material-aware and rig-sensitive generalized eigenvalue problem. 
The resulting subspace can easily capture rotational motion and guarantees that the resulting
simulation is rotation equivariant. We further propose a simple local-global solver for linear
co-rotational elasticity and propose a clustering method to aggregate per-tetrahedra non-linear 
energetic quantities. The result is a compact simulation that is
fully decoupled from the complexity of the mesh.

[[low-res](https://arxiv.org/pdf/2303.11886)]

