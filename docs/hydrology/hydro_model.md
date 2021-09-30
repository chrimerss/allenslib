---
layout: default
title: Hydrologic Modelling
parent: Hydrology
nav_order: 12
---

# Global hydrologic model

__[Technical review of large-scale hydrological models for implementation in operational flood forecasting schemes on continental level](https://www.sciencedirect.com/science/article/pii/S1364815215300529)__



## PCR-GLOBWB

__[PCR-GLOBWB 2: a 5 arcmin global hydrological and water resources model (GMD)](https://gmd.copernicus.org/articles/11/2429/2018/)__

Model structure is as follows. This paper detailed description of each modeling component: irrigation and water use, land surface, groundwater, and surface water routing.

![model_struc](https://gmd.copernicus.org/articles/11/2429/2018/gmd-11-2429-2018-f01-web.png)

# Vector-based runoff routing

## MizuRoute

__[A Vector-Based River Routing Model for Earth System Models: Parallelization and Global Applications](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002434)__

This paper presents a global implementation of MizuRoute modeling, coupled with Earth System Models. They specifically investigated the impact of parallelization on runoff simulations.

## RAPID

__[Implementation of a vector-based river network routing scheme in the community WRF-Hydro modeling framework for flood discharge simulation](https://www.sciencedirect.com/science/article/pii/S1364815217313531#bib12)__

Paper described the process coupling vector-based routing and WRF-Hydro for flood forecast.

They assessed the impact of LSM resolutions on vector routing results.

"as a river goes downstream and aggregates a larger contributing area, the model errors resulted from various upstream locations tend to be cancelled out."

## AutoRoute

__[AutoRAPID: A Model for Prompt Streamflow Estimation and Flood Inundation Mapping over Regional to Continental Extents](https://onlinelibrary.wiley.com/doi/full/10.1111/1752-1688.12476)__

A rapid flood inundation mapping tool for large scale flood simulations.



# Improvement to hydrologic processes

## Surface-groundwater exchange

__[Representation of bi-directional fluxes between groundwater and surface water in a bucket type hydrologic model - WRR](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028835)__

In this article, the authors enabled streamflow and groundwater interaction in bi-direction to a comceptual model, meaning streamflow can seepage to groundwater when groundwater level is lower than stream water level which is calculated using the rating curve.

It is an inspirational research that encourages us to account for this two-way interaction especially in intermittent streams where streamflow loss is a main contributor.

## Inclusion of reservoir module

__[Accuracy vs. Realism: DOes including reservoirs improve hydrologic models? - frontiers](file:///Users/allen/Downloads/accuracy-vs-realism-does-including-reservoirs-improve-hydrological-models.pdf)__

This study, the authors proposed adding a reservoir module to lumped hydrologic models to better enhance the realism and accuracy. Indeed, they found reservoir module significantly improves hydrologic responses than without it.
