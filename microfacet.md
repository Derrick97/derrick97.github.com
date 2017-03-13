---
layout: home
title: Microfacet Theory
---
---

Microfacet Theory

{% include figure.html image="https://sfault-image.b0.upaiyun.com/6b/da/6bda91dd3fd303e50fca7ba5dc80d1fd_articlex" %}

A physically based specular BRDF is based on micro-facet theory, which describe a surface is composed of many micro-facets and each micro-facet will only reflect light in a single direction according to their normal(m):

So, in the above diagram, for light coming from direction l to be reflected to viewing direction v, the micro-facet normal m must be equals to the half vector between l and v.
A micro-facet BRDF has the following form:

which consists of 3 terms: Fresnel term(F), Distribution term(D) and Geometry term(G). Their meaning can be found in the background talk presented by Naty Hoffman in siggraph 2010. And these 3 terms can be chosen independently as stated in the talk Physically-based lighting in Call of Duty:Black Ops (although "Microfacet Models for Refraction through Rough Surfaces" states that some G depends on D to maintain energy conservation, but some G are extended to handle arbitrary distribution, so in this blog post, I assume that the G function is independent of D). So I decided to find some distribution functions D and geometry functions G and play with different combinations to see how it affects the rendering result. You can also play around with different combinations using the WebGL demo(need a webGL enabled browser such as Chrome) in the last section of the post.
