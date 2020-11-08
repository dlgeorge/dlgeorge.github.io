---
title: Software
subtitle: information and links to open-source projects
description: information and links to open-source software projects
featured_image: /images/pages/Kaust_confroom_crop1.jpg
---

## Open-source software packages for wave propagation and surface flows.

---
### Clawpack


Clawpack is an open-source project and collection of software packages for hyperbolic conservation laws and related sytems of PDEs. These systems commonly govern problems exhibiting wave-propagation which arise across the scientific disciplines. 

#### overview

Clawpack was established in 1994 by Randall LeVeque (Univ. of Wash.) to implement a finite volume framework utilizing wave-propagation algorithms applicable to general nonlinear hyperbolic systems. These numerical methods belong to the class of high-resolution Godunov schemes with limiters which provide stability and convergence to physically admissable discontinuous weak solutions, such as shock-capturing for conservation laws. Clawpack also provides patch-based adaptive mesh refinement (AMR) originally developed by Marsha Berger (NYU) and later formulated in the numerical wave-propagation framework. For more information and links to relevant publications and research, see the official Clawpack site: [clawpack.org](http://www.clawpack.org).
 
#### source code and repositories

Clawpack source code and repositories are hosted on github: 

* [github.com/clawpack](https://github.com/clawpack). 

Links to documentation and instructions for developers can also be found at [clawpack.org](http://www.clawpack.org).

---
### GeoClaw

GeoClaw is an open-source package within the Clawpack project for simulating shallow earth-surface flows involving water-wave propagation and inundation (*e.g.*, tsunamis, storm surges and general overland flooding problems).

#### overview

GeoClaw evolved from a collection of algorithms developed for modeling tsunamis in the Clawpack adaptive numerical framework (George, 2006; George, 2008; LeVeque, George, et al., 2011). These algorithms provide robust inundation capturing and well-balanced resolution in the presence of dominant steady states (e.g., ocean at rest). Additionally, AMR schemes that preserve well-balancing and inundation capturing in conjunction with mass, momentum and energy conservation enable global-scale tsunami propagation and local-scale inundation in reasonably efficient single simulations. These methods are more generally applicable to shallow free-surface flows over topography, which motivated the extension of GeoClaw to overland flooding problems in irregular terrain (e.g, George, 2010; Berger, George, et al., 2011). Later extensions of these algorithms were developed for storm-surge applications (e.g., Mandli, 2014). GeoClaw is now used for a variety of applications involving shallow water flows over topography. Features and enhancements continue to be developed within the Clawpack project (e.g., Mandli, Ahmadia, et al., 2016). See [Projects](/projects/) for some examples and galleries and [geoclaw.org](http://www.geoclaw.org) for links to related research.
  
#### source code and repositories

GeoClaw is a subpackage available with the latest versions (v5) of Clawpack, hosted on github:

* [github.com/clawpack](https://github.com/clawpack). 

Information related to GeoClaw development is available at the official Clawpack site ([clawpack.org](http://www.clawpack.org)) and [geoclaw.org](http://www.geoclaw.org). 

---
### D-Claw

D-Claw is an open-source package for modeling shallow two-phase flows, such as dense granular-fluid mixtures like landslides and debris flows. It can also be used for modeling hybrid problems involving the interaction of variably concentrated granular mixtures and water (*eg.*, landslide-generated tsunamis, dam breach floods, fluid or solid entrainment by inundating or overlying flows). 

#### overview

D-Claw was developed in collaboration with Richard Iverson at the USGS. It embodies a synthesis of the independent lines of research behind Clawpack and GeoClaw with granular dynamics and landslide physics research by Iverson (e.g., Iverson, 1997). A detailed description of the model underlying the D-Claw software is provided by Iverson & George (2014) and George & Iverson (2014). For further background information and some application examples, see [projects](/projects/)

#### source code and repositories

The documentation for the latest version of Clawpack and GeoClaw (v5), available at [clawpack.org](http://www.clawpack.org), provides a general overview of the methodologies underlying the D-Claw software. However, D-Claw is built on legacy versions of Clawpack and GeoClaw (v4). The Clawpack v4 source code is available at [github.com/clawpack/clawpack-4.x](https://github.com/clawpack/clawpack4.x). An additional legacy version of GeoClaw (v4) is available at [github.com/geoflows/geoclaw-4.x](https://github.com/geoflows/geoclaw4.x). D-Claw documentation is still in progress, but basic usage instructions are available in source-code and application repositories below. D-Claw inherits the Clawpack licenses and user agreeements. 

The source code and latest git repository for D-Claw are available on github:

* [github.com/geoflows/D-Claw](https://github.com/geoflows/D-Claw).

A repository for applications is also available:

* [github.com/geoflows/dclaw-apps](https://github.com/geoflows/dclaw-apps).

The application repository is in progress, as is documentation for D-Claw. If you would like to make contributions to either of these repositories, please follow the development workflow used for Clawpack, described at [www.clawpack.org/developers](http://www.clawpack.org/developers.html). Briefly, please fork the repositories to your own github account, develop on a new or feature branch, and issue pull requests from that branch to github/geoflows.


### References 

* **Local adaptive mesh refinement for shock hydrodynamics.** M.J. Berger and P. Colella, 1989. *J. Comput. Phys.,* 82: 64-84. 
* **The GeoClaw software for depth-averaged flows with adaptive refinement.**  M. J. Berger, D. L. George, R. J. LeVeque and K. T. Mandli, 2011. *Advances in Water Resources*, 34: 1195--1206. doi: 10.1016/j.advwatres.2011.02.016. [pdf]({{ site.baseurl }}/pubs/BergerGeorgeEtAl2011_AWR.pdf)
* **Finite volume methods and adaptive refinement for tsunami propagation and inundation,** D.L. George, 2006. *Ph.D. thesis*, University of Washington, Seattle. [pdf]({{ site.baseurl }}/pubs/George2006_Phd.pdf)
* **Augmented Riemann solvers for the shallow water equations over variable topography with steady states and inundation.** D. L. George, 2008. *J. Comput. Phys.*, 227(6): 3089--3113. [pdf]({{ site.baseurl }}/pubs/George2008_JCP.pdf)
* **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 2. Numerical predictions and experimental tests.** D. L. George and R. M. Iverson, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/GeorgeIverson2014_ProcRSocA.pdf) 
*  **A depth-averaged debris-flow model that includes the effects of evolving dilatancy: 1. Physical basis.** R. M. Iverson and D. L. George, 2014. *Proc. R. Soc. A*, 470 (2170). [pdf]({{ site.baseurl }}/pubs/IversonGeorge2014_ProcRSocA.pdf)
* **Finite volume methods for hyperbolic problems.** R.J. LeVeque, 2002. Texts in Applied Mathematics, Cambridge University Press.
* **Tsunami modeling with adaptively refined finite volume methods.** R.J. LeVeque, D.L. George and M.J. Berger, 2011. *Acta Numerica* 20, pp. 211--289. Arieh Iserles, ed. [pdf]({{ site.baseurl }}/pubs/LeVequeGeorgeEtAl2011_ActaNumerica.pdf)
* **Adaptive mesh refinement for storm surge.** K.T. Mandli and C.N. Dawson, 2014. *Ocean Modeling,* V. 75, 36-50.
*  **Clawpack: building an open source ecosystem for solving hyperbolic PDEs.** K.T. Mandli, A.J. Ahmadia, M.J. Berger, D. Calhoun, D.L. George, Y. Hadjimichael, D.I. Ketcheson, G.I. Lemoine and R.J. LeVeque, 2016. *Peer J Computer Science*, 2, e68. [pdf]({{ site.baseurl }}/pubs/MandliAhmadiaEtAl2016_PeerJ_clawpack.pdf)







