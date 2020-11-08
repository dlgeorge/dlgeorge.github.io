---
title: 'The 2014 Oso, WA disaster'
subtitle: 'modeling alternative scenarios and mobility with D-Claw'
date: 2015-01-01 00:00:00
description: Computations of the 2014 Oso, WA disaster reveal mobility bifurcations related to initial and critical porosities.
featured_image: '/images/projects/oso/Oso_arial_photo_Cover.jpg'
---

### D-Claw modeling of the 2014, Oso, Washington landslide disaster reveals potential mobility bifurcations due to initial material parameters.


This page features material and excerpts from:

**Landslides that liquefy: modeling mobility bifurcation and the 2014 Oso, Washington, USA disaster.** R.M. Iverson, D.L. George, 2016. *Geotechnique*, V. 66(3), 175--187. [pdf]({{ site.baseurl }}/pubs/IversonGeorge2016_Geotechnique_Oso.pdf)

see also:

**Landslide mobility and hazards: implications of the 2014 Oso disaster.** R.M. Iverson, D.L. George, et al., 2015. *Earth Planet. Sci. Lett.*, V. 412, pp. 197--208. [pdf]({{ site.baseurl }}/pubs/IversonGeorgeEtAl2015_EPSL_Oso.pdf)

![](/images/projects/oso/Oso_arial_photo.jpg)

---
#### Abstract
<small>
Some landslides move slowly or intermittently downslope, but others liquefy during the early stages of motion, leading to runaway acceleration and high-speed runout across low-relief terrain. Mechanisms responsible for this disparate behaviour are represented in a two-phase, depth-integrated, landslide dynamics model that melds principles from soil mechanics, granular mechanics and fluid mechanics. The model assumes that gradually increasing pore-water pressure causes slope failure to nucleate at the weakest point on a basal slip surface in a statically balanced mass. Failure then spreads to adjacent regions as a result of momentum exchange. Liquefaction is contingent on pore-pressure feedback that depends on the initial soil state. The importance of this feedback is illustrated by using the model to study the dynamics of a disastrous landslide that occurred near Oso, Washington, USA, on 22 March 2014. Alternative simulations of the event reveal the pronounced effects of a landslide mobility bifurcation that occurs if the initial void ratio of water-saturated soil equals the lithostatic, critical-state void ratio. They also show that the tendency for bifurcation increases as the soil permeability decreases. The bifurcation implies that it can be difficult to discriminate conditions that favour slow landsliding from those that favour liquefaction and long runout.
</small>

---
#### D-Claw modeling of landslide dynamics at Oso

D-Claw is used to study the dynamics of a large, high mobility landslide that occurred following a long period of unusually wet weather near Oso, Washington, USA, on 22 March 2014. The landslide (officially named the SR 530 landslide by Washington State) caused 43 fatalities, ranking it second only to a 1985 event in Mameyes, Puerto Rico, as the worst landslide disaster in US history (cf. Jibson, 1992). Results of a multidisciplinary investigation of the landslide’s behaviour are presented elsewhere (Iverson et al., 2015). 

---
<figure>
<figcaption> Figure 1. Overhead view comparing D-Claw results (blue) for baseline parameters compared with observed runout (outlined in yellow: fine line: debris avalance deposit and slump block. thick line: debris-flow runout).</figcaption>
<div class="gallery" data-columns="2">
    <img src="{{ site.baseurl }}/images/projects/oso/OsoDClawMapCompare_small.jpg">
</div>
</figure>
---

D-Claw considers the gravity driven motion of fluid-filled granular mixtures that can undergo dilation and contraction during both quasi-static and inertial deformation. The model employs depth integrated continuum mechanical equations that blend concepts from critical-state soil mechanics, fluid mechanics and granular mechanics. Iverson & George (2014) provide a comprehensive derivation of the model equations, and George & Iverson (2014) describe the numerical method of solving the equations, as well as tests of model predictions against data from large-scale experiments. 

---
<figure>
<figcaption>Figure 2. Overhead view of the simulated behaviour of the Oso landslide using the baseline parameter values for the material parameters used in Iverson et al, 2015, providing the best fit. Landslide area is shown by shading with intensity of the shading inversely
proportional to the degree of basal liquefaction.</figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/oso/DClaw6panel_Geotechnique.png">
</div>
</figure>
---

####  Landslide source initialization for D-Claw modeling

Estimation of the total volume of the Oso landslide required differencing the 2013 and 2014 lidar topography, but also required reconstruction of the landslide’s basal slip-surface geometry. This reconstruction was necessary because considerable landslide debris remained in the source area at the conclusion of the event. Three alternative reconstructions yielded source-area volume estimates ranging from 7-9 million cubic meters, with the intermediate volume deemed most plausible (Iverson et al., 2015). This basal slip surface reconstruction, along with the 2013 lidar topography, also established the initial geometry used in the model simulations presented here.

