---
layout: home
title: Basic Knowledge of Radiometry
---

In order to completely understand BRDF Theorem, we need to get the basic knowledge of radiometry.

# Radiometry

  Computer Graphic Technic simulates the interaction between visible light and various materials, which contains the transfer of the energy. Computer Graphic for realistic objects is based on the physical rendering model, while rediometry is the subject that measures the transfer of energy of electromagnetic radiation.
  
## Physical quantity in Radiometry ([see table below](#table1))

### Energy

   Symbol: Q
   
   Unit: J
  
   Energy here represents the energy for photons. Each photon has its own energy, related with frequency. The higher the frequency, the higher the energy.

### Flux (also called Radiant flux)

   Symbol: Φ (specifically in radiometry, which is different from the usual symbol P)
   
   Unit: W (J/s)
   
   Definition: 
   
   <img src="https://puu.sh/uIQPi/b0a77987c5.gif">
   
   Actually, flux refers to the power. However, it is called Flux (or Radiant Flux) in Radiometry. It measures the total energy goes through a surface or area per unit time.

### Irradiance

   Symbol: E
   
   Unit: 
   <img src="https://puu.sh/uIQi9/428088dba8.gif">

   
   Definition: 
   
   <img src="https://puu.sh/uIQYo/ee212a8c4e.gif">
   
   Irradiance measures the radiation energy reaching per unit area per unit time, or flux reaching per unit area. We can understand it as the density of flux to area. 
   
   Hence the received energy for sphere:  
   
   <img src="https://puu.sh/uIQAA/23b5db00c5.gif">
   
### Radiant Existance

   It is also called Radiosity. Represent by Symbol M. it is similar with irradiance. The only difference is that irradiance measures the flux density reaching the surface while radiant existance measures the flux density leaving the surface.
   
### Radiant Intensity

   Symbol: I
   
   Unit: W/sr
   
   Definition:
   
   <img src="https://puu.sh/uIRyl/b5af4d9a4c.gif">
   
   It measures the flux per solid angle. 

### Radiance

  Symbol: L
  
  Unit: <img src="https://puu.sh/uISB3/5654d5c895.gif">
  
  Definition:
  
  <img src="https://puu.sh/uISK4/a7e01404bf.gif">
  
  Radiance is the flux density per unit area per unit solid angle. The area here is the prjection area in the direction perpendicular to the light.
  
  Radiance can be consider as the colour we actually see from a point on an object. In Physical-based Graphic rendering, the computer computes the radiance to get the colour of the point. 
  
  <div>
  These basic physical quantity is collected in the following table below:
  <a id="table1">
   {% include mytable.html %}
   </a>
</div>
## BRDF Model

the BRDF model measures the ratio of the irritance of the incident beam and the reflectance of the reflected beam. it described how much energy of specific wavelength of light is transferred to a specific given direction in the reflective surface.

  
  
  
