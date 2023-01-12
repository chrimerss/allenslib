---
layout: default
title: Hydrologic Modelling
parent: Hydrology
nav_order: 12
---

# Model review

__[Physically based modeling in catchment hydrology at 50: Survey and outlook WRR](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2015WR017780)__

__[Why do we have so many different hydrological models? A review based on the case of Switzerland](https://wires.onlinelibrary.wiley.com/doi/10.1002/wat2.1574)__

__[100 Years of Progress in Hydrology](https://journals.ametsoc.org/view/journals/amsm/59/1/amsmonographs-d-18-0019.1.xml)__

__[Global river hydrography and network routing: baseline data and new approaches to study the world's large river systems](https://onlinelibrary.wiley.com/doi/10.1002/hyp.9740)__

The authors laid out high-level comparisons between vector-based and raster-based routing.

__[More complex is not necessarily better in large scale hydrological modelling - A model complexity experiment across the contiguous United States](https://journals.ametsoc.org/view/journals/bams/aop/BAMS-D-21-0284.1/BAMS-D-21-0284.1.xml?tab_body=pdf)__

The authors used semi-distributed models and flexible structure and parameter set to conduct US-continental scale model evaluation. The results suggest in contrast that increases in number of soil layers do not imporve model performance but separation of fast flow/slow flow do so.


# Global hydrologic model

__[Technical review of large-scale hydrological models for implementation in operational flood forecasting schemes on continental level](https://www.sciencedirect.com/science/article/pii/S1364815215300529)__



## PCR-GLOBWB

__[PCR-GLOBWB 2: a 5 arcmin global hydrological and water resources model (GMD)](https://gmd.copernicus.org/articles/11/2429/2018/)__

Model structure is as follows. This paper detailed description of each modeling component: irrigation and water use, land surface, groundwater, and surface water routing.

![model_struc](https://gmd.copernicus.org/articles/11/2429/2018/gmd-11-2429-2018-f01-web.png)

# Runoff routing models

## Vector-based routing

### MizuRoute

__[A Vector-Based River Routing Model for Earth System Models: Parallelization and Global Applications](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002434)__

This paper presents a global implementation of MizuRoute modeling, coupled with Earth System Models. They specifically investigated the impact of parallelization on runoff simulations.

### RAPID

__[Implementation of a vector-based river network routing scheme in the community WRF-Hydro modeling framework for flood discharge simulation](https://www.sciencedirect.com/science/article/pii/S1364815217313531#bib12)__

Paper described the process coupling vector-based routing and WRF-Hydro for flood forecast.

They assessed the impact of LSM resolutions on vector routing results.

"as a river goes downstream and aggregates a larger contributing area, the model errors resulted from various upstream locations tend to be cancelled out."

__[Towards Real-Time Continental Scale Streamflow Simulation in Continuous and Discrete Space](https://onlinelibrary.wiley.com/doi/10.1111/1752-1688.12586)__

RAPID routing with reservoir regulation included

### AutoRoute

__[AutoRAPID: A Model for Prompt Streamflow Estimation and Flood Inundation Mapping over Regional to Continental Extents](https://onlinelibrary.wiley.com/doi/full/10.1111/1752-1688.12476)__

A rapid flood inundation mapping tool for large scale flood simulations.

## Raster routing

### MOSART (used in CESM)

__[A Physically Based Runoff Routing Model for Land Surface and Earth System Models](https://journals.ametsoc.org/view/journals/hydr/14/3/jhm-d-12-015_1.xml)__

# Improvement to hydrologic processes

## Surface-groundwater exchange

__[Representation of bi-directional fluxes between groundwater and surface water in a bucket type hydrologic model - WRR](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028835)__

In this article, the authors enabled streamflow and groundwater interaction in bi-direction to a comceptual model, meaning streamflow can seepage to groundwater when groundwater level is lower than stream water level which is calculated using the rating curve.

It is an inspirational research that encourages us to account for this two-way interaction especially in intermittent streams where streamflow loss is a main contributor.

## Inclusion of reservoir module

__[Accuracy vs. Realism: DOes including reservoirs improve hydrologic models? - frontiers](file:///Users/allen/Downloads/accuracy-vs-realism-does-including-reservoirs-improve-hydrological-models.pdf)__

This study, the authors proposed adding a reservoir module to lumped hydrologic models to better enhance the realism and accuracy. Indeed, they found reservoir module significantly improves hydrologic responses than without it.

## Importance of routing in Global Climate Models

__[On the Suitability of GCM Runoff Fields for River Discharge Modeling: A Case Study Using Model Output from HadGEM2 and ECHAM5](https://journals.ametsoc.org/view/journals/hydr/13/1/jhm-d-10-05011_1.xml)__

The authors compared direct runoff output from GCMs, routed runoff, and offline global hydrological model (PCR-GLOBWB). The importance of routing, especially for small basins is underlined.

# Hydrologic calibdation
__[Calibrating a hydrological model in a regional river of the Qinghai–Tibet plateau using river water width determined from high spatial resolution satellite images.](https://www.sciencedirect.com/science/article/pii/S0034425718302414?via%3Dihub)__

This paper introduces the first attempt to calibrate a hydrologic model based on river width data derived from commercial satellites. Likewise, this approach is highly suitable in hydrodynamic models because we can estimate river width at given cross-sections.

__[Combining optical remote sensing, McFLI discharge estimation, global hydrologic modelling, and data assimilation to improve daily discharge estimates across an entire large watershed ](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR027794)__

In this paper, the authors used LandSat to reconstruct river width and eventually use flow law to infer discharge. They assimulated the discharge with acknowledging all uncertainty terms and compared against GRADES as baseline, and they found a significant improvement. The reach-level routing is computationally efficient for global or large scale hydrologic modelling.

__[In Quest of Calibration Density and Consistency in Hydrologic Modeling: Distributed Parameter Calibration against Streamflow Characteristics](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018WR024178)__

In this article, the authors pointed out two ways of calibrating hydrologic models on a large scale: 1. hydrologic regionalization for model parameters based on basin characteristics or regressions; 2. regionalization on streamflow, and use it as the target to calibrate the model. This paper targets the latter one.

They calibrated three sensitive parameters from the VIC model against four streamflow signatures: Qmean, Q10, Q90, and base flow index. These values are calculated from gauges II dataset. They present a significant improvement comparing the calibrated model and non-calibrated model. Also, they pointed out some regions that reluctant to calibrations, such as arid regions.

__[Global Fully Distributed Parameter Regionalization Based on Observed Streamflow From 4,229 Headwater Catchments](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019JD031485)__

In this paper, the authors calibrated the gridded HBV model at daily scale globally to obtain a distributed parameters, and they regressed calibrated parameters to ungauged regions via a transfer function (regression).
They are able to obtain a median KGE of 0.46, improved from 0.29 on average. They also analyzed regionalizations of those parameters to gain a physical understanding.

__[Toward seamless hydrologic predictions across spatial scales](https://hess.copernicus.org/articles/21/4323/2017/)__

A general protocol of how to apply parameterization of earth system models in predicting hydrologic response across scales.

The most common parameterization techniques found in the literature are (1) look-up tables (LUTs), (2) manual or automatic calibration, (3) hydrologic response units (HRUs), (4) representative elementary watersheds (REWs), (5) a priori regularization functions, (6) simultaneous regionalization/regularization functions, and (7) dissimilarity-based metrics to transfer model parameters.

# Model evaluation

__[When best is the enemy of good – critical evaluation of performance criteria in hydrological models (HESS)](https://hess.copernicus.org/preprints/hess-2022-380/hess-2022-380.pdf)__

The authors compared a comprehensive list of evaluation factors such as NSE, KGE, KGE', and other variants to showcase their deficiencies in some extent, particularly the counter-balancing errors. Depending on the overall perspective, authors urge careful selection of evaluation criterion for hydrological model calibration and validation.
