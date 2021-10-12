---
title: 'Assessment of a landslide tsunami threat in Alaska'
subtitle: 'modeling a hypothetical landslide, wave generation, and resulting tsunami with D-Claw'
date: 2021-08-01 00:00:00
description: Assessment of the wave generating potential of a large landslide failure in the Barry Arm of Harriman Fjord, Prince William Sound, Alaksa.
featured_image: '/images/projects/barryarm/OverheadPhoto_wtxt.png'
---


### Modeling a potential large landslide and resulting tsunami in Prince William Sound, Alaska

This page features excerpts and figures from:

**Preliminary assessment of the wave generating potential from landslides at Barry Arm, Prince William Sound, Alaska.**, K.R. Barnhart, R.P. Jones, D.L. George, J.A. Coe, and D.M. Staley, 2021. *USGS Open-File Report*, 1071. [pdf]({{ site.baseurl }}/pubs/BarnhartJonesEtAl2021.pdf)

<figure>
<figcaption>Barry Arm of Harriman Fjord, Prince William Sound. </figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/barryarm/OverheadPhoto_wtxt.png">
</div>
</figure>


---
### Abstract

<small>We simulated the concurrent rapid motion of landslides on an unstable slope at Barry Arm, Alaska. Movement of landslides into the adjacent fjord displaced fjord water and generated
a tsunami, which propagated out of Barry Arm. Rather than assuming an initial sea surface height, velocity, and location for the tsunami, we generated the tsunami directly using a model capable of simulating the dynamics of both water and landslide material. The fjord below most of the landslide source area was occupied by the Barry Glacier until about 2012; therefore, our direct simulation of tsunami generation by landslide motion required new topographic and bathymetric data, which was col- lected in 2020. The topographic data also constrained landslide geometries and volumes. We considered four scenarios based on two landslide volumes and two landslide mobilities—a more mobile, contractive landslide and a less mobile, noncontrac- tive landslide. The larger of the two volumes is 689 × 106 cubic meters (m3)—larger than the volume estimate in a previous study—and reflects the largest plausible volume given current observational data. The considered scenario that generated the largest wave heights resulted in forecast wave heights of over 200 meters (m) in the northern part of Barry Arm, adjacent to the landslide source area and runup on the opposite fjord wall in excess of 500 m. Simulated wave heights in excess of 5 m in southern Barry Arm and in Harriman Fjord occurred within 10–15 minutes (min) of landslide motion. The simulated tsunami reached Whittier, Alaska, approximately 20 min after initial rapid landslide motion, with peak heights of just over 2 m in Passage Fjord, 500 m offshore Whittier, occurring 26 min after initial rapid motion. Time of peak wave heights was consistent with previous modeling. Although results are preliminary and can be refined with additional observations and analyses, they provide a refined assessment of the upper bound of the hazard presented by the Barry Arm landslides. The results herein sup- port the National Oceanic and Atmospheric Administration’s National Tsunami Warning Center mission to detect, forecast, and warn for tsunamis in Alaska.
</small>

---
### Introduction

When situated upslope of waterbodies, landslides have the potential to generate a tsunami by rapidly moving into the waterbodies and displacing water. This poses a hazard to nearby populations, infrastructure, and marine traffic. There are multiple recent instances of tsunamigenic landslides in
steep maritime terrain in the Arctic and subarctic. These events are particularly problematic in areas that have experienced rapid glacial retreat, as (1) debuttressing of and (or) thermo- mechanical damage to steep valley sides may increase the susceptibility of valley walls to rapid landslide motion, and
(2) rapid glacial retreat may increase the likelihood of land- slide runout into open water rather than onto glacial ice that would have been present prior to glacial retreat. Examples of large tsunamigenic landslides in recently deglaciated terrain include July 9, 1958, Lituya Bay, Alaska (Miller, 1960a,
b; Ward and Day, 2010); April 27, 1975, Kitimat, British Columbia (Kirby and others, 2016); October 17, 2015, Taan Fjord, Alaska (George and others, 2017; Haeussler and others, 2018; Higman and others, 2018); and June 17, 2017, Karrat Fjord, Greenland (Bessette-Kirton and others, 2017; Poli, 2017; Gauthier and others, 2018).

