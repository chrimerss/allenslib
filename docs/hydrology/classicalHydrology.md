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

__[A web based tool for operational real-time flood forecasting using data assimilation to update hydraulic states](https://www.sciencedirect.com/science/article/pii/S1364815216301839)__

In this study, the authors coupled a semi-distributed hydrologic model which is suited fort karst areas along with a hydraulic model (linear lag-and-route model) for flood forecast. The main focus of this study is to update hydraulic states using openDA data assimilation tools.

__[The effect of coupling hydrologic and hydrodynamic models on probable maximum flood estimation](https://www.sciencedirect.com/science/article/pii/S002216941730272X?via%3Dihub#b0225)__

In this article, the author coupled hydrologic model and hydrodynamic model in a way that hydrologic model generated hydrograph is forced as boundary condition in the hydrodynamic model. Unlike other studies that compare the flood extent or depth to observations, they focused on the probable maximum flood. They simply compared coupled model with hydrologic model in 1D representations.

# Modeling Toolkits

__Multi-objective unstructured triangular mesh generation for use in hydrological and land surface models__

In this paper, the authors introduced a way to construct unstructured meshes based on topographic data and river channel bathymetry to reduce heterorgeneity, which is well-suited for hydrologic/hydrodynamic modeling.

__Flamig, Z. L., Vergara, H., and Gourley, J. J.: The Ensemble Framework For Flash Flood Forecasting (EF5) v1.2: Description and Case Study, Geosci. Model Dev. Discuss., https://doi.org/10.5194/gmd-2020-46, in review, 2020.__

An descriptive paper stating the latest EF5 model and its application to the CONUS.

__[Mesh type tradeoffs in 2D hydrodynamic modeling of flooding with a Godunov-based flow solver](https://www.sciencedirect.com/science/article/pii/S0309170814000360)__

"Unstructured mesh mandates greater overhead to track the neighborhood of data around each cell, and makes it more challenging to compute gradients in the solution because data points do not fall on a regular grid; but unstructured mesh is very appealing for the ease with which meshes can be generated and tailored to the unique geometry of application sites and the ability to locally refine the mesh around areas of interest"

"In areas of high topographic variability, a fine mesh may be required to resolve important flow paths and thus minimize input data errors. Similarly, a relatively fine mesh can be used to resolve sharp flow features such as a hydraulic jump and thus minimize numerical errors."

Computational cost for an explicit finite volume model scales in proportion to the number of cells and the number of time steps.

In this study, a real case dam-break example illustrates the benefits of unstructured grid compared to quadrilateral mesh, that relative coarse grid and medium grid resolution, i.e., 1km, 100m to 10m, the unstructured perform better in terms of the computational efficiency. But ultra-high resolution, the structured is better

__[SHUD](https://www.shud.xyz/_book/index.html)__

A fully coupled hydrologic model that resolves overland flow, groundwater flow in a unstructured mesh.

# Sensitivity Analysis

__[Sensitivity analysis of environmental models: A systematic review with practical workflow](https://www.sciencedirect.com/science/article/pii/S1364815216300287#bib35)__

In this paper, authors comprehensively reviewed approaches to evaluate the sensitivity issue in environmental modeling, spaning from mapping, rakning, screening purposes and local/global sensitivity. A suit of methodologies such as pertubations, density, correlations are exclusively mentioned.

At the end, they proposed a workflow to dissect the sensitivity from inputs sampling to output post-analysis. 

__[Estimating a-priori kinematic wave model parameters based on regionalization for flash flood forecasting in the Conterminous United States](https://www.sciencedirect.com/science/article/pii/S0022169416303626)__

In this paper, the authors described a way to approximate the simplified 1D-Saint-Venant routing (aka. kinematic wave model) parameters by using historical USGS stream gauge data that links flow rate and depth (i.e., routing curve) and hydroclimatologic data (i.e., precipitation, soil moisture), and terrain (DEM).

This approach has been applied in the CONUS in the rencent 10 years with event-based studies. A satisfactory result has been produced by measuring the flood timing error and flood peak error.

__[MGB-IPH model for hydrological and hydraulic simulation of large floodplain river systems coupled with open source GIS](https://www.sciencedirect.com/science/article/pii/S136481521630189X#bib51)__

[Hodges (2013)](https://www.sciencedirect.com/science/article/pii/S1364815213001898?via%3Dihub) suggested simplified routing methods should be increasingly substituted by hydrodynamic methods in large-scale hydrological models.

river routing and inundation dynamics are processes that, normally, are represented by relatively simple approaches. A recent review of twelve large-scale hydrological models (Kauffeldt et al., 2016) concluded that most of them use kinematic wave or even simpler methods for river flow routing. Huang et al. (2016) tested nine hydrological models in large-scale river basins, four of them not included in the review by Kauffeldt et al. (2016), and all of them have simplified methods for river routing.

In steep terrain regions, adopting simplified river routing methods is not often a problem, but in low relief terrains the results of the hydrological models can be strongly affected if river routing is not adequately represented, for instance, due to floodplain storage and backwater effects (Getirana and Paiva, 2013).

In some cases, there is a need for coupling the land surface scheme with the flow routing and flooding model, because of the loss of volume by infiltration and evapotranspiration in large areas, as reported by Pedinotti et al. (2012) in the Niger river basin, by Paz et al. (2014) in the Pantanal wetlands (South America) and by Bauer et al. (2006) in the Okavango Delta.

In this paper, the authors coupled a semi-distributed hydrologic model with a psedo-2D hydraulic routing scheme. They claimed that, compared to linear reservoir and kinematic wave which are the most common ways, this routing is advanced in simulating non-dendritic catchment and flat areas. And they relates the water level with area to approximate the flooded area.

# Hydrologic Regionalization

__[Investigating regionalization techniques for large-scale hydrological modelling](https://www.sciencedirect.com/science/article/pii/S0022169419300496)__

In this paper, the authors presented unsupervised clustering and supervised clustering for hydrologic regionalization.

# Process-based hydrologic modelling

__Ivanov, V.Y., E.R. Vivoni, R.L. Bras, and D. Entekhabi (2004), Preserving high-resolution surface and rainfall data in operational-scale basin hydrology: a fully-distributed physically-based approach, J. Hydrol., 298, 80-111, doi: 10.1016/j.hrol.2004.03.041__

In this paper, the authors exhaustively described the way to design a process-based modeling framework, and the design of meshes to preserve the variability of topographic inputs. They tested this operational model in three basins in Oklahoma, not only surface flow (discharge) is their concern, but other fluxes and states are included completely to introduce this model.


# CREST family

<img src="../../src/CREST_family_development.png">

## CREST 1.0

__Jiahu Wang, Yang Hong, Li Li, Jonathan J. Gourley, Sadiq I. Khan, Koray K. Yilmaz, Robert F. Adler, Frederick S. Policelli, Shahid Habib, Daniel Irwn, Ashutosh S. Limaye, Tesfaye Korme & Lawrence Okello (2011) The coupled routing and excess storage (CREST) distributed hydrological model, Hydrological Sciences Journal, 56:1, 84-98, DOI: 10.1080/02626667.2010.543087__

This paper detailed physical-based process (including water balance model components, sub-grid/downstream routing process). 

The first paper introduced CRESTH model v1.0

## CREST V1.6

__Wu, H., R. F. Adler, Y. Hong, Y. Tian, and F. Policelli, 2012: Evaluation of Global Flood Detection Using Satellite-Based Rainfall and a Hydrologic Model. J. Hydrometeor., 13, 1268–1284, https://doi.org/10.1175/JHM-D-11-087.1.__

CREST V1.6 applied to global flood detection

__S. I. Khan et al., "Satellite Remote Sensing and Hydrologic Modeling for Flood Inundation Mapping in Lake Victoria Basin: Implications for Hydrologic Prediction in Ungauged Basins," in IEEE Transactions on Geoscience and Remote Sensing, vol. 49, no. 1, pp. 85-95, Jan. 2011, doi: 10.1109/TGRS.2010.2057513.__

Regional flood detection with multiple events.

## CREST V2.0

__[Statistical and hydrological evaluation of TRMM-based Multi-satellite Precipitation Analysis over the Wangchu Basin of Bhutan: Are the latest satellite precipitation products 3B42V7 ready for use in ungauged basins?](https://www.sciencedirect.com/science/article/pii/S0022169413004952#b0160)__

(1) enhancement of the computation capability using parallel distribution techniques to make the model more efficient than the previous version (Wang et al., 2011); (2) model implementation with options of either spatially uniform, semi-distributed, or distributed parameter values; (3) automatic extraction of a-priori model parameter estimates from high-resolution land cover and soil texture data. The physically-based parameters, Ksat and WM, can be derived from land cover types and soil texture data based on a look-up table (Chow et al., 1988); (4) a modular design framework to accommodate research, development and system enhancements; and (5) inclusion of the optimization scheme SCE-UA (Duan et al., 1992, Duan et al., 1993) to enable automatic calibration of the CREST model parameters.

EF5-based CREST is originated here

## CREST V2.1

__[Refining a Distributed Linear Reservoir Routing Method to Improve Performance of the CREST Model](https://ascelibrary.org/doi/10.1061/%28ASCE%29HE.1943-5584.0001442)__

Introduction:

The previous version of the CREST, using linear reservior routing, untruly produces discontinuous runoff, which tends to underestimate channel flow at the outlet point. Therefore, a fully distributed linear reservior routing model is proposed.

By definition, the fully integrated LRR means runoff produced at each trajectory cell is taken into account, instead of directly produced at desired point.

Three case studies are designed to verify the performance gain of the new routing scheme.

### CREST-SVAS

__[A framework to improve hyper-resolution hydrological simulation in snow-affected regions](https://www.sciencedirect.com/science/article/pii/S0022169417303414?via%3Dihub#b0170)__

Introduction:

The land surface model exhibits great uncertainty, especially the snow models, which in turn propagates errors into flow simulations.

In this paper, the authors extended the CREST model with a soil-vegetation-atmosphere layer (vegetation interception, snow accumulation, melting, and refreezing)

Improvements:

1. Three snow layers are added in addition to the CREST, to represent the snow melting, refreezing process.

2. Two ablation schemes (with or without canopy) were implemented.

3. A energy balance is included (only if snow is present)

## CREST V3.0

__Kan, G.; Tang, G.; Yang, Y.; Hong, Y.; Li, J.; Ding, L.; He, X.; Liang, K.; He, L.; Li, Z.; Hu, Y.; Cui, Y. An Improved Coupled Routing and Excess Storage (CREST) Distributed Hydrological Model and Its Verification in Ganjiang River Basin, China. Water 2017, 9, 904.__

The improvements of CREST V3.0 against V2.x are:

1). Separating the soil layer into three layers and considering tension water, soil moisture, and evapotranspiration computations like in the original version.

2). Adding a free water storage computation module with a free water distribution curve to describe the sub-grid variations of free water storage.

3). According to free water storage, separating runoff into three components, including overland flow, interflow, and ground water.

4). Improving the flow concentration module into a four-mechanism cell-to-cell routing, including overland flow, interflow, ground water, and river channel flow routings. Based on the arrival time of each upstream grid cell to its downstream outlet grid cell, the generated runoff is routed down along the flow concentration path generated according to the eight-flow-direction method.
