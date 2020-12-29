---
layout: default
title: Flood Analysis
parent: Hydrology
nav_order: 3
---


# Global Flood Analysis

__[Global modeling of seasonal mortality rates from river floods](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020EF001541)__

In this paper published in Earth's Future, the authors specifically dissect the seasonal response of the global flood events (including the peak timing, peak distribution, flood impact, mortality rate) with the aid of global hydrological model LISFLOOD (GloFAS-Reanalysis dataset v3.0: https://data.jrc.ec.europa.eu/collection/id-00288)

From the analysis, they not only represent major watersheds in the globe for the pure flood generation, but also sheding lights on political boundaries (i.e. countries) for flood assessment since measures have been taken differently with countries.

It is claimed as the first paper to study on global seasonal flood analysis.

__[Sampson, C. C., A. M. Smith, P. D. Bates, J. C. Neal, L. Alfieri, and J. E. Freer (2015), A high-resolution global flood hazard model, Water Resour. Res., 51, 7358–7381, doi:10.1002/2015WR016954.](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1002/2015WR016954)__

In this paper, the authors presented six challenges for global flood risk mapping and came with their solutions:

1. reliable terrain data

2. extreme flow generation either by hydrologic model or regional flood frequency analysis

3. global river networks

They approached the river width by using web-survey, and the river depth is estimated based on 1 or 2 year return period discharge as bankfull discharge. With bankful discharge, channel width, and slope, the channel depth could be approached by manning's equation.

4. Flood defenses

This is more challenging than the other because the structure is way smaller than the modelling grid-cell size

5. Computational Hydraulic Engine

"A novel simplified implementation of shallow water equations yielded an glgorithm for which the minimum stable time step scales linearly with decreasing grid size, rather than quadratically as had been the case with previous diffusion wave formulations"

"The study determined that inclusion of both the channel network and floodplain was essential, and that
inclusion of the smaller subgrid channels on the floodplain yielded significantly increased simulation accuracy in terms of water level, wave propagation speed, and inundation extent"

6. Automation Framework


# Regional Flood analysis

__[Combined modelling of US fluvial, pluvial and coastal flood hazard under current and future climates](https://www.essoar.org/pdfjs/10.1002/essoar.10504362.1)__

In this paper, the authors updated the current US continental flood hazard maps with assigned frequency under different scenarios (historical, present, and projection). They highlighted the changes in hydrography data, surface water profile, extreme event magnitudes, downscaling using hi-res. terrain data, and incorporated local interventions.

They detailed how the boundary conditions are derived for the consideration of fluvial (IDF forced hydrologic simulation) and coastal flooding (tide gauge data), while for pluvial flooding, they simply uses rain-on-grid simulations at each 30 m grid. 

They indicate the ensemble prediction is important to better quantify the uncertainties and more model validation efforts are needed.

__[Implications of Using Global Digital Elevation Models for Flood Risk Analysis in Cities](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028241)__

In this paper, the authors compared six globbaly available DEM data, and assessed how the DEM coupld affect urban flood forecast. They found OS Terrain 50 has the best statistics when validated against high water marks and flood extent derived from photos, videos.

They finally discussed that the outlet water level data in water channles does not nessarily need to be accurate in impact studies if peak floodplain extent is accurate enough.

__[How probable is widespread flooding in the United States?](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028096)__

In this paper, the authors used a stochastic streamflow generator built upon 38 years USGS streamflow data conditioned on main 18 catchments to investigate the spatial distribution of flood events in dependence of flood susceptibility. 

They found a strong dependence of flood susceptibility and seasonality in parts of the US, especially western US. Some catchments governed by intermittent streamflow however exhibits less seasonality. Catchments with snowmelting dominant streamflow generation has high susceptibility in spring and winter.

__[Quantifying the importance of spatial resolution and other factors through global sensitivity analysis of a flood inundation model](https://doi.org/10.1002/2015WR018198)__

In this paper, the authors firstly evaluate the model sensitivity with respect to parameters, inflow and topography in terms of flood dynamics. They not only simulated based on bulk flow, but also spatiotemporal variation of flood dynamics. It is worth trying to conduct similar research for CREST-iMAP model parameters or probabilistic QPEs.

__[A COMPREHENSIVE DATABASE OF FLOOD EVENTS IN THE CONTIGUOUS UNITED STATES FROM 2002 TO 2013](https://journals.ametsoc.org/bams/article/98/7/1493/70155/A-Comprehensive-Database-of-Flood-Events-in-the)__

The authors constructed US flood database based on gauge data and precipitation data to separate baseflow from flood events.






