---
title: 'D-Claw'
subtitle: 'software for simulating granular-fluid flows'
date: 2020-01-08 00:00:00
description: D-Claw is an open-source numerical software package for simulating granular-fluid flows, such as landslides, debris flows, and lahars.
featured_image: '/images/pages/MSH2_crop2.jpg'
---

![](/images/projects/dclaw/misc/Rainier_frame00015.png)

## Overview

D-Claw is an open-source numerical software package developed at the USGS for modeling granular-fluid flows (landslides, debris flows, etc.). D-Claw is built on top of [Clawpack](www.clawpack.org) and [GeoClaw](www.geoclaw.org) software. 

### code

D-Claw is built on top of Clawpack v4.x code. It is a generalization, or extension, of the v4.x GeoClaw code, incorporating GeoClaw's numerical algorithms for general free-surface flows over topography. However, D-Claw solves an extended two-phase (solid-fluid) shallow-flow model (see more below).

The current version of D-Claw v4.x is available at github: [www.github.com/dlgeorge/D-Claw](www.github.com/dlgeorge/D-Claw). Merging D-Claw's features into the current Clawpack v5.x code is planned in the future. 

### mathematical model

The two-phase granular-fluid model implemented in D-Claw is based on mathematical models developed by [Richard Iverson]() and Dave George at the USGS. This model combines principles from fluid, solid, and soil mechanics. A unique feature of the model is the coupled evolution of the solid-grain concentration and the basal pore-fluid pressure, based on the principles of granular dilatancy. This co-evolution mediates the coulomb effective stress and hence the mobility of the flow. The resulting non-linear system of PDEs is a strictly hyperbolic system, similar to the more basic shallow water equations. The development of this model was informed by controlled experiments conducted at the USGS debris-flow flume over the last ~ 25 years. The aim of those experiments was to investigate the complex physics of debris flows, including their initiation and mobility. For more details see publications below.


---

### Images

Snapshots of D-Claw simulations:

<div class="gallery" data-columns="3">
	<img src="/images/projects/dclaw/misc/Rainier_frame00015.png">
	<img src="/images/projects/dclaw/misc/Rainierframe00080.png">
	<img src="/images/projects/dclaw/misc/Alderframe00083.png">
	<img src="/images/projects/dclaw/misc/tyndall_oblique_frame00015.png">
	<img src="/images/projects/dclaw/misc/Sisters_frame00035.png">
	<img src="/images/projects/dclaw/misc/dclaw_oso.jpg">
</div>


---

### Slideshow

More images of D-Claw simulations:

<div class="gallery" data-columns="1">
	<img src="/images/projects/dclaw/misc/Rainier_frame00015.png">
	<img src="/images/projects/dclaw/misc/Rainierframe00080.png">
	<img src="/images/projects/dclaw/misc/tyndall_oblique_frame00015.png">
	<img src="/images/projects/dclaw/misc/Sisters_frame00035.png">
	<img src="/images/projects/dclaw/misc/Alderframe00083.png">
	<img src="/images/projects/dclaw/misc/dclaw_oso.jpg">
</div>

### Animations

Selected D-Claw animations (to appear):

---

### related publications

*  A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis. R. M. Iverson and D. L. George, 2014. *Proc. R. Soc. A*, 470 (2170).
* A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests. D. L. George and R. M. Iverson, 2014. *Proc. R. Soc. A*, 470 (2170). 
* Landslides that liquefy: modeling mobility bifurcation and the 2014 Oso, Washington, USA disaster. R. M. Iverson, D. L. George, 2016. *Geotechnique*, V. 66(3), pp. 175--187.
* Landslide mobility and hazards: implications of the 2014 Oso disaster. R. M. Iverson, D. L. George, et al., 2015. *Earth Planet. Sci. Lett.*, V. 412, pp. 197--208.
*  New methodology for computing tsunami generation by subaerial landslides: application to the 2015 Tyndall Glacier Landslide, Alaska. D. L. George, R. M. Iverson, C. M. Cannon, 2017. *Geophys. Res. Lett.*, V. 44(14), 7276--7284.
* The GeoClaw software for depth-averaged flows with adaptive refinement.  M. J. Berger, D. L. George, R. J. LeVeque and K. T. Mandli, 2011. *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016.
* Augmented Riemann solvers for the shallow water equations over variable topography with steady states and inundation. D. L. George, 2008. *J. Comput. Phys.*, 227(6): 3089--3113.