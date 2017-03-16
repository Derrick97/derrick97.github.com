---
layout: home
title: Microfacet Theory
---
---

Microfacet Theory

{% include figure.html image="https://puu.sh/uKl9C/7f42464401.png" caption="microsurface vs macrosurface" %}

Microfacet theory regards the point on the surfaces is composed by many mirco-surfaces with different direction. Those microfacet all have their normals, as the diagram above shows. In our macro-world, we normally consider the surface of a object as a smooth, flat plane. The n obviously illustrate the normal of the macrosurface. However, base on the Microfacet theory, the macrosurface can be reconstructed as microsurfaces. m is one of their normals which is shown above.  

{% include figure.html image="https://puu.sh/uKkYb/fd3329ba1d.png" caption="incident and reflected light according to the normals" %}

For incoming light with direction l, if it incidents onto the microsurface with normal h, then it would be reflected to direction v and be viewed by our eyes. And the reflected light would be in direction v if and only if the normal of the microsurface bisects the angle between l and v. The the total amount of reflected light in direction v of a given surface must be constant. Hence we need to know the normal distribution of the microsurfaces of a macrosurface to calculate the intensity of the reflected light in a given viewed angle.

A microfacet BRDF consists of 3 terms: Fresnel term(F), Distribution term(D) and Geometry term(G). 

Fresnel term(F) states the ratio between reflected light and refracted light which is absorbed by the surface itself since not all the incident light would be reflected by the surface. 

The Distribution term(D), or we called Normal Distribution Function (NDF) describes the probability distribution of the normal of all microfacets that compose the point on the surface. If we give a direction d to NDF, then it would return the ratio of the microfacet whose normal is in direction d to all microfacets. 

However, not all the microfacet can successfully receive and reflect light. There are three circumstances that could happen when light incidents into the microsurface. One is called shadowing, Since some incident light would be blocked out when coming in. Similarly, the another one is called masking, which the reflected light would be blocked. And the third one says that some light would reflected inside microfacets internally. Those three circumstances are all illustrated in the diagram below.

{% include figure.html image="https://puu.sh/uvclu/be1c251774.PNG" caption="Masking, Shading and inter-reflection" %}

The Geometry Term(G) measures the ratio of the light which can be seen in given direction to all incident light in another direction. 