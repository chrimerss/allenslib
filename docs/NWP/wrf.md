---
layout: default
title: WRF simulations
parent: NWP
nav_order: 1
---

# General

[__The Weather Research and Forecasting Model: Overview, System Efforts, and Future Directions__](https://journals.ametsoc.org/view/journals/bams/98/8/bams-d-15-00308.1.xml#bib8)

This article introduces a variety range of WRF coupled models, across different fields.

# Extreme event simulations

[__Extreme rainfall from Hurricane Harvey (2017): Empirical intercomparisons of WRF simulations and polarimetric radar fields__](https://www.sciencedirect.com/science/article/pii/S0169809518314327#bb0210)

In this article, the authors simulated WRF in Harvey and use the radar simulator to compare the dual-polarimetric variables to observations for different microphysics options in WRF. They claim there is only weak dependence of TC tracks with microphysical schemes. The default Morrison simulation shows the beset match of rainfall accumulations.

configurations:

The horizontal grids are 300 × 300, 406 × 403 and 505 × 475, with horizontal grid spacing of 9 km, 3 km and 1 km, respectively. The vertical grids contain 50 sigma levels and the upper boundary is set at 50 hPa. The physics options we use are the Yonsei University (YSU) boundary layer scheme, the Rapid Radiative Transfer Model (RRTM) for longwave radiation, Dudhia's scheme for shortwave radiation and the Noah land surface model. The combination of physics options has been extensively tested in simulating landfalling TCs in previous studies (see e.g., Yang et al., 2017; Liu and Smith, 2016). The integral time steps for the three domains are 54 s, 18 s and 6 s, respectively. Initial and boundary conditions for WRF simulations are provided by the NCEP Global Forecast System (GFS) analyses (see https://rda.ucar.edu/datasets/ds083.3/ for more details), with a spatial resolution of 0.25-degree by 0.25-degree and temporal resolution of 6-hour.

[Assessing the Impacts of Different WRF Precipitation Physics in Hurricane Simulations](https://journals.ametsoc.org/view/journals/wefo/27/4/waf-d-10-05000_1.xml)

In this study, they compared all microphysical schemes for hurricane simulations including extreme rainfall and hurricane tracks. It was found the Lin scheme better produces the hurricane tracks.

configurations:

In all simulations, the 6-hourly analyses from the Global Forecast System (GFS), developed by the National Centers for Environmental Prediction (NCEP), were used as the initial and boundary conditions of the model. The simulation was performed in ‘‘predictive’’ mode, with observations only updated at boundaries throughout the simulation (i.e., no observation assimilation). The simulation began at 1200 UTC 21 September 2005, and continued until 1200 UTC 25 September 2005. The model settings were based on the Noah land surface model (Chen and Dudhia 2001), the Rapid Radiative Transfer Model (RRTM) longwave radiation scheme (Mlawer et al. 1997), the Dudhia shortwave radiation model (Dudhia 1989), and the Yonsei University (YSU) planetary boundary layer scheme (Hong et al. 2006; Hong and Dudhia 2003).

 
# Assimilating soil moisture into WRF framework

__[Examining the Impact of SMAP Soil Moisture Retrievals on Short-Range Weather Prediction under Weakly and Strongly Coupled Data Assimilation with WRF-Noah](https://journals.ametsoc.org/view/journals/mwre/147/12/mwr-d-19-0017.1.xml)__

This study provides a pseudo data assimilation of soil moisture from SMAP into WRF framework. They did cycling experiments and integration to investigate the impacts.

<p align="center">
 <img src="https://journals.ametsoc.org/view/journals/mwre/147/12/full-mwr-d-19-0017.1-f5.jpg">
</p>
