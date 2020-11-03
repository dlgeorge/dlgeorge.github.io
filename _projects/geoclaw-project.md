---
title: 'GeoClaw'
subtitle: 'software for simulating shallow-water flows'
date: 2011-01-01 00:00:00
description: GeoClaw is an open-source numerical software package for water-wave propagation and inundation (tsunamis, storm surges, overland flooding).
featured_image: '/images/projects/geoclaw/tsunamis/Pacific2011.png'
---

![](/images/projects/geoclaw/tsunamis/Pacific2011_HI.png)

### overview

GeoClaw is open-source software for simulating shallow earth-surface flows involving water-wave propagation and inundation (*e.g.*, tsunamis, storm surges and general overland flooding problems). See [software](/software/) for an overview, background information, links to research, or information related to source-code development. 

### application examples and galleries

a few examples of GeoClaw applications are below. See also [clawpack.org](http://www.clawpack.org).

---
#### modeling transoceanic tsunami propagation and inundation: the 2011 Tohoku Tsunami.

A GeoClaw simulation of the 2011 Tohoku Tsunami, with inundation modeling of Hilo, HI. A coarse level-1 grid is used for the steady-state ocean at rest, refined to level-2 grids for deep-ocean wave propagation. Level-3 grids resolve the compressed waves as they approach the coastal waters of the Hawaiin Islands, with meter-scale level-4 grids resolving the harbor and inundation of Hilo, HI (the actual inundation was limited to small onshore waves). See ([LeVeque, George, et al., 2011]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)) for more information.

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

<figure>
<img src="{{ site.baseurl }}/images/projects/geoclaw/tsunamis/honshu2hilo.gif">
</figure>

---
#### modeling overland flooding in rugged terrain: the Malpasset dam-break disaster, France, 1959.

<figure>
<img src="{{ site.baseurl }}/images/projects/geoclaw/malpasset/malpasset_dam_beforeafter.jpg">
</figure>

GeoClaw's algorithms are more generally applicable to free-surface water flows over topography, such as with overland flooding in steep terrain. This was applied to the Malpasset dam break disaster in southern France, 1959, which has served as a valuable benchmarking problem due to extensive field data. AMR allows the resolution of flood waters descending through a complex drainage within a larger bounding domain, avoiding the need of topographic mesh generation or prohibitively large uniform grids. This required an enhancement of the treatment of wet-dry interfaces within GeoClaw's Riemann solver (George, 2008), particularly where topographic jumps are high in steep terrain. See ([George, 2010]({{ site.baseurl }}/pubs/George2010_IJNMF.pdf)) for details.

<div class="gallery" data-columns="4">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00000.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00001.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00005.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00010.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00030.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00040.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00050.png">
	<img src="/images/projects/geoclaw/malpasset/oblique/frame00070.png">
</div>

<figure>
<img src="{{ site.baseurl }}/images/projects/geoclaw/malpasset/malpasset_oblique.gif">
</figure>

<div class="gallery" data-columns="4">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00000.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00005.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00010.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00020.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00030.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00050.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00060.png">
	<img src="/images/projects/geoclaw/malpasset/overhead/frame00120.png">
</div>

<figure>
<img src="{{ site.baseurl }}/images/projects/geoclaw/malpasset/malpasset_overhead.gif">
</figure>

### related publications

* **Finite volume methods and adaptive refinement for tsunami propagation and inundation,** D.L. George, 2006. *Ph.D. thesis*, University of Washington, Seattle. [pdf]({{ site.baseurl }}/pubs/George2006_Phd.pdf)
* **Augmented Riemann solvers for the shallow water equations over variable topography with steady states and inundation.** D. L. George, 2008. *J. Comput. Phys.*, 227(6): 3089--3113. [pdf]({{ site.baseurl }}/pubs/George2008_JCP.pdf)
* **Tsunami modeling with adaptively refined finite volume methods.** R.J. LeVeque, D.L. George and M.J. Berger, 2011. *Acta Numerica* 20, pp. 211--289. Arieh Iserles, ed. [pdf]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)
* **The GeoClaw software for depth-averaged flows with adaptive refinement.**  M. J. Berger, D. L. George, R. J. LeVeque and K. T. Mandli, 2011. *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016. [pdf]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)
* **Adaptive finite volume methods with well-balanced Riemann solvers for modeling floods in rugged terrain: application to the Malpasset dam-break flood (France, 1959).** D.L. George, 2010. *Int. J. Numer. Methods Fluids*, 66(8): 1000--1018. [pdf]({{ site.baseurl }}/pubs/George2010_IJNMF.pdf)
* **Finite volume methods for hyperbolic problems.** R.J. LeVeque, 2002. Texts in Applied Mathematics, Cambridge University Press.
* **Local adaptive mesh refinement for shock hydrodynamics.** M.J. Berger and P. Colella, 1989. *J. Comput. Phys.,* 82: 64-84.
* **Adaptive mesh refinement for storm surge.** K.T. Mandli and C.N. Dawson, 2014. *Ocean Modeling,* V. 75, 36-50.

