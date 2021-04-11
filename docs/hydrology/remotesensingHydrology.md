---
layout: default
title: Remote Sensing hydrology
parent: Hydrology
nav_order: 1
---

__Gleason, Colin & Durand, Michael. (2020). Remote Sensing of River Discharge: A Review and a Framing for the Discipline. Remote Sensing. 12. 1107. 10.3390/rs12071107.__

A comprehensive review of how remote sensing is applied in aid of hydrology.

# Global hydrologic model

## WaterGAP




# Fresh Water availability

__Rodell, M., Famiglietti, J.S., Wiese, D.N. et al. Emerging trends in global freshwater availability. Nature 557, 651–659 (2018). https://doi.org/10.1038/s41586-018-0123-1__

**HIGHLY RECOMMENDED**

In this article, authors addressed the global map of changes in fresh water availability with satellite observations and also climate models for projection. Very detailed global-regional analysis across the all continents. The impact of elevated precipitation, human-induced irrigation(mining), climate change, glacier depletion, and so on. 

# Calibration

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
