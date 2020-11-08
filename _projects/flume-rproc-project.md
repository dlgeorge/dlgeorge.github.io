---
title: 'Granular-fluid models for landslide initiation and runout'
subtitle: 'model development and validation informed by experiments'
date: 2014-01-01 00:00:00
description: D-Claw granular-fluid model equations that incorporate dilatancy are informed by large-scale landslide initiation and runout experiments at the USGS debris-flow flume. 
featured_image: '/images/projects/flume/NR_oblique_compare2panel.png'
---

### Development of two-phase hyperbolic models that incorporate granular-dilatancy and pore-pressure feedbacks, informed by experiments at the USGS debris-flow flume. The model basis of the D-Claw software.


This page features material and excerpts from the companion papers:

* **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis.** R.M. Iverson and D.L. George, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf)

* **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests.** D. L. George and R.M. Iverson, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/GeorgeIverson2014_ProcRSocA.pdf)


![](/images/projects/flume/GR_oblique_doors_compare2panel.png)

---
### Abstract
<small>
To simulate debris-flow behaviour from initiation to deposition, we derive a depth-averaged, two-phase model that combines concepts of critical-state soil mechanics, grain-flow mechanics and fluid mechanics. The model’s balance equations describe coupled evolution of the solid volume fraction, *m*, basal pore-fluid pressure, flow thickness and two components of flow velocity. Basal friction is evaluated using a generalized Coulomb rule, and fluid motion is evaluated in a frame of reference that translates with the velocity of the granular phase. Source terms in each of the depth-averaged balance equations account for the influence of the granular dilation rate, defined as the depth integral of solid-phase divergence. Calculation of the dilation rate involves the effects of an elastic compressibility and an inelastic dilatancy
angle proportional to *m − meq*, where *meq* is the value of *m* in equilibrium with the ambient stress state and flow rate. Normalization of the model equations shows that predicted debris-flow behaviour depends principally on the initial value of *m − meq* and on the ratio of two fundamental timescales. One of these timescales governs downslope debris-flow motion, and the other governs pore-pressure relaxation that modifies Coulomb friction and regulates evolution of *m*. 
</small>

---
### Introduction

Depth-averaged models are commonly used for shallow-flow hydrodynamic modeling and have been extended to multi-component granular flows such as landslides. However, standard single-phase models that employ adapted rheological rules for a single-phase fluid are innadequate for the complex dynamics of landslides and debris flows. Spatial and temporal changes in macroscopic material behaviour that result from local rearrangements of grains and attendant evolution of pore-fluid pressure pose fundamental challenges for continuum mechanical modelling of debris flows. The most conspicuous transitions occur as debris mobilizes from static material on slopes, liquefies and flows rapidly, and later regains rigidity during consolidation of deposits. Most debris-flow models neglect these transitions, and instead treat rheology or depth-averaged flow resistance as inherent properties of debris. With this approach, flow dynamics simulations typically employ basal flow resistance coefficients less than half as large as those necessary to statically balance forces at flow initiation sites. Unbalanced initial states are held in check by assuming that an imaginary dam restrains the debris until the modeller issues a command, but use of this type of initial condition compromises physical relevance.

By contrast, most natural debris flows commence when balanced forces are infinitesimally perturbed. Flow onset commonly results from rainfall or snowmelt that triggers failure of debrismantled slopes or mobilization of scree in steep rills and gullies. As masses of water-saturated grains begin to move, however, the governing force imbalance can evolve dramatically owing to pore-pressure feedbacks that modify the apparent rheology of the debris. Differences between this type of behaviour and behaviour that arises from a stipulated rheology and force imbalance have great practical as well as theoretical significance, because pore-pressure feedbacks can determine whether a rapid debris flow develops at all—as opposed to a creeping landslide that moves imperceptibly or intermittently downslope.

---
### Objectives

Our chief goal is seamless simulation of debris-flow motion from initiation to deposition without any redefinition of governing equations, re-evaluation of parameters or restructuring of numerical methods. We pursue these goals by formulating a depth-averaged model that
allows feedbacks to develop during coupled evolution of solid and fluid volume fractions, porefluid pressure and debris-flow velocity and thickness. The feedbacks involve dilatancy – the state-dependent propensity of granular materials to undergo changes in solid volume fraction as they shear. Well-known since the time of Reynolds, variable dilatancy underpins the critical-state theory of soil mechanics, and it plays a key role in determining of the continuum-scale rheology of dense granular flows. Previous depth-averaged debris-flow models have included effects of solid–fluid interactions, and a few have accounted for evolution of solid and fluid volume fractions. However, no previous model has explicitly considered dilatancy coupled to pore-pressure feedbacks that mediate transitions between static and dynamic states. 

Our model is a depth-averaged granular-fluid model in the form of a two-phase, strictly hyperbolic system for depth, momentum, volume fractions, and pore-fluid pressure.  Like all depth-averaged models, our model neglects some details of three-dimensional behaviour. It nevertheless provides predictions that can be rigorously tested because it computes flow depths, velocities and basal pore pressures with a resolution similar to that of the most-detailed debris-flow data collected to date. Use of the solid volume fraction as an additional prognostic variable expands the possibilities for future model applications.

