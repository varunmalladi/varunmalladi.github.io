---
permalink: /
excerpt: "Programming"
author_profile: true
redirect_from: 
  - /programming/
  - /programming.html
---

## DARTS Ray Tracing Engine
_C++_

My extension to the Dartmouth Academic Ray Tracing Skeleton. This project implements features such as parametric surfaces and meshes, 
Monte Carlo integration, and multiple importance sampling. For the final rendering competition my partner and I received special 
mention for the following render:

![](images/darts_fp.jpeg)

There are two major features on display here. First, the skin is rendered using volumetric scattering techniques. Second, the glowing 
facial material is fluorescent; the primary light source in the scene is actually the dark hand. It is emitting light outside the 
visible spectrum, which the fluorescent materials picks up and re-emits within the visible spectrum.

## ekki Graphics Frontend
_Rust + wgpu_

I realized while working on my ray tracer that a lot of boilerplate and debugging was spent on parsing scenes and displaying results. 
Even when this worked it was difficult to edit the scene files, considering they were all json. My goal with this project is to 
provide a common frontend that programs like ray tracers can use to visualize their input and output, and through which they can be
easily invoked.

![](images/ekki.jpeg)

The project is still in its early stages. I'm currently working on the infrastructure to load C dynamic libraries at runtime, which is
how I imagine a computationally expensive program would be invoked through the frontend.
