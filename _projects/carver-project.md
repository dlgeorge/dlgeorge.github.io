---
title: 'Cascading flow hazards'
subtitle: 'modeling landslides, waves, breach erosion, and flows with D-Claw'
date: 2018-01-01 00:00:00
description: Hypothetical case study - South Sister Volcano and moraine-dammed Carver Lake, Oregon.
featured_image: '/images/projects/carver/Summit2Lake_frame00035.png'
---

### Hazard assessment near South Sister Volcano, Oregon, based on hypothetical models of Carver Lake outburst floods.


This page features excerpts and material from:

**Seamless numerical simulation of a hazard cascade in which a landslide triggers a dam-breach flood and consequent debris flow,** D.L. George, R.M. Iverson, and C.M. Cannon, 2020. *Debris-Flow Hazards Mitigation: Mechanics, Monitoring, Modeling, and Assessment, Association of Environmental and Engineering Geologists, Special Publication 28.* [pdf]({{ site.baseurl }}/pubs/GeorgeIversonCannon_7thDFHM.pdf)

<figure>
<div class="gallery" data-columns="2">
    <img src="{{ site.baseurl }}/images/projects/carver/slideview_sv_mc622_k-9_opt_rcolors_0.5res.gif">
    <img src="{{ site.baseurl }}/images/projects/carver/damview_sv_mc622_k-9_opt_0.5res_rcolors.gif">
</div>
<figcaption> D-Claw animations described further below.</figcaption>
</figure>

---
### Abstract
<small>
Numerical simulations of hazard cascades downstream from moraine-dammed lakes commonly must specify linkages between models of discrete processes such as wave overtopping, dam breaching, erosion, and downstream floods or debris flows.  Such linkages can be rather arbitrary and can detract from the ability to accurately conserve mass and momentum during complex sequences of events.  Here we describe an alternative methodology in which we use high-resolution lidar topography and 2-D, two-phase conservation laws to seamlessly simulate all stages of a hazard-cascade that culminates in a debris flow. Our simulations employ our depth-integrated numerical model D-Claw to evaluate hazards from prospective breaching of a moraine dam that impounds Carver Lake on the eastern flank of South Sister volcano in central Oregon, USA.  We simulate a “worst-case scenario” sequence of events that begins with a hypothetical 1.6 million cubic meter landslide that originates near the summit of South Sister and enters Carver Lake. Wave generation and displacement of lake water then leads to dam overtopping, breach erosion, and a downstream debris flow that funnels into Whychus Creek and eventually reaches the community of Sisters, Oregon, about 20 km away.  Notably, our simulations predict that much of the debris is directed away from Sisters as a result of natural avulsion and flow diversion that occurs near the head of a low-gradient alluvial fan upstream from Sisters.  Consequently, predicted hazards to downtown Sisters are less severe than those predicted by 1-D shallow-water simulations of a Carver Lake dam breach that were performed in the 1980s.</small>

---
### Introduction

In a recent study, we used D-Claw to model a hypothetical outburst flood from a moraine-dammed lake on the east side of South Sister volcano near the town of Sisters, Oregon, USA. The hypothetical landslide begins near the summit of South Sister and enters Carver Lake, where it generates large waves that overtop the moraine dam. Because D-Claw can model the erosion and entrainment of basal sediment, the subsequent dam breaching process occurs spontaneously, leading to lake drainage and downslope floods and debris flows. Owing to spreading and avulsion of the modeled flow in a system of distributary channels on the alluvial fan upstream from Sisters, the predicted hazard to the community is less severe than was predicted by 1-D shallow-water computations performed in the 1980s (Laenen et al., 1987), as the 1-D modeling does not make possible the direct modeling of stream bifurcation, but rather requires the primary flood channel to be chosen a priori.

---
### Background: hazards downstream from Carver Lake, Oregon

