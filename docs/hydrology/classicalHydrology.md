---
layout: default
title: Classical hydrology
parent: Hydrology
nav_order: 2
---

# Rainfall-runoff coefficient

**Miao, C., Zheng, H., Jiao, J., Feng, X., Duan, Q., & Mpofu, E. (2020).
The changing relationship between rainfall and surface runoff on the Loess Plateau, China. Journal of Geophysical Research:
Atmospheres, 125, e2019JD032053. https://doi.org/10.1029/2019JD032053**

In this article, authors examined the rainfall-runoff generation, particularly the coefficient changes over two periods: 1971-1987,
and 2008-2016; This is a decent article to look or review possible attributes of the changing runoff in this specific region (i.e.,
human activity, vegetation, climatology etc.)

One adoptable methodology in this study is to determine the critical point for thresholding runoff throughout Pettitt test.

Main findings:
1. The runoff coefficient decreased greatly in Loess Plateau;
2. The precipitation threshold became greater on the middle regions of the plateau during P2.

# Conceptual planetary hydrology

__Gleeson, T., Wang‐Erlandsson, L., Porkka, M., Zipper, S. C., Jaramillo, F., Gerten, D., et al ( 2020). Illuminating water cycle modifications and Earth system resilience in the Anthropocene. Water Resources Research, 56, e2019WR024957. https://doi.org/10.1029/2019WR024957__

In this big paper, the authors proposed a framework to address the scientific problems: How to determine the tipping point of changes resulting in a irreversiable situation; in other words, what is the maximum changes that breaks the earth system resilience.

Even though this is a conceptual paper, it really motivates researchers to dive into and look for answers to benefit our human society.

# Coupled hydrologic/hydraulic modeling for flood innudation

__A high resolution coupled hydrologic–hydraulic model (HiResFlood-UCI) for flash flood modeling__

UCI group developed the coupling framework of SAC-based hydrologic model and BreZo-based hydraulic model. The advantage of coupling these two can improve the streamflow prediction, and also provide the flood depth and velocity which is crucial to categorize the flood.

__Montanari, M., Hostache, R., Matgen, P., Schumann, G., Pfister, L., & Hoffmann, L. (2009). Calibration and sequential updating of a coupled hydrologic-hydraulic model using remote sensing-derived water stages. Hydrology and Earth System Sciences, 13(3), 367-380.__

In this paper, the authors coupled a parsimonious hydrologic model (3 parameters) with a 1-D hydrodynamic model. The focus of this study is to envision the calibrating schemes by (1) all-in-one calibration and (2) sequential calibration. Not only stream gauge data are used for calibration, the SAR derived extent as well in order to perceive the accuracy of generating flood inundation maps.

__[Flood inundation modelling: A review of methods, recent advances and uncertainty analysis](https://www.sciencedirect.com/science/article/pii/S1364815216310040#!)__

The authors reviewed the development of inundation-driven models based on either emperical/physical. They explicated from modeling domains (1D/2D/3D), different numerical solvers, levels of realisations.

They also sheded lights on the future applications, first, the integration of remotely sensed imageries with physical models throughout data assimilations, the desire for high-performance computations, model uncertainty analysis will continue to play a significant role. 

# Modeling Toolkits

__Multi-objective unstructured triangular mesh generation for use in hydrological and land surface models__

In this paper, the authors introduced a way to construct unstructured meshes based on topographic data and river channel bathymetry to reduce heterorgeneity, which is well-suited for hydrologic/hydrodynamic modeling.

__How to cite: Flamig, Z. L., Vergara, H., and Gourley, J. J.: The Ensemble Framework For Flash Flood Forecasting (EF5) v1.2: Description and Case Study, Geosci. Model Dev. Discuss., https://doi.org/10.5194/gmd-2020-46, in review, 2020.__

An descriptive paper stating the latest EF5 model and its application to the CONUS.

# Sensitivity Analysis

__[Sensitivity analysis of environmental models: A systematic review with practical workflow](https://www.sciencedirect.com/science/article/pii/S1364815216300287#bib35)__

In this paper, authors comprehensively reviewed approaches to evaluate the sensitivity issue in environmental modeling, spaning from mapping, rakning, screening purposes and local/global sensitivity. A suit of methodologies such as pertubations, density, correlations are exclusively mentioned.

At the end, they proposed a workflow to dissect the sensitivity from inputs sampling to output post-analysis. 

__[Estimating a-priori kinematic wave model parameters based on regionalization for flash flood forecasting in the Conterminous United States](https://www.sciencedirect.com/science/article/pii/S0022169416303626)__

In this paper, the authors described a way to approximate the simplified 1D-Saint-Venant routing (aka. kinematic wave model) parameters by using historical USGS stream gauge data that links flow rate and depth (i.e., routing curve) and hydroclimatologic data (i.e., precipitation, soil moisture), and terrain (DEM).

This approach has been applied in the CONUS in the rencent 10 years with event-based studies. A satisfactory result has been produced by measuring the flood timing error and flood peak error.
