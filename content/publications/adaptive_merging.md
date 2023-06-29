+++
categories = []
comments = false
date = "2016-10-02T15:59:13-04:00"
draft = false
showpagemeta = false
showcomments = false
slug = ""
tags = ["publication"]
title = "Adaptive Merging for Rigid Body Simulation"
description = ""
+++
###### ACM Transactions on Graphics (SIGGRAPH North America), 2020
[Eulalie Coevoet](https://eulaliecoevoet.com/), **Otman Benchekroun**,  [Paul G. Kry](https://www.cs.mcgill.ca/~kry/),
{{< youtube id="mmVVRVt8EF4" autoplay="false" >}}

[//]: # ({{< figure src=/publications/adaptive_merging/teaser.png width=600 width=600 >}})
We reduce computation time in rigid body simulations by merging collections of bodies when 
they share a common spatial velocity. Merging relies on monitoring the state of contacts, 
and a metric that compares the relative linear and angular motion of bodies based on their sizes. 
Unmerging relies on an inexpensive single iteration projected Gauss-Seidel 
sweep over contacts between merged bodies, which lets us update internal contact forces over time, 
and use the same metrics as merging to identify when bodies should unmerge.
Furthermore we use a contact ordering for graph traversal refinement of the internal 
contact forces in collections, which helps to correctly identify all the bodies that must unmerge
when there are impacts. The general concept of merging is similar to the common technique 
of sleeping and waking rigid bodies in the inertial frame, and we exploit this too, but our 
merging is in moving frames, and unmerging takes place at contacts between bodies rather than 
at the level of bodies themselves. We discuss the previous relative motion metrics in comparison to ours, 
and evaluate our method on a variety of scenarios.

[[acm](https://dl.acm.org/doi/abs/10.1145/3386569.3392417)]

