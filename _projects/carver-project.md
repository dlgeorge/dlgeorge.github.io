---
title: 'Cascading flow hazards'
subtitle: 'modeling landslides, waves, breach erosion, and flows with D-Claw'
date: 2018-01-08 00:00:00
description: D-Claw is extended to simulate a landslide that induces wave-generated dam erosion and resulting outburst floods that entrain material leading to downslope debris flows. Hypothetical case study - South Sister Volcano and moraine-dammed Carver Lake, Oregon.
featured_image: '/images/projects/carver/Summit2Lake_frame00035.png'
---

### Carver Lake and South Sister Volcano, Oregon.


This page features material from:

**Seamless numerical simulation of a hazard cascade in which a landslide triggers a dam-breach flood and consequent debris flow,** D.L. George, R.M. Iverson, and C.M. Cannon, 2020. *Debris-Flow Hazards Mitigation: Mechanics, Monitoring, Modeling, and Assessment, Association of Environmental and Engineering Geologists, Special Publication 28.*

![](/images/projects/carver/Summit2Lake_frame00035.png)

---
#### Abstract
<small>
Numerical simulations of hazard cascades downstream from moraine-dammed lakes commonly must specify linkages between models of discrete processes such as wave overtopping, dam breaching, erosion, and downstream floods or debris flows.  Such linkages can be rather arbitrary and can detract from the ability to accurately conserve mass and momentum during complex sequences of events.  Here we describe an alternative methodology in which we use high-resolution lidar topography and 2-D, two-phase conservation laws to seamlessly simulate all stages of a hazard-cascade that culminates in a debris flow. Our simulations employ our depth-integrated numerical model D-Claw to evaluate hazards from prospective breaching of a moraine dam that impounds Carver Lake on the eastern flank of South Sister volcano in central Oregon, USA.  We simulate a “worst-case scenario” sequence of events that begins with a hypothetical 1.6 million cubic meter landslide that originates near the summit of South Sister and enters Carver Lake. Wave generation and displacement of lake water then leads to dam overtopping, breach erosion, and a downstream debris flow that funnels into Whychus Creek and eventually reaches the community of Sisters, Oregon, about 20 km away.  Notably, our simulations predict that much of the debris is directed away from Sisters as a result of natural avulsion and flow diversion that occurs near the head of a low-gradient alluvial fan upstream from Sisters.  Consequently, predicted hazards to downtown Sisters are less severe than those predicted by 1-D shallow-water simulations of a Carver Lake dam breach that were performed in the 1980s.</small>

---
#### Modeling preview

<figure>
<figcaption> West-looking oblique perspective of the failure and evolution of the simulated landslide mass which inundates Carver Lake and generates waves that overtop the moraine dam. The wave action at the dam begins to erode channel material. Shading indicates the solid volume fraction, m, which varies from 0 (pure water) to ~ 0.6 (dense granular-fluid mixture). Modeling set-up and animation provided below</figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/LandslideMerged.png">
</figure>

<figure>
<figcaption> North-looking oblique perspective of wave generation, overtopping and erosion of the moraine dam that leads to a downstream debris flow. Modeling set-up and animation provided below.</figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/DamMerged.png">
</figure>

---
#### Hazards Downstream from Carver Lake, Oregon

Carver Lake is a moraine-dammed lake on the eastern flank of South Sister volcano in central Oregon, USA. The lake sits approximately 20 km upstream from the community of Sisters, Oregon, located in the valley below. The outlet channel of Carver Lake is a small tributary of Whychus Creek, which flows through downtown Sisters. 

In the 1980s, concern was raised regarding the flooding risk posed to the Sisters community, should a moraine-dam failure lead to an outburst flood from Carver Lake. Modeling conducted at the time utilized 1D shallow-water equations and suggested that, in the event of complete lake drainage, the flooding hazard could be substantial (Laenen et al., 1987). Because of recent advances in flood and debris-flow modeling capabilities, there has been interest by community members to reassess this hazard with more sophisticated methods.  

