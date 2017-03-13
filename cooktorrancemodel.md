---
layout: home
title: Cook-Torrance Model
---
---

## Disadvantage of other Models
 
There are several models for modelling the specular reflection of a surface. The earlier one is called Phong Model, which is an empirical model. The basic idea of it is to take this whole process into two parts, one for white specular reflection, and another for color diffuse reflection. This works very well when modelling a plastic thing, but is bad for metallic surface.

{% include figure.html image="https://puu.sh/uvclt/389a73228f.PNG" caption="Phong Model works well on modelling plastic" %}

The reason is that for modelling a plastic, the internal reflection contributes to the diffusion reflection, but for a metal, because it is a conductor, the light hitting on its surface will trigger a reflection of wave, thus most of the reflection happens on the surface rather than in the internal structure. Thus, modelling a metallic surface using Phong model is not ideal.

{% include figure.html image="https://puu.sh/uvclu/be1c251774.PNG" caption="G-Function measures how much light is lost during the reflection" %}





## How does Cook-Torrance Model works?
  
Cook-Torrance Model works with three functions: F, G, D. Function F represents Fresnel Equations, which measures the ratio of light reflection to refraction. Function G represents Geometrical Attenuation Factor, which measures how much light is lost during the refl ection (Graph) In the graph below, we can see that some lights are blocked during the reflection on microfacet, and the G is used to measure this. Function D represents Normal Distribution Function. The basic idea of Normal Distribution Function is to calculate the ratio of microfacet structure on a given direction to all the microfacet structures on the surface. These three functions give the expression of Cook-Torrance Model. 
 
{% include figure.html image="https://puu.sh/uvclp/196b61c09c.PNG" caption="expression of Cook-Torrance Model" %}

The Graph below shows a graph generated using cook-torrance model:

{% include figure.html image="https://puu.sh/uvclq/1a87710725.PNG" caption="Generating Using Cook-Torrance" %}