---
### Model development and validation utilizing the USGS debris-flow flume

To test D-Claw, we present simulations of two types of large-scale experiments conducted at the USGS debris-flow flume (Figure 1). In the first type of test, we address short-timescale dynamics during onset of debris-flow motion triggered by gradually rising pore-fluid pressures in static slopes. In the second type, we address dynamics over the longer timescales that are relevant during subsequent downslope motion, runout and deposition. Traditionally, these two distinct problems have been treated with dissimilar models, one for onset of slope instability and one for the dynamics of ensuing motion. By contrast, D-Claw simulates both flow onset from an initially balanced equilibrium state and flow dynamics in states that are far from equilibrium.

---
<figure>
<figcaption> Figure 1. The USGS debris-flow flume near Blue River, Oregon, is the largest field-scale facility of its type. Highly controlled and closely monitored experiments inform physical and numerical model development and validation. </figcaption>
<img src="{{ site.baseurl }}/images/projects/flume/Flume3panelHistory.png">
</figure>
---

---
### Predictions of slope stability and flow mobilization: natural release experiments.

In this section, we investigate D-Claw’s ability to predict debris-flow mobilization from an initially stable sediment mass. In each of the mobilization experiments (described by Iverson et al. 2000), a 6 cubic meter rectangular prism of sediment was placed behind a retaining wall positioned normal to the bed. Rising pore-water pressures that triggered slope failure were generated by controlled watering.  Evolving pore-water pressures and slope deformation were monitored continuously by a network of piezometers, tensiometers, subsurface tiltmeters and surface extensometers.

---
<figure>
<figcaption> Figure 2. Natural release experiments at the debris-flow flume aimed at investigating the initiation process with detailed data collection of dynamically evolving dynamics, stress, and pore-fluid pressure. </figcaption>
<div class="gallery" data-columns="2">
    <img src="/images/projects/flume/NaturalRelease.jpg">
    <img src="/images/projects/flume/NR_dense_oblique.png">
    <img src="/images/projects/flume/NaturalReleaseCartoon.png">
    <img src="/images/projects/flume/NaturalReleasePlanviewDClaw.png">
</div>
</figure>
---

We consider repeated experiments in which only the initial sediment porosity is intentionally varied. In some experiments, the sediment was loosely placed resulting in initial solid volume fractions *m* < 0.5. In other cases, the sediment was densified through vibrational compaction of multiple layers resulting in initial solid volume fractions *m* > 0.6. Ancillary testing revealed that the critical-state solid volume fraction for this sediment at appropriately low confining stresses was about 0.56. We classify the initial states *m*< 0.56 as ‘loose’, while those in experiments with *m*>0.56 were classified as ‘dense’. 

During slope failure, loosely packed sediment quickly liquefied and transformed into rapid debris flows. This behaviour resulted from sediment contraction upon shearing, evidenced by a dramatic, contemporaneous increase in porefluid pressure. With densely packed sediment, on the other hand, slope failures exhibited self-stabilizing behaviour, because pore-fluid pressures decreased as the deforming sediment dilated. In such cases, landslides crept slowly and sometimes intermittently downslope. These contrasting styles of behaviour test not only D-Claw’s ability to seamlessly simulate the transition of a stable mass into a moving mass, but also the model’s ability to regulate evolution of pore-fluid pressure and thereby influence the degree and nature of landslide mobilization.

#### Case 1: loose-sediment experiment: dilatancy feedbacks lead to liquefaction and runaway acceleration.

We first consider model performance in simulating an experiment with loosely packed sediment. In these experiments and simulations, initial failure of the sediment results in profound weaking associated with liquefaction and runaway acceleration. (George & Iverson, 2014, provides a more detailed description of model results and piezometer and extensometer data.)

---
<figure>
<figcaption> Figure 3. D-Claw results for the loose-soil experiment. Left: cross-sectional perspective at selected times. Basal pore
pressure is indicated by the fractional depth of blue-shaded sediment, with lithostatic pressure indicated by full blue shading. The position of Lagrangian numerical sensors used to gauge model predictions are shown with markers that move with the sediment. Subsequent to failure the pore-fluid pressure quickly elevates upon contractive behavior leading to liquefaction and rapid acceleration Right: time-series comparison with results from numerical sensors and experimental data recorded by piezometer and extensometer data in the experiments described by Iverson et al., 2000. Top and bottom panels indicate different model material parameter choices within the constrained range. </figcaption>
<div class="gallery" data-columns="2">
    <img src="/images/projects/flume/figure06.png">
    <img src="/images/projects/flume/figure07.png">
</div>
</figure>

<figure>
<figcaption> Figure 4. Cross-sectional animation of a D-Claw simulation of the loose soil experiment. </figcaption>
<img src="{{ site.baseurl }}/images/projects/flume/NR_loose_planview_markers.gif">
</figure>
---


#### Case 2: dense-sediment experiment: dilatancy feedbacks lead to slow episodic motion.