---
<figure>
<figcaption>Figure 3. Landslide source geometries were construced with the aid of pre- and post-event lidar. Buried deposits required fitting a failure surface to availabe data, based on logarithmic spirials---a commonly assumed basal profile in lieu of further data. </figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/oso/OsoDClawLogSpiralSources.png">
</div>
</figure>
---

#### Using D-Claw to reveal landslide mobility bifurcations based on material parameters

The evolution of material strength in a landslide that liquefies is contingent on the evolving dynamics of the landslide as a whole. Therefore, realistic models of liquefying landslides cannot be founded on traditional rheological formulas, which specify that local resistance to motion is a function of only local stress states and displacements or displacement rates (Iverson, 2003). Instead, realistic models must allow the apparent rheology to evolve in response to feedbacks that develop as the distributions of landslide mass, momentum and pore pressure evolve. These large-scale feedbacks can cause time- and space-dependent changes in the local material state, similar to changes that play a central role in quasi-static, critical-state soil mechanics. In contrast to evolving material states in quasi-static soils, however, evolving material states in liquefying landslides may be influenced by arbitrarily large, rapid displacements and momentum transfer. 

---
<figure>
<figcaption>Figure 4. Lidar-based imagery before and after the 2014 landslide is used to compare the smaller 2006 Hazel slide from the source region which did not exhibit the high mobility of the 2014 slide, but rather slumped and remained north of the Stilliguamish River.</figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/oso/OsoHazelOblique.png">
</div>
</figure>
---

Models that aim to explain the behaviour of landslides that liquefy must also be able to explain landslide behaviour in which liquefaction does not occur – without invoking differences in intrinsic granular friction. Models that lack this discriminatory power can shed no light on factors favouring or limiting the potential for liquefaction and attendant high mobility. Indeed, the difference between relatively slow, stable landslide motion and unstable, liquefying landslide motion may represent a sharp behavioural bifurcation (Iverson et al., 2000; Iverson, 2005). Important questions about such a bifurcation concern its sensitivity to initial conditions and material properties.

---
<figure>
<figcaption>Figure 5. D-Claw model results showing different mobilities based on the relative values of the critical (0.64) and initial (m0) porosities. Decreasing inital porosities lead to enhanced mobility due to dilatancy effects and liquefaction.</figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/oso/DClawMobilities_6panel.png ">
</div>
</figure>
---

Here the focus is placed on insights that can be gained from using D-Claw to model the dynamics of the landslide as well as a spectrum of alternative behaviours computed for landslides with the same initial geometry and basal friction angle, but with modified values of the initial solid volume fraction *m0* and permeability *k0*.

---
<figure>
<figcaption> Figure 6. Time series results with alternative parameters for the initial solid volume fraction and initial hydraulic permeability, showing the evolution of mobility. Left: Three simulations with constant values of initial hydraulic permeability (k0=e-8) and three different intial porosities strongly affects the degree of liquefaction and ultimate mobility. Right: Three simulations with constant initial porosity (m0 = 0.62) and three different hydraulic permeabilities affects the time-scale of pore-pressure diffusion and mobility evolution.</figcaption>
<div class="gallery" data-columns="2">
    <img src="/images/projects/oso/TKEComparePorosity.png">
    <img src="/images/projects/oso/TKEComparePerm.png">
</div>
</figure>
---
---
<figure>
<figcaption> Figure 7. Plots of 27 different D-Claw simulations with alternative values for the initial solid volume fraction m0 and initial hydraulic permeability k0, showing the bifurcation of mobility when m0<m_crit. Panels show alternative measures of ultimate mobility </figcaption>
<div class="gallery" data-columns="3">
    <img src="/images/projects/oso/MaxTKE.png ">
    <img src="/images/projects/oso/HoverL.png">
    <img src="/images/projects/oso/CoverageArea.png ">
</div>
</figure>
---

---
#### Conclusions

An important practical implication of these findings is that large differences in landside mobility can result from small differences in initial conditions. Model studies aimed at landslide hazard prognostication can in principle account for the associated uncertainties by adopting probabilistic methods. Nevertheless, the challenge in making useful predictions is great, because bifurcating landslide dynamics can result in divergent outcomes.

---
#### References

* **Landslides that liquefy: modeling mobility bifurcation and the 2014 Oso, Washington, USA disaster.** R.M. Iverson, D.L. George, 2016. *Geotechnique*, V. 66(3), 175--187. [pdf]({{ site.baseurl }}/pubs/IversonGeorge2016_Geotechnique_Oso.pdf)
* **Landslide mobility and hazards: implications of the 2014 Oso disaster.** R.M. Iverson, D.L. George, et al., 2015. *Earth Planet. Sci. Lett.*, V. 412, pp. 197--208. [pdf]({{ site.baseurl }}/pubs/IversonGeorgeEtAl2015_EPSL_Oso.pdf)
* **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests.** D. L. George and R.M. Iverson, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/GeorgeIverson2014_ProcRSocA.pdf)
*  **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis.** R.M. Iverson and D.L. George, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf)