<figure>
<figcaption> Overhead image of the summit of South Sister and Carver Lake.</figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/CarverLake.png">
</figure>

<figure>
<figcaption> Maps showing the relative location of Carver Lake (near southwest corner) and Sisters, Oregon.</figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/map_merged.png">
</figure>

---
#### D-Claw modeling set-up

D-Claw simulations were performed on a large domain (approximately 50 km by 50 km), which included the summit of South Sister in the southwest corner and extended northward beyond the community of Sisters. A hypothetical landslide source geometry encompassing 1.6 million cubic meters of material was constructed near the summit of South Sister volcano and extending downslope toward Carver Lake. Computations were initialized in D-Claw with a solid volume fraction, 0.62, within the landslide source area, except for within Carver Lake. A region beginning near the upstream face of the moraine dam and extending downstream from the lake outlet was initialized with potentially erodible material occupying depths approximately 20 meters below the current DEM topography, and extending for approximately 300 meters downstream along the drainage channel. The erodible material was assumed to be a saturated granular-fluid mixture with the same material properties as the surrounding material


---
#### Animations


<figure>
<figcaption> West-looking oblique perspective of the failure and evolution of the simulated landslide mass which inundates Carver Lake and generates waves that overtop the moraine dam. The wave action at the dam begins to erode channel material. Shading indicates the solid volume fraction, m, which varies from 0 (pure water) to ~ 0.6 (dense granular-fluid mixture).</figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/mv622k9sl.gif">
</figure>

<figure>
<figcaption>North-looking oblique perspective of wave generation, overtopping and erosion of the moraine dam that leads to a downstream debris flow. </figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/damview_sv_mc622_k-9.gif">
</figure>

---
#### Downstream results based on hypothetical modeling

<figure>
<figcaption>D-Claw results showing the flood and debris-flow inundation in the alluvial fan surrounding Sisters. Shading indicates the maximum depth observed at any location for the duration of the simulation. </figcaption>
<img src="{{ site.baseurl }}/images/projects/carver/SistersFan_inundation.png">
</figure>


---
#### Conclusions

Dam-break outburst floods and other phenomena that involve grain-fluid mixtures (e.g., landslides, debris flows, dam breaches and bed-material entrainment) interacting with bodies of water, pose modeling challenges due to the multi-physics nature of the cascading hazards. Coupling disparate models together is less than desirable, due to implementation difficulties and model inaccuracy from ad hoc, non-conservative, coupling assumptions.
We used D-Claw to seamlessly model a hypothetical landslide and the resulting cascade of lake inundation, wave generation, dam overtopping, breach growth and downstream debris flow. The modeling approach requires only  initial conditions and material parameters for the landslide material, water, and erodible bed material with no explicitly specified coupling assumptions. Obtaining high-resolution results with such simulations also requires use of high-resolution digital topographic data, such as the lidar data we utilized in this study.
Compared to earlier studies employing 1-D equations and coarse topography, our modeling suggests a strikingly different result for our test case involving inundation near Sisters, Oregon. Owing in part to the use of 2-D equations as well as high-resolution lidar topography, our results suggest that flow avulsion and diversion on the alluvial fan surrounding Sisters would lead to a less severe flood hazard to the community.

---
#### References

* Laenen, A., Scott, K.M. Costa, J.E. and Orzol, L.L. (1987), **Hydrologic hazards along Squaw Creek from a hypothetical failure of the glacial moraine impounding Carver Lake near Sisters, Oregon,** *Open-file report 87-41,* U.S. Geological Survey.
* O’Connor, J.E., Hardison, J.H., and Costa, J.E. (2001), **Debris flows from failures of Neoglacial-age dams in the Three Sisters and Mount Jefferson wilderness areas, Oregon,** *Professional Paper 1606,* U.S. Geological Survey.