Carver Lake is a moraine-dammed lake on the eastern flank of South Sister volcano in central Oregon, USA. The lake sits approximately 20 km upstream from the community of Sisters, Oregon, located in the valley below. The outlet channel of Carver Lake is a small tributary of Whychus Creek, which flows through downtown Sisters. 

In the 1980s, concern was raised regarding the flooding risk posed to the Sisters community, should a moraine-dam failure lead to an outburst flood from Carver Lake. Modeling conducted at the time utilized 1D shallow-water equations and suggested that, in the event of complete lake drainage, the flooding hazard could be substantial (Laenen et al., 1987). Because of recent advances in flood and debris-flow modeling capabilities, there has been interest by community members to reassess this hazard with more sophisticated methods.  

---
<figure>
<figcaption> Figure 1. The summit of South Sister Volcano and the moraine-dammed Carver Lake. Left: oblique arial photograph showing the summit of the volcano and Carver Lake. Right: overhead map showing the summit and Carver Lake to the upper right.</figcaption>
<div class="gallery" data-columns="2">
    <img src="{{ site.baseurl }}/images/projects/carver/CarverProutyPhoto.png">
    <img src="{{ site.baseurl }}/images/projects/carver/CarverLake.png">
</div>
</figure>

<figure>
<figcaption> Figure 2. Maps showing the relative location of Carver Lake (near southwest corner) and Sisters, Oregon. Left: map showing the extent of the D-Claw simulation domain. Boxes enclose the regions depicted in panels on the right. Top Right: map showing the area around Carver Lake. Bottom Right: map showing the area around Sisters, Oregon. </figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/carver/map_merged.png">
</div>
</figure>
---
There is consensus among geologists and engineers who have visited Carver Lake (e.g., Laenen et al.,1987; O’Connor et al., 2001) that the moraine dam appears stable to spontaneous failure, and that a failure would most likely require overtopping waves generated by a landslide entering the lake. We therefore used D-Claw to simulate scenarios in which a landslide originates on the slopes of South Sister above Carver Lake. All subsequent processes (e.g., wave generation, dam overtopping, erosion, downstream flooding and debris flows) were simulated seamlessly. That is, dam failure and flooding were not specified by the model set-up. Assumptions only about the landslide size and
location and the erodibility of the dam material were explicitly prescribed. 

---
### D-Claw modeling of landslide, wave-generation, dam erosion and downstream floods

Simulations were performed on a large domain (approximately 50 km by 50 km), which included the summit of South Sister in the southwest corner and extended northward beyond the community of Sisters. A hypothetical landslide source geometry encompassing 1.6 million cubic meters of material was constructed near the summit of South Sister volcano and extending downslope toward Carver Lake. Computations were initialized in D-Claw with a solid volume fraction, 0.62, within the landslide source area, except for within Carver Lake. A region beginning near the upstream face of the moraine dam and extending downstream from the lake outlet was initialized with potentially erodible material occupying depths approximately 20 meters below the current DEM topography, and extending for approximately 300 meters downstream along the drainage channel. The erodible material was assumed to be a saturated granular-fluid mixture with the same material properties as the surrounding material.

---
<figure>
<figcaption> Figure 3. West-looking oblique perspective of the failure and evolution of the simulated landslide mass which inundates Carver Lake and generates waves that overtop the moraine dam. The wave action at the dam begins to erode channel material. Shading indicates the solid volume fraction, m, which varies from 0 (pure water) to ~ 0.6 (dense granular-fluid mixture). </figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/carver/LandslideMerged.png">
</div>
</figure>
---

<figure>
<figcaption> Figure 4. North-looking oblique perspective of wave generation, overtopping and erosion of the moraine dam that leads to a downstream debris flow. Modeling set-up and animation provided below.</figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/carver/DamMerged.png">
</div>
</figure>


---
### Downstream results 

