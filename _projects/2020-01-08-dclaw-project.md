---
title: 'D-Claw'
subtitle: 'software for simulating granular-fluid flows'
date: 2020-01-08 00:00:00
description: D-Claw is an open-source numerical software package for simulating granular-fluid flows, such as landslides, debris flows, and lahars.
featured_image: '/images/pages/MSH2_crop2.jpg'
---

![](/images/projects/dclaw/misc/Rainier_frame00015.png)

## Overview

D-Claw is an open-source numerical software package for modeling granular-fluid flows (landslides, debris flows, etc.). D-Claw is built on top of [Clawpack](www.clawpack.org) and [GeoClaw](www.geoclaw.org) software. D-Claw implements a two-phase granular mathematical model developed by Richard Iverson and David George at the U.S. Geological Survey. 

### software features

D-Claw employs modified versions of many software features first implemented in GeoClaw (*e.g.,* [George, 2006; ]({{ site.baseurl }}/pubs/George2006_Phd.pdf) [Berger, George, et al., 2011]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)). These include shock-capturing wave-propagation algorithms (LeVeque, 2002) and patch-based adaptive mesh refinement algorithms (AMR) (Berger, 1989) extended to free-surface flows over topography ([George, 2006; ]({{ site.baseurl }}/pubs/George2006_Phd.pdf)[LeVeque, George, et al., 2011]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)). These AMR techniques enable the dynamic resolution of flows that traverse geometrically complex drainage routes within large bounding domains. AMR also facilitates the computationally tractable use of high-resolution lidar elevation data in subdomains of interest, without complex topographic data synthesis or computational mesh generation. Robust well-balanced Riemann solvers, originally developed for the shallow water equations [(George, 2008)]({{ site.baseurl }}/pubs/George2008_JCP.pdf), have been extended to D-Claw's model equations. These algorithms provide accurate capturing of discontinuites, inundation fronts over irregular topography, and steady-state resolution (pools, static masses, river-like flow). 

### mathematical model

The two-phase granular-fluid model implemented in D-Claw is based on mathematical models originally developed by Richard Iverson and later co-developed with David George, at the USGS. The model, described in detail by [Iverson & George, 2014]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf) and [George & Iverson, 2014]({{ site.baseurl }}/pubs/GeorgeIverson2014_ProcRSocA.pdf), combines principles of fluid, solid, and soil mechanics. A unique feature of the model is the coupled evolution of the solid-grain concentration and the basal pore-fluid pressure, based on the principles of granular dilatancy. This co-evolution mediates the coulomb effective stress and hence the mobility of the flow, and hence allows the simulation of slope failure, incipient motion, and deposition without unrealistic force balances. The governing PDEs form a strictly hyperbolic system with non-conservative products, sharing fundamental mathematical stability properties with the more basic shallow water equations. The development of this model was informed by controlled experiments conducted at the USGS debris-flow flume over the last ~ 25 years (*see eg.,* experimental [video archives](https://pubs.usgs.gov/of/2007/1315/)). The aim of those experiments was to investigate the complex physics of debris flow motion, including initiation processes. Experimental work at the flume is ongoing. For more details see publications below.

### model development and extensions

Ongoing D-Claw development is aimed at extending its capabilities to more general surface flow processes through the incorporation and refinement of physical and mathematical submodels. Recent examples include the extension of our two-phase model to the full spectrum of surface flows with evolving sediment loads (from pure water to solid-granular flows), enabling the modeling of the interaction of water bodies and granular mixtures (*e.g.,* landslide-generated tsunamis, landslide and debris flow interactions with lakes and rivers). The incorporation of entrainment of erodible sediment has further extended D-Claw's capabilities to include flood and debris-flow bulking, earthen-dam erosion, lake outburst flood modeling, and debris-entraining tsunami inundation. Extension of D-Claw to post-wildfire debris flows, in which overland flow entrains sediment, is an active and collaborative current research project. Additional previous extensions include particle-size segregation and levee formation (an important process for debris-flow dynamics). Rainfall infiltration and pore-pressure diffusion modeling are also actively under development. See [projects](/projects) for specific applications.   

### source code

D-Claw is built on top of Clawpack v4.x code. It is a generalization, or extension, of the v4.x GeoClaw code, incorporating GeoClaw's numerical algorithms for general free-surface flows over topography. However, D-Claw solves a two-phase (granular-fluid) shallow-flow model (see more below).

The current version of D-Claw v4.x is available at github: [github.com/geoflows/D-Claw](https://github.com/geoflows/D-Claw). Merging D-Claw with the current Clawpack v5.x code is planned in the future. 

See [software](/software/) for more information.


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

Selected D-Claw animations (to appear). See also individual project pages.

---

### related publications

*  **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis.** R. M. Iverson and D. L. George, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf)
* **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests.** D. L. George and R. M. Iverson, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/GeorgeIverson2014_ProcRSocA.pdf) 
* **Landslides that liquefy: modeling mobility bifurcation and the 2014 Oso, Washington, USA disaster.** R. M. Iverson, D. L. George, 2016. *Geotechnique*, V. 66(3), 175--187. [pdf]({{ site.baseurl }}/pubs/IversonGeorge2016_Geotechnique_Oso.pdf)
* **Landslide mobility and hazards: implications of the 2014 Oso disaster.** R. M. Iverson, D. L. George, et al., 2015. *Earth Planet. Sci. Lett.*, V. 412, pp. 197--208. [pdf]({{ site.baseurl }}/pubs/IversonGeorgeEtAl2015_EPSL_Oso.pdf)
*  **New methodology for computing tsunami generation by subaerial landslides: application to the 2015 Tyndall Glacier Landslide, Alaska.** D. L. George, R. M. Iverson, C. M. Cannon, 2017. *Geophys. Res. Lett.*, V. 44(14), 7276--7284.  [pdf]({{ site.baseurl }}/pubs/GeorgeIversonEtAl2017_GRL_Tyndall.pdf)
* **Tsunami modeling with adaptively refined finite volume methods.** R.J. LeVeque, D.L. George and M.J. Berger, 2011. *Acta Numerica* 20, pp. 211--289. Arieh Iserles, ed. [pdf]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)
* **The GeoClaw software for depth-averaged flows with adaptive refinement.**  M. J. Berger, D. L. George, R. J. LeVeque and K. T. Mandli, 2011. *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016. [pdf]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)
* **Finite volume methods for hyperbolic problems.** R.J. LeVeque, 2002. Texts in Applied Mathematics, Cambridge University Press.
* **Local adaptive mesh refinement for shock hydrodynamics.** M.J. Berger and P. Colella, 1989. *J. Comput. Phys.,* 82: 64-84. 
* **Augmented Riemann solvers for the shallow water equations over variable topography with steady states and inundation.** D. L. George, 2008. *J. Comput. Phys.*, 227(6): 3089--3113. [pdf]({{ site.baseurl }}/pubs/George2008_JCP.pdf)
* **Finite volume methods and adaptive refinement for tsunami propagation and inundation,** D.L. George, 2006. *Ph.D. thesis*, University of Washington, Seattle. [pdf]({{ site.baseurl }}/pubs/George2006_Phd.pdf)