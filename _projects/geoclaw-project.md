---
title: 'GeoClaw'
subtitle: 'software for simulating shallow-water flows'
date: 2008-01-01 00:00:00
description: GeoClaw is an open-source numerical software package for water-wave propagation and inundation (tsunamis, storm surges, overland flooding).
featured_image: '/images/projects/geoclaw/tsunamis/Pacific2011.png'
---

<figure>
<figcaption> GeoClaw simulation of the 2011 Tohoku Tsunami with local inundation modeling in Hilo, HI.</figcaption>
<div class="gallery" data-columns="1">
    <img src="{{ site.baseurl }}/images/projects/geoclaw/tsunamis/honshu2hilo.gif">
</div>
</figure>
---
### Overview

GeoClaw is an open-source package within the Clawpack project for simulating shallow earth-surface flows involving water-wave propagation and inundation (*e.g.*, tsunamis, storm surges and general overland flooding problems).

See [software](/software/) for more information about GeoClaw and the Clawpack project, or [projects](/projects/) for some example applications involving GeoClaw. More information can also be found at [geoclaw.org](http://www.geoclaw.org).

---
### Background

GeoClaw evolved from a collection of algorithms developed for modeling tsunamis as part of my thesis work (George, 2006). Implemented in the Clawpack adaptive numerical framework, these algorithms provide robust inundation capturing and well-balanced resolution in the presence of dominant steady states (e.g., ocean at rest). Additionally, AMR schemes that preserve well-balancing and inundation capturing in conjunction with mass, momentum and energy conservation enable global-scale tsunami propagation and local-scale inundation in reasonably efficient single simulations ( see also, George, 2008; LeVeque, George, et al., 2011). These methods are more generally applicable to shallow free-surface flows over topography, which motivated the extension of GeoClaw to overland flooding problems in irregular terrain (e.g, George, 2010; Berger, George, et al., 2011). Later extensions of these algorithms were developed for storm-surge applications (e.g., Mandli, 2014). GeoClaw is now used for a variety of applications involving shallow water flows over topography. Features and enhancements continue to be developed within the Clawpack project (e.g., Mandli, Ahmadia, et al., 2016). 

---
### GeoClaw example: modeling transoceanic tsunami propagation and inundation: the 2011 Tohoku Tsunami.

A GeoClaw simulation of the 2011 Tohoku Tsunami, with inundation modeling of Hilo, HI. A coarse level-1 grid is used for the steady-state ocean at rest, refined to level-2 grids for deep-ocean wave propagation. Level-3 grids resolve the compressed waves as they approach the coastal waters of the Hawaiin Islands, with meter-scale level-4 grids resolving the harbor and inundation of Hilo, HI (the actual inundation was limited to small onshore waves). For a detailed description of GeoClaw algorithms related to AMR and other algorithms for tsunamis modeling, see (George, 2006; Berger, George et al., 2011; & LeVeque, George, et al., 2011).

<figure>
<div class="gallery" data-columns="3">
	<img src="/images/projects/geoclaw/tsunamis/frame00000.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00001.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00010.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00030.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00040.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00045.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00050.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00058.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00062.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00064.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00066.png">
	<img src="/images/projects/geoclaw/tsunamis/frame00075.png">
</div>
</figure>

### References

see also [geoclaw.org](http://www.geoclaw.org) for links to publications involving GeoClaw.

* **Finite volume methods and adaptive refinement for tsunami propagation and inundation,** D.L. George, 2006. *Ph.D. thesis*, University of Washington, Seattle. [pdf]({{ site.baseurl }}/pubs/George2006_Phd.pdf)
* **Augmented Riemann solvers for the shallow water equations over variable topography with steady states and inundation.** D. L. George, 2008. *J. Comput. Phys.*, 227(6): 3089--3113. [pdf]({{ site.baseurl }}/pubs/George2008_JCP.pdf)
* **Tsunami modeling with adaptively refined finite volume methods.** R.J. LeVeque, D.L. George and M.J. Berger, 2011. *Acta Numerica* 20, pp. 211--289. Arieh Iserles, ed. [pdf]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)
* **The GeoClaw software for depth-averaged flows with adaptive refinement.**  M. J. Berger, D. L. George, R. J. LeVeque and K. T. Mandli, 2011. *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016. [pdf]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)
* **Adaptive finite volume methods with well-balanced Riemann solvers for modeling floods in rugged terrain: application to the Malpasset dam-break flood (France, 1959).** D.L. George, 2010. *Int. J. Numer. Methods Fluids*, 66(8): 1000--1018. [pdf]({{ site.baseurl }}/pubs/George2010_IJNMF.pdf)
* **Finite volume methods for hyperbolic problems.** R.J. LeVeque, 2002. Texts in Applied Mathematics, Cambridge University Press.
* **Local adaptive mesh refinement for shock hydrodynamics.** M.J. Berger and P. Colella, 1989. *J. Comput. Phys.,* 82: 64-84.
* **Adaptive mesh refinement for storm surge.** K.T. Mandli and C.N. Dawson, 2014. *Ocean Modeling,* V. 75, 36-50.

