---
title: Software
subtitle: information and links to open-source software projects
description: information and links to open-source software projects
featured_image: /images/pages/Kaust_confroom_crop1.jpg
---

## Software development

#### Clawpack

Clawpack is an open-source project and software package for solving hyperbolic conservation laws (and related sytems of PDEs) utilizing adaptive finite volume wave propagation algorithms. For an overview, documentation, or other information on how to use or contribute, see the official Clawpack site, [clawpack.org](http://www.clawpack.org). Clawpack source-code, subpackages, and other repositories are hosted on github at [github.com/clawpack](https://github.com/clawpack).


#### GeoClaw

GeoClaw is open-source software for simulating shallow earth-surface flows involving water-wave propagation and inundation (*e.g.*, tsunamis, storm surges and general overland flooding problems). GeoClaw is a subpackage available with the latest versions (v5) of Clawpack, hosted on github at [github.com/clawpack](https://github.com/clawpack). Information related specifically to GeoClaw is available at [geoclaw.org](http://www.geoclaw.org).  


#### D-Claw

D-Claw is an open-source package for modeling shallow two-phase flows, such as dense granular-fluid mixtures like landslides and debris flows. It can also be used for modeling hybrid problems involving the interaction of variably concentrated granular mixtures and water (*eg.*, landslide-generated tsunamis, dam breach floods, fluid or solid entrainment by inundating or overlying flows). D-Claw was developed in collaboration with Richard Iverson at the USGS. A detailed description of the model underlying the D-Claw software can be found in, **A depth-averaged debris-flow model that includes the effects of evolving dilatancy,** *Proc. R. Soc. A*, 470 (2170), **1.** Iverson & George and **2.** George & Iverson, 2014. 

The documentation for the latest version of Clawpack and GeoClaw (v5), available at [clawpack.org](http://www.clawpack.org), provides a general overview of the methodologies underlying the D-Claw software. However, D-Claw is built on legacy versions of Clawpack and GeoClaw (v4). The Clawpack v4 source code is available at [github.com/clawpack/clawpack-4.x](https://github.com/clawpack/clawpack4.x). An additional legacy version of GeoClaw (v4) is available at [github.com/geoflows/geoclaw-4.x](https://github.com/geoflows/geoclaw4.x) Documentation for D-Claw is still in progress, but basic usage instructions are available in source-code and application repositories below.

The source code and latest git repository for D-Claw are available on github:

* [github.com/geoflows/D-Claw](https://github.com/geoflows/D-Claw).

A repository for applications is also available:

* [github.com/geoflows/dclaw-apps](https://github.com/geoflows/dclaw-apps).

The application repository is in progress, as is documentation for D-Claw. If you would like to make contributions to either of these repositories, please follow the development workflow used for Clawpack, described at [www.clawpack.org/developers](http://www.clawpack.org/developers.html). Briefly, please fork the repositories to your own github account, develop on a new or feature branch, and issue pull requests from that branch to github/geoflows.

Example of development workflow below. 

```
git clone git://github.com/geoflows/D-Claw.git
cd D-Claw
git remote add username htpps://github.com/username/D-Claw.git
```
or fork on github to username and fork that.
or if you have ssh keys and want to avoid typing your password when you push to github:

```
git remote add username git@github.com:username/D-Claw.git
```
Develop in a branch other than master:
```
git checkout -b my_branch
```
And then push to your repository:
```
git push username my_branch
```
Issue pull requests to geoflows/D-Claw from your repository to contribute to D-Claw. Update your master branches from geoflows/D-Claw:
```
git pull origin master
```
If you prefer, rename origin to something easy to remember ("geoflows" or "upstream" or similar):
```
git remote rename origin geoflows
```

D-Claw inherits the Clawpack licenses and user agreeements. 