Several kilometers upstream of the community of Sisters, Whychus Creek debouches onto an alluvial fan with low relief and a system of (now dry) distributary channels. When the modeled flow reached this point after approximately 1 hour, it immediately overtopped the low banks of the main branch of Whychus Creek, spreading into the distributory channels. The flow continued to spread widely across the alluvial fan, eventually inundating Sisters. However, due to the spreading, the depth of the flow in the main channel was reduced significantly, presumably lessening the flood risk posed to the more densely populated area of Sisters adjacent to the main channel. The results contrasted with early 1-D simulations performed in the 1980's, which assumed that most of the flow was confined to the channel.

---
<figure>
<figcaption>Figure 6. Overhead view of the simulation domain. Left: the simulation at t=0. South Sister Volcano and Carver Lake are in the lower left. Right: the AMR grids that resolve flood waves from Carver Lake to Sisters, Oregon. </figcaption>
<div class="gallery" data-columns="2">
    <img src="{{ site.baseurl }}/images/projects/carver/frame00000.png">
    <img src="{{ site.baseurl }}/images/projects/carver/frame00280.png">
</div>
</figure>

<figure>
<figcaption>Figure 7. Downstream results on the alluvial fan surrounding Sisters, Oregon. Left: D-Claw animation. Right: Inundation map -- shading indicates the maximum depth observed at any location for the duration of the simulation. </figcaption>
<div class="gallery" data-columns="2">
    <img src="{{ site.baseurl }}/images/projects/carver/sisters_fan_amr_blue_opt1.gif">
    <img src="{{ site.baseurl }}/images/projects/carver/SistersFan_inundation.png">
</div>
</figure>

---
### Conclusions

Dam-break outburst floods and other phenomena that involve grain-fluid mixtures (e.g., landslides, debris flows, dam breaches and bed-material entrainment) interacting with bodies of water, pose modeling challenges due to the multi-physics nature of the cascading hazards. Coupling disparate models together is less than desirable, due to implementation difficulties and model inaccuracy from ad hoc, non-conservative, coupling assumptions.

Our modeling approach requires only initial conditions and material parameters for the landslide material, water, and erodible bed material with no explicitly specified coupling assumptions. Obtaining high-resolution results with such simulations also requires use of high-resolution digital topographic data, such as the lidar data we utilized in this study. Compared to earlier studies employing 1-D equations and coarse topography, our modeling suggests a strikingly different result for our test case involving inundation near Sisters, Oregon. Owing in part to the use of 2-D equations as well as high-resolution lidar topography, our results suggest that flow avulsion and diversion on the alluvial fan surrounding Sisters would lead to a less severe flood hazard to the community.

---
### References

* Berger, M.J., George, D.L.,  LeVeque, R.J. and K.T. Mandli, 2011. **The GeoClaw software for depth-averaged flows with adaptive refinement.**   *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016 [pdf]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)
* George, D.L. 2010.**Adaptive finite volume methods with well-balanced Riemann solvers for modeling floods in rugged terrain: application to the Malpasset dam-break flood (France, 1959).**  *Int. J. Numer. Methods Fluids*, 66(8): 1000--1018. [pdf]({{ site.baseurl }}/pubs/George2010_IJNMF.pdf)
* George, D.L., Iverson, R.M. and Cannon, C.M., 2017.**New methodology for computing tsunami generation by subaerial landslides: application to the 2015 Tyndall Glacier Landslide, Alaska.**  *Geophys. Res. Lett.*, V. 44(14), 7276--7284. [pdf]({{ site.baseurl }}/pubs/GeorgeIversonEtAl2017_GRL_Tyndall.pdf)
* Laenen, A., Scott, K.M. Costa, J.E. and Orzol, L.L., 1987, **Hydrologic hazards along Squaw Creek from a hypothetical failure of the glacial moraine impounding Carver Lake near Sisters, Oregon,** *Open-file report 87-41,* U.S. Geological Survey.
* O’Connor, J.E., Hardison, J.H., and Costa, J.E., 2001, **Debris flows from failures of Neoglacial-age dams in the Three Sisters and Mount Jefferson wilderness areas, Oregon,** *Professional Paper 1606,* U.S. Geological Survey.