In spring 2020, a citizen scientist identified a large, poten- tially tsunamigenic landslide in Barry Arm (figs. 1 and 2), a recently deglaciated fjord in Prince William Sound, Alaska (Johnson, 1916; Dai and others, 2020). Here, the northwest flank of the fjord side wall has destabilized into at least three large, slow-moving landslides (fig. 2; Dai and others, 2020; Schaefer and others, 2020; Coe and others, 2021). Evidence for motion at the largest landslide (named Landslide A) extends back to 1957, with more rapid movement between 2010 and 2017 coincident with the retreat of the Barry Glacier calving front (Dai and others, 2020). During 2020, remote interferometric synthetic aperture radar (InSAR) monitoring revealed seasonally isolated movement of Landslide A of about 17 centimeters (cm) between September 23 and October 17 (Schaefer and others, 2020). Based on strike slip and oblique slip faults located within Landslide A, Coe and others (2021) subdivided Landslide A into three kinematic elements (fig. 2; the Prow, Core, and Tail). The kinematic element boundaries reflect past deformational history and may change based on future deformation. The second landslide, Landslide B or the Wedge, is located up valley to the northeast of Landslide A. It was identified during InSAR analysis in summer 2020 and confirmed as an active landslide by InSAR deformation and structure mapping (Schaefer and others, 2020; Coe and others, 2021). The third landslide was identified based on differencing of June and October 2020 light detection and ranging (lidar) data by the Alaska Division of Geology & Geophysical Surveys (DGGS). This analysis revealed rapid movement of an area adjacent to Landslide A called the Kite (fig. 2) and a significant rockfall that mobilized as a rock ava- lanche from the headscarp of Landslide A (DGGS, 2021). The planimetric extent of Landslide A and the Kite are adjacent; however, the structural mapping (Coe and others, 2021) and lidar differencing (DGGS, 2021) indicate that these landslides moved independently in 2020. Although recent landslide kine- matics are relatively well constrained, little is known about the potential for future rapid motion, landslide volumes, and
timescale over which the hazard will persist.

For this preliminary report, we simulated the generation and propagation of a tsunami originating from the concur- rent rapid motion of Landslides A and B and the Kite into the adjacent fjord water. Our primary goal was to advance our understanding of potential tsunamigenic landslide hazards for the Barry Arm landslides using a coupled landslide runout and wave propagation model. Our results support the National Oceanic and Atmospheric Administration (NOAA) National Tsunami Warning Center’s mission to provide reliable detec- tion, forecasting, and warning of tsunamis to protect life and
property. Our methods advance upon existing work (for exam- ple, the tsunami modeling of Dai and others, 2020) through the direct treatment of landslide physics using the model D-Claw and incorporation of topographic and bathymetric data col- lected in 2020 (NOAA, 2020; Daanen and others, 2021).
D-Claw is a depth-averaged, two-phase model capable of simulating motion of variable granular fluid mixtures, ranging from landslides to clear water, and has been used to simulate subaerial landslide tsunami generation (George and others, 2017). Rather than assume an initial location, wave height,
and velocity for the tsunami, the use of D-Claw permits direct simulation of tsunami genesis from landslide motion into the fjord. Within, we consider only the case of all identified landslides rapidly moving together, two alternative landslide volumes constrained by observations of headscarp and toe angles, and two options for landslide mobility.

The larger of the two considered volumes represents the largest plausible volume, given current observational con- straints. Additional observations may refine our understanding and could increase or decrease the estimated volume. Before this work was conducted, whether a landslide with material that is more mobile would produce a larger tsunami than a landslide with material is less mobile was not clear; accord- ingly, we considered both cases. Similarly, considering only the scenario in which all landslides rapidly move together is intended to represent the likely worst-case scenario that pro- duces the largest waves. Whether other landslide geometries or rapid landslide motion sequences will produce a larger wave is uncertain. For example, the following are other plausible scenarios: a sequence in which movement of an identified landslide destabilizes an adjacent, previously stable area; complex landslide-water-glacier interactions below Landslide B; or far-field tsunami-tidewater glacier interactions.

The newly available topographic and bathymetric data allow us to directly simulate the landslide and subsequent wave generation, rather than assume the magnitude of an ini- tial wave. Our scenarios, topographic surface, and bathymetric surface are constrained by data collected after the preliminary modeling by Dai and others (2020), which simulated a series of hypothetical waves, generated not by landslide-water interaction, but as “hot start” initial wave conditions (more discussion of “hot start” initial conditions are discussed in “Model Description” section). We describe the approach of Dai and others (2020) and compare our results with theirs in the “Discussion” section.

Our results reflect a refinement on anticipated wave heights near the landslide, as well as in more distal locations in Prince William Sound, including at Passage Canal near the town of Whittier, Alaska.

<figure>
<figcaption>Figure 1.  A, Prince William Sound, Alaska, and B, the region between Whittier, Alaska, and the landslide source area. Both maps indicate place names discussed in the text, and panel A indicates the considered computational domain. (from Barnhart et al., 2021). </figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/barryarm/Figure1.png">
</div>
</figure>


---

---
### References

* Rozell, N. (2016), **The Giant Wave of Icy Bay**, *Geophys. Inst. AK Press Release*, Fairbanks, Alaska. Available at [www.gi.alaska.edu/alaska-science-forum/giant-wave-icy-bay](http://www.gi.alaska.edu/alaska-science-forum/giant-wave-icy-bay).
* Stark, C. P. (2015), **Landslide dynamics from seismology: New results,** Abstract EP51D-08 presented at 2015 Fall Meeting, *AGU*, San Francisco.