Next we consider model performance in simulating an experiment with densely packed sediment. In these experiments and simulations, initial failure of the sediment leads to a dilative response of the denser soil, which reduced the pore-fluid pressure during deformation, acting to retard motion. The pore-fluid pressure slowly rebounded after each precipitous drop, leading to semi-periodic stick–slip cycles (Figure 5). 

---
<figure>
<figcaption> Figure 4. D-Claw results for the dense-soil experiment. Left: cross-sectional perspective at selected times. Basal pore
pressure is indicated by the fractional depth of blue-shaded sediment, with lithostatic pressure indicated by full blue shading. The material fails at t=0 (middle panel) but remains visually in place for the duration of the simulation at t=60 s (right panel).  Right: time-series results from Lagrangian numerical sensors for the simulated position and basal pore pressure of a material.  Dilative behavior causes a slow episodic creep and pressure reduction with each slip cycle.</figcaption>
<div class="gallery" data-columns="2">
    <img src="/images/projects/flume/NR_dense_planview.png">
    <img src="/images/projects/flume/NR_dense_displacement_pressure.png">
</div>
</figure>
---


---
#### Gate-release experiments: downslope dynamics and runout.

In this section, we investigate D-Claw’s ability to predict debris-flow dynamics, runout and deposition measured in a set of gate-release flume experiments.  In these experiments, loose sediment was placed in a hopper behind a vertical gate near the top of the flume, saturated with water, and released by suddenly opening the gate (Figures 5-7). Upon releasing the headgate, the saturated mixtures quickly liquefied and developed into debris flows that descended the flume channel before emerging onto a nearly planar runout pad and forming deposits.

---
<figure>
<figcaption> Figure 5. Schematic of gate-release experiments at the debris-flow flume.</figcaption>
<img src="{{ site.baseurl }}/images/projects/flume/GateReleaseCartoon.png">
</figure>
---

---
<figure>
<figcaption> Figure 6. Photographs of the headgate doors opening for a gate-release experiment.</figcaption>
<div class="gallery" data-columns="3">
    <img src="/images/projects/flume/GateDoors1.jpg">
    <img src="/images/projects/flume/GateDoors2.jpg">
    <img src="/images/projects/flume/GateDoors3.jpg">
</div>
</figure>
---

We focus on the mean behaviour measured in an aggregated set of eight experiments referred to as sand–gravel–mud (SGM) experiments due to the composition of the sediment, which contained about 6% mud-sized particles by dry weight (Iverson et al., 2010).

---
<figure>
<figcaption> Figure 7. D-Claw simulation of a gate-release experiment. Color shading indicates the degree of liquefaction, with blue indicating lithostatic pressure.</figcaption>
<img src="{{ site.baseurl }}/images/projects/flume/GR_oblique_doors.gif">
</figure>
---

Aggregated time-series data reported by Iverson et al., 2010,  provide a basis for straightforward comparison with our D-Claw simulation. In Figure 8, grey shading represents the mean±1 s.d. measured in eight experiments. Figure 13a compares the measured flow depth at *x* = 2 m with model results obtained with and without the simulated motion of the headgate. Note that the gate slightly impedes the flow, resulting in a delayed and more abrupt rise in thickness as most of the flow reaches *x* =2 m. Figure 13b shows the computed basal pore-fluid pressure *p*, compared to the lithostatic and hydrostatic pressure for the computed thickness *h*, illustrating the high degree of liquefaction at early times. Measurements of the basal pore-fluid pressure in the experiments were not obtained at *x* =2 m.

---
#### Conclusions



---
#### References

* George, D.L. and Iverson, R.M., 2014. **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests.**  *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl}}/pubs/GeorgeIverson2014_ProcRSocA.pdf)
* Iverson, R.M. and George, D.L., 2014. **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis.**  *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf)
* Iverson, R.M. and George, D.L., 2016. **Landslides that liquefy: modeling mobility bifurcation and the 2014 Oso, Washington, USA disaster.**  *Geotechnique*, V. 66(3), 175--187. [pdf]({{ site.baseurl }}/pubs/IversonGeorge2016_Geotechnique_Oso.pdf)
* Iverson, R.M., George, D.L., et al., 2014**Landslide mobility and hazards: implications of the 2014 Oso disaster.** R.M. Iverson, D.L. George, et al., 2015. *Earth Planet. Sci. Lett.*, V. 412, pp. 197--208. [pdf]({{ site.baseurl }}/pubs/IversonGeorgeEtAl2015_EPSL_Oso.pdf)
* Iverson RM, Logan M, LaHusen RG, Berti M. 2010, **The perfect debris flow? aggregated results
    from 28 large-scale experiments**. *J. Geophys. Res.* 115, 1–29. (doi:10.1029/2009JF001514)
* Iverson RM, Reid ME, Iverson NR, LaHusen RG, Logan M, Mann JE, Brien DL., 2000. **Acute sensitivity of landslide rates to initial soil porosity.**  *Science* 290, 513–516. (doi:10.1126/science.290.5491.513)
