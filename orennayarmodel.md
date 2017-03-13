---
layout: home
title: Oren Nayar Model
---
---
## Disadvantages of other model
 
  For modelling a smooth surface such as matte, there is an easy model called Lambertian Model, which assumes that the light diffuses evenly in all direction. The result of this model is an object which looks equally illuminated in all directions. 
  
  {% include figure.html image="https://puu.sh/uvclH/f9a0fc6ab8.PNG" caption="Lambertian Model : direction 1" position="left" %}
  
  {% include figure.html image="https://puu.sh/uvclI/6a3c60b80c.PNG" caption="Lambertian Model : direction 1" position="right" %}
  
  This works well on smooth surface but not for rough surface, because irregular bumps, or called “microfacet”, on the rough surface, will not diffuse the light evenly. 

## Utilizing Oren Nayar Model

  The basic idea of this model is to take the effect of bumps into consideration. It assumes that the microfacet structure on the rough surface are symmetric V-shaped bumps, and the surface of every bump perform perfect Lambertian diffusion. In other words, Oren Nayar model takes the rough surface as a composition of lots of tiny smooth surface, and using the easy model for smooth surface to model a rough surface. The model generated after using Oren Nayar’s algorithm is below.
  
   {% include figure.html image="https://puu.sh/uvcls/eda177746d.PNG" caption="Using Lambertian Model" position="left" %}
   
   {% include figure.html image="https://puu.sh/uvclE/adaef73c48.PNG" caption="Using Oren Nayar Model" position="right" %}