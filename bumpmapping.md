---
layout: home
title: Bump Mapping
---
---
When modelling a surface using Microfacet Models, the roughness of the surface is an extremely important parameter in the BRDF. In real world, the illumination will change when the object or light resources are moving. Using other mapping technique, such as texture mapping, however, cannot illustrate the roughness very successfully. It always appears smoothly no matter how the object or light sources move. Bump mapping is a powerful technique for solving this problem.
   
## Basic Idea of bump mapping
  
To simulate a realistic rough surface, bump mapping adds a bump function on the normal direction of the surface. This such algorithm that generalizes rough surfaces into bumps with bump functions on the normal direction is called Perturbation.

## Why Bump Mapping Works?
  
Because the effect of the bumps on the reflection is mainly due to the normal direction, thus such method can ensure that the illumination will be changed once the object move because the normal of the bump is also moving, which will make the object looks not always smooth as what texture mapping will do. At the same time, this method also preserve the original geometric features of the object, so the work of reworking on the geometry of the object are not needed, thus save a great amount of time and memory.

