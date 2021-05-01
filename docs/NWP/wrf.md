
---
layout: default
title: WRF simulations
parent: NWP
nav_order: 1
---

# Extreme event simulations

[__Extreme rainfall from Hurricane Harvey (2017): Empirical intercomparisons of WRF simulations and polarimetric radar fields__](https://www.sciencedirect.com/science/article/pii/S0169809518314327#bb0210)

In this article, the authors simulated WRF in Harvey and use the radar simulator to compare the dual-polarimetric variables to observations for different microphysics options in WRF. They claim there is only weak dependence of TC tracks with microphysical schemes. The default Morrison simulation shows the beset match of rainfall accumulations.

configurations:

The horizontal grids are 300 × 300, 406 × 403 and 505 × 475, with horizontal grid spacing of 9 km, 3 km and 1 km, respectively. The vertical grids contain 50 sigma levels and the upper boundary is set at 50 hPa. The physics options we use are the Yonsei University (YSU) boundary layer scheme, the Rapid Radiative Transfer Model (RRTM) for longwave radiation, Dudhia's scheme for shortwave radiation and the Noah land surface model. The combination of physics options has been extensively tested in simulating landfalling TCs in previous studies (see e.g., Yang et al., 2017; Liu and Smith, 2016). The integral time steps for the three domains are 54 s, 18 s and 6 s, respectively. Initial and boundary conditions for WRF simulations are provided by the NCEP Global Forecast System (GFS) analyses (see https://rda.ucar.edu/datasets/ds083.3/ for more details), with a spatial resolution of 0.25-degree by 0.25-degree and temporal resolution of 6-hour.

