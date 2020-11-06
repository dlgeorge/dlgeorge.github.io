---
title: 'Landslide tsunamis'
subtitle: 'modeling landslides, wave generation, and tsunamis with D-Claw'
date: 2017-01-01 00:00:00
description: Case study - the 2015 Tyndall Glacier (Alaska) landslide and tsunami.
featured_image: '/images/projects/tyndall/ObliqueDClaw60s.png'
---


### Tyndall Glacier and Taan Fjord, Alaska

This page features material from:

New methodology for computing tsunami generation by subaerial landslides: application to the 2015 Tyndall Glacier Landslide, Alaska. D. L. George, R.M. Iverson and C.M. Cannon, 2017. *Geophys. Res. Lett.*, V. 44(14), 7276--7284. [pdf]({{ site.baseurl }}/pubs/GeorgeIversonEtAl2017_GRL_Tyndall.pdf).

![](/images/projects/tyndall/ObliqueDClaw30s.png)

---
#### Abstract

<small>Landslide-generated tsunamis pose significant hazards and involve complex, multiphase physics that are challenging to model. We present a new methodology in which our depth-averaged two-phase model D-Claw is used to seamlessly simulate all stages of landslide dynamics as well as tsunami generation, propagation, and inundation. Because the model describes the evolution of solid and fluid volume fractions, it treats both landslides and tsunamis as special cases of a more general class of phenomena. Therefore, the landslide and tsunami can be efficiently simulated as a single-layer continuum with evolving solid-grain concentrations, and with wave generation via direct longitudinal momentum transfer—a dominant physical mechanism that has not been previously addressed in this manner. To test our methodology, we used D-Claw to model a large subaerial landslide and resulting tsunami that occurred on 17 October 2015, in Taan Fjord near the terminus of Tyndall Glacier, Alaska. Modeled shoreline inundation patterns compare well with those observed in satellite imagery.</small>

---
#### Modeling preview

<figure>
<figcaption> The simulated landslide initiation and generation of impulse waves. The color scale indicates the evolving solid-volume fraction. Model set-up and animations provided below.</figcaption>
<div class="gallery" data-columns="3">
	<img src="/images/projects/tyndall/ObliqueDClaw00s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw10s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw20s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw30s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw40s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw50s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw60s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw70s.png">
	<img src="/images/projects/tyndall/ObliqueDClaw80s.png">
</div>
</figure>

<figure>
<figcaption>The simulated landslide initiation and generation of impulse waves. The color scale indicates the evolving surface elevation. Model set-up and animations provided below.</figcaption>
<div class="gallery" data-columns="3">
	<img src="/images/projects/tyndall/OverheadDClaw000s.png">
	<img src="/images/projects/tyndall/OverheadDClaw100s.png">
	<img src="/images/projects/tyndall/OverheadDClaw200s.png">
	<img src="/images/projects/tyndall/OverheadDClaw300s.png">
	<img src="/images/projects/tyndall/OverheadDClaw400s.png">
	<img src="/images/projects/tyndall/OverheadDClaw500s.png">
</div>
</figure>

---
#### The 2015 Tyndall Glacier landslide and tsunami, Taan Fjord, Alaska.

At about 8:19 P.M. (local time) on 17 October 2015, after a period of heavy rain, a large landslide occurred near the toe of Tyndall Glacier, which originates on the flanks of Mount St. Elias and terminates at the head of Taan Fjord and Icy Bay, Alaska. Runout of the 2015 landslide generated a tsunami in Taan Fjord that reached vertically 150 m up a hillside on the opposite side of the fjord (Rozell, 2016). Landslide mass estimates from the long-period seismicity radiated by the landslide were about 180 billion kg, which implies a volume of about 70–80 million cubic meters (Stark, 2015). 

<figure>
<figcaption> The landslide source area (a) in relation to Icy Bay and (b) in relation to southeast Alaska. (c) A photograph
taken following the landslide (courtesy of Christopher Larsen, University of Alaska, Fairbanks) provides an oblique view
of the Tyndall Glacier terminus and adjacent landslide source area.
</figcaption>

