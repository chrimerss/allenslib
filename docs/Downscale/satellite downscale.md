---
layout: default
title: satellite downscale
parent: Downscale
nav_order: 1
---

__Ma, Z., et al. (2019). "An updated moving window algorithm for hourly-scale satellite precipitation downscaling:
a case study in the Southeast Coast of China." Journal of Hydrology.__

Author synthesized IMERG data and coupled with cloud properties e.g. cloud   effective   radius   (CER),
cloud   top   height   (CTH),   cloud   top temperature (CTT) and cloud optical thickness (COT) to perform hourly based satellite QPE
downscale. 

According to the result, CER is the one that affects downscale performances most.

<p align="center">
<img src="https://chrimerss.github.io/allenslib/src/IMERG_downscale_clouds_flowchart.png" width="60%">
</p>
<p align="center">Fig. Flowchart of processing downscaling.</p>

__Abbaszadeh, P., Moradkhani, H., & Zhan, X. (2019). Downscaling SMAP radiometer soil moisture over the CONUS using an ensemble learning method. Water Resources Research, 55, 324–344. https://doi.org/10.1029/2018WR023354__

<p align="center">
  <img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/7d90a42a-b20e-4282-b559-daa87e14d348/wrcr23736-fig-0001-m.jpg" width="60%">
</p>
<p align="center">Fig. Flowchart of processing downscaling SMAP.</p>

Insights:

1. The validations used in this article are primitive: (a) in-situ evaluation over verification period; (b) downscaled temporal dynamics is evaluated by looking at the time series; (c) spatial heterogeneity is evaluated; (d) further validation based on two subregions that contains different geophysical properties.

2. The datasets used: (a) SMAP level-3 9-km; (b) MODIS land surface temporature and NDVI; (c) NWS 4-km precipitation; (d) CONUS soil data; (e) topography data (slope, elevation, etc.)
