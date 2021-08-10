---
layout: default
title: Hydrologic Modelling
parent: Hydrology
nav_order: 12
---

# Global hydrologic model

## PCR-GLOBWB

__[PCR-GLOBWB 2: a 5 arcmin global hydrological and water resources model (GMD)](https://gmd.copernicus.org/articles/11/2429/2018/)__

Model structure is as follows. This paper detailed description of each modeling component: irrigation and water use, land surface, groundwater, and surface water routing.

![model_struc](https://gmd.copernicus.org/articles/11/2429/2018/gmd-11-2429-2018-f01-web.png)

# Vector-based runoff routing

## MizuRoute

__[A Vector-Based River Routing Model for Earth System Models: Parallelization and Global Applications](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002434)__

This paper presents a global implementation of MizuRoute modeling, coupled with Earth System Models. They specifically investigated the impact of parallelization on runoff simulations.


# Improvement to hydrologic processes

## Surface-groundwater exchange

__[Representation of bi-directional fluxes between groundwater and surface water in a bucket type hydrologic model - WRR](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028835)__

In this article, the authors enabled streamflow and groundwater interaction in bi-direction to a comceptual model, meaning streamflow can seepage to groundwater when groundwater level is lower than stream water level which is calculated using the rating curve.

It is an inspirational research that encourages us to account for this two-way interaction especially in intermittent streams where streamflow loss is a main contributor.