<img src="{{ site.baseurl }}/images/projects/tyndall/IcyBay.png">
</figure>

To draw further inferences about the scope of the event, we used satellite imagery acquired beforehand and shortly afterward (ASTER, Landsat, and Earth Observing 1-Advanced Land Imager). We constructed hypothetical landslide source models (basal failure surfaces and landslide-mass geometries) and simulated landslides, tsunami generation, wave propagation, and inundation along Taan Fjord with several methodologies including D-Claw. Computational results are compared to satellite derived data.

<figure>
<figcaption>(a) Map view and (b) vertical cross-section profile of the landslide source area near the terminus of the Tyndall
Glacier. Three longitudinal transects crossing the landslide source identify the location of fitted logarithmic spirals used
to estimate the shape of the continuous failure surface. The vertical cross section (Figure 2b) is along the dark transect
shown in Figure 2a.
</figcaption>

<img src="{{ site.baseurl }}/images/projects/tyndall/LandslideSource.png">
</figure>

---
#### Animations

<figure>
<figcaption>The simulated landslide initiation and generation of impulse waves. The color scale indicates the evolving
solid-volume fraction.</figcaption>
<img src="{{ site.baseurl }}/images/projects/tyndall/Tyndall_oblique_grl.gif">
</figure>



<figure>
<figcaption>The simulated landslide initiation and generation of impulse waves. The color scale indicates the evolving surface elevation.</figcaption>
<img src="{{ site.baseurl }}/images/projects/tyndall/Tyndall_overhead_grl.gif">
</figure>

---
#### Comparison of modeling approaches and data

<figure>
<figcaption>NDVI images indicating the decreased vegetation caused by tsunami inundation near the shoreline of the
Taan Fjord. The extent of the inundation predicted by D-Claw is outlined in black.</figcaption>
<img src="{{ site.baseurl }}/images/projects/tyndall/NDVI_2panel.png">
</figure>

<figure>
<figcaption>Time series of the simulated tsunami at five chosen locations in Taan Fjord and Icy Bay, showing the wave
heights relative to the undisturbed water elevation (−1.07 msl). Results of the seamless D-Claw simulation (red) are
compared to those of the precomputed variable bottom simulation (dotted blue). Locations of the time series are
indicated on the map as triangles near labels G1–G5. All locations are downstream of the reach of significant
solid material. </figcaption>
<img src="{{ site.baseurl }}/images/projects/tyndall/TsunamiGauges.png">
</figure>


---
#### Conclusions

Our seamless D-Clawsimulations of the Tyndall Glacier landslide and Taan Fjord tsunami used an uncalibrated
model but produced shoreline inundation patterns that are consistent with the data currently available.More
in-depth comparisons would require higher-resolution bathymetry and topography as well as additional
field data. Comparisons of two alternative approaches (seamless versus precomputed landslide and evolving
seafloor) predict similar tsunami waves in Taan Fjord and Icy Bay. Thus, the two approaches would likely lead
to similar assessments of inundation hazards in this particular case. However, the seamless approach using
D-Claw has clear computational and methodological advantages because it avoids the step of precomputing
an evolving spatiotemporal landslide surface, and the mass and momentum of the system are automatically
resolved owing to the absence of quasi-coupled model interfaces. Our results suggest that D-Claw can
simulate the impulse waves associated with subaerial landslide tsunamis with sufficient fidelity for hazard
forecasting.

---
#### References

* Rozell, N. (2016), **The Giant Wave of Icy Bay**, *Geophys. Inst. AK Press Release*, Fairbanks, Alaska. Available at [www.gi.alaska.edu/alaska-science-forum/giant-wave-icy-bay](http://www.gi.alaska.edu/alaska-science-forum/giant-wave-icy-bay).
* Stark, C. P. (2015), **Landslide dynamics from seismology: New results,** Abstract EP51D-08 presented at 2015 Fall Meeting, *AGU*, San Francisco.




