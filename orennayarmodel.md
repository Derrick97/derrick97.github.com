---
layout: home
title: Oren Nayar Model
---
---
 
## Disadvantages of other model
 
  For modelling a smooth surface such as matte, there is an easy model called Lambertian Model, which assumes that the light diffuses evenly in all direction. The result of this model is an object which looks equally illuminated in all directions (Lambert 1, Lambert 2). This works well on smooth surface but not for rough surface, because irregular bumps, or called “microfacet”, on the rough surface, will not diffuse the light evenly. 

## Utilizing Oren Nayar Model

  The basic idea of this model is to take the effect of bumps into consideration. It assumes that the microfacet structure on the rough surface are symmetric V-shaped bumps, and the surface of every bump perform perfect Lambertian diffusion. In other words, Oren Nayar model takes the rough surface as a composition of lots of tiny smooth surface, and using the easy model for smooth surface to model a rough surface. The model generated after using Oren Nayar’s algorithm is below.
