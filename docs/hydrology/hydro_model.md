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

__[A Comprehensive Assessment of Floodwater Depth Estimation Models in Semiarid Regions WRR](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2022WR032031)__

The authors compared three types of inundation models based on DEM: HAND, TVD, and FwDET. It shows HAND and TVD overestimate floodwater depth while FwDET underestimate, as compared to hydrodynamic model outputs.


__[Recent Advances and New Frontiers in Riverine and Coastal Flood Modeling Rev. Geophysics](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022RG000788)__

It discusses in detail the flood driving factors and recent advances in hydrologic / hydrodynamic model development.

<p align="center">
<img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/ae957884-23f6-4882-b62e-74ca026e5d3e/rog20329-fig-0001-m.jpg">
</p>


![Conceptual](https://agupubs.onlinelibrary.wiley.com/cms/asset/2e74592b-7bf5-43ae-9e48-436ab1308f7b/wrcr26287-fig-0002-m.jpg)


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

__[A Robust Strategy to Account for Data Sampling Variability in the Development of Hydrological Models WRR](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022WR033703)__

The authors argued that traditional approaches in hydrologic calibration and validation (based on one period) cannot generalize model performance because the data sampling variability is not accounted for.

In this paper, they proposed a new way to account for data sampling varibility in hydrologic model evaluation, taken the insight from stochastic gradient descent. As such, confidence is generated to address hydrologic evaluations.

# Model evaluation

__[When best is the enemy of good – critical evaluation of performance criteria in hydrological models (HESS)](https://hess.copernicus.org/preprints/hess-2022-380/hess-2022-380.pdf)__

The authors compared a comprehensive list of evaluation factors such as NSE, KGE, KGE', and other variants to showcase their deficiencies in some extent, particularly the counter-balancing errors. Depending on the overall perspective, authors urge careful selection of evaluation criterion for hydrological model calibration and validation.

__[Insights From Dayflow: A Historical Streamflow Reanalysis Dataset for the Conterminous United States WRR](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022WR032312)__

This study coupled VIC-RAPID from Lin et al. 2019, but assimilated USGS stream gauges into their modeling framework. They can obtain 50% gauges having KGE>0.5. They benchmarked on w/o data assimilation and see the improvement.

<p align="center">
  <img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/b360091c-4282-4aa1-8284-2d70640dfa0b/wrcr26432-fig-0007-m.jpg">
</p>

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

__[Probablistic Numerical Modelling of Compound Flooding Caused by Tropical Storm Matthew over a Data Scarce Coastal Environment](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028565)__

In this article, the authors attempt to quantify the uncertainties of flood mapping due to event rainfall, tide wave propagation, etc. They proposed a coupling framework combining a hydrologic model (HyMOD) and a 2D hydrodynamic model (LISFLOOD-FP) to generate a probablistic flood maps after taking 3000 simulations according to the uncertainties from different rainfall products, model parameterisation, and tide time series.

They concluded that rainfall and ocean wave are the most important contributors to coastal flooding, unsurprisingly.

__[Validation of a full hydrodynamic model for large‐scale hydrologic modelling in the Amazon](https://onlinelibrary.wiley.com/doi/full/10.1002/hyp.8425)__

In this paper, it introduces a lot of needs for developing a coupled model, specifically the deficiences in current hydrologic models. They can be characterized as two main points:

1. issues in river routing are significant in flat river systems like the Amazon and its tributaries, where the influence of sea tide can be up to 1000km upstream. and the subcritical and diffusive flow in Amazon flood wave illustrates the backwater effect which traditional hydrologic model cannot conquer;

2. Floodplain inundation modelling is not available in hydrologic models.

__[AutoRAPID: A Model for Prompt Streamflow Estimation and Flood Inundation Mapping over Regional to Continental Extents](https://onlinelibrary.wiley.com/doi/full/10.1111/1752-1688.12476)__

In this paper, the authors coupled RAPID hydrologic routing module with AutoRoute for hydrodynamic part. For efficiency, they simulated 9 consecutive years of Mississippi river basin within only 45 mins (24 processors and 3-hr time step).

__[Simulation of Hurricane Harvey flood event through coupled hydrologic‐hydraulic models: Challenges and next steps](https://onlinelibrary.wiley.com/doi/full/10.1111/jfr3.12716)__

In this paper, the authors bridge the hydrologic-hydraulic modeling by using VIC+RAPID (hydrologic) and Flood2D-GPU, applied in Harrious county during Hurricane Harvey.

They tested the sensitivity of modelling parameters including initial water depth, roughness, soil moisture, bathymetry, and reservious storage. They used gauged stage time series and HWM interpolated water depth to validate the model performance.

"For a large flood event such as Hurricane Harvey, the effect of the initial water depths is insignificant. The Manning's n values may increase the peak water depth by ~1%, the flood extents by 65km2, and the high danger zone by ~6%. On the contrary, the bathymetry correction factors may reduce the flood extent by ~1.4% and the high‐danger zone by ~4%. Reducing the reservoir storage capacity to 1% may increase the flood extent by ~4% and the high‐danger zone by ~17%."

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

__[Influence of mesh structure on 2D full shallow water equations and SCS Curve Number simulation of rainfall/runoff events](https://www.sciencedirect.com/science/article/pii/S0022169412002697)__

In this paper, the arthors compared different types of meshes with different resoltions, including square cells, structured cells, and unstructure cells w/ or w/o local refinement.

The first conclusion is that coarser resolution results in higher surface volume and larger lagged time.

Second, rectangular mesh tends to be less viscous than structured triangular meshes, which he explains triangular mesh is more directionality,

Third, the local refined meshes predict better surface volume, and it performs much better than most structured rectangular mesh and triangular mesh, and better than unstructured mesh.

At last, in terms of computational efficiency, local refined mesh achieves the best tradeoff of accurate results and least computational efforts.

__[SHUD](https://www.shud.xyz/_book/index.html)__

A fully coupled hydrologic model that resolves overland flow, groundwater flow in a unstructured mesh.

__[Enhancing river model set-up for 2-D dynamic flood modelling](https://www.sciencedirect.com/science/article/pii/S1364815215000304#bib7)__

This paper details necessary steps for a hydrodynamic model in the context of flood mapping. Several caveats are drawn, including representing realistic terrain, a coupling between hydrologic model and a hydrodynamic model, and insertion of man-made structures (bridges, buildings, weirs).

__[FWDET–Floodwater Depth Estimation Tool](https://doi.org/10.5194/nhess-2019-78)__

[Github](https://github.com/csdms-contrib/fwdet)

Use remote sensing sources (polygon) and high-resolution DEM to approximate Flood depth.

__[The Landlab v1.0 OverlandFlow component: a Python tool for computing shallow-water flow across watersheds](https://gmd.copernicus.org/articles/10/1645/2017/gmd-10-1645-2017.pdf)__

An efficient way for flood depth estimation, using simplified SWE. In particular, advection term is ignored, similar to LISFLOOD-FP. This model is hosted with Landlab python library.

__[Estimating river channel bathymetry in large scale flood inundation models](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2020WR028301)__

Traditionally, flood water in large scale hydrodynamic models is assumed to be uniform along channels, yet such assumption violates in a dynamic representation of flood wave propagation. In this work, the authors tested the gradually varied flow in river channels to observe the difference with uniform flow method. They claim that the difference can be tremendous when applied in large scale simulations.


## Cellular Automata for Fluid

__[Efficient Urban Inundation Model for Live Flood Forecasting with Cellular Automata and Motion Cost Fields](https://www.mdpi.com/2073-4441/12/7/1997/htm)__

The authors implemented Cellular Automata in an urban environment for efficiency. The governing PDE is:

$H_t=H_{t-1}+(\sum{D_{ij,t-1}}-\sum{D_{ij,t}}\frac{\deltat,b^2}+Source$

__[From python scripting to parallel spatial modeling](https://www.computer.org/csdl/pds/api/csdl/proceedings/download-article/12OmNBv2Cjf/pdf)__

A Python module for implementing cellular automata.

__[A Cellular Automata Fast Flood Evaluation (CA‐ffé) Model](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2018WR023679)__

First attempt to use Cellular Automata, published in WRR.

## DL in flood inundation modeling

__[Clustering-based hybrid inundation model for forecasting flood inundation depths](https://www.sciencedirect.com/science/article/pii/S002216941000106X)__

Early tentative approach to forecast flood inundation depth with ML models. They firstly cluster study domain to different regions that potentially differ in flood response. Then, ANN model is trained on 12-h maximum flood depth, simulated by HEC-RAS and SWMM.

__[Inundation Modeling in Data Scarce Regions](https://arxiv.org/pdf/1910.05006.pdf)__

Google's initiative towards global inundation mapping. They detailed the terrain data they used by reconstructing optical satellite images with 3D depth model, and the hydraulic models empowered by TPU over the globe.

__[Physics Informed Data Driven model for Flood Prediction: Application of Deep Learning in prediction of urban flood development](https://arxiv.org/pdf/1908.10312v1.pdf)__

In this article, the authors used deep learning method to replace SWE. Several DL models are intercompared: CNN, GAN, and GAN with data assimilation. The model is trained to ANUGA 2D FVM solver in a case study in Austin. The speedup is almost 5000 times, compared to ANUGA.

__[An ANN-based emulation modelling framework for flood inundation modelling: Application, challenges and future directions](https://www.sciencedirect.com/science/article/pii/S1364815219307601#bib89)__

In this paper, the authors discussed potentials using ML to emulate flood inundation. They propose ANN based model trained on TUFlow solved water depth (3 historical events and six designed events). A case study in Australia is provided. Inputs, such as flood drivers (i.e., inflow, tidal condition). They used information theory, partial mutual information (PMI) specifically to select most important input features.

One hilight of this work is that they discussed the prospecitve future of using ML model to replace SWE, and they validate the results based on three aspects:   

1. predictive validity: to ensure the model can generalise over the range of calibration data (that is validation step).

2. replicative validity: to ensure the model has captured the underlying relationship in the available data

3. structure validity: Structure validation is “to ensure the model is plausible when compared with a priori knowledge” of the system)

__[Artificial neural network based hybrid modeling approach for flood inundation modeling](https://www.sciencedirect.com/science/article/pii/S0022169420310660#!)__

The authors attempted to generalize ANN model from data-rich regions to data-sparse regions. A hybrid framework is developed, using point-based ANN, block-based ANN (in consecutive times). Point-based ANN turns out to have better generalization.

A framework of their workflow is provided as follows, in which they cluster regions with sufficient data or poor data coverage, and subsequently they construct relationships between data-rich model and data-sparse model.

<p aligh="center">
  <img src="https://ars.els-cdn.com/content/image/1-s2.0-S0022169420310660-gr1_lrg.jpg">
</p>

They classified the model domain into data-rich channel and data-sparse flood plain. Within the floodplains, they applied ANNs+ReLU to reclify values above max depth in channel.

<p align="center">
  <img src="https://ars.els-cdn.com/content/image/1-s2.0-S0022169420310660-gr4_lrg.jpg">
</p>

__[Improvement of Two-Dimensional Flow-Depth Prediction Based on Neural Network Models By Preprocessing Hydrological and Geomorphological Data](https://link.springer.com/article/10.1007/s11269-021-02776-9)__

In this paper, the authors used a set of hydrologic variables e.g., Runoff, roughness, FAR, slope with a latent time to predict flood depth at next time step. The models they used are RNNs, benchmarked on traditional ANNs. One highlight is that they did multi-dimensional cluster to seperate the watershed into different properties based on environmental variables.

__[U-FLOOD – Topographic deep learning for predicting urban pluvial flood water depth](https://www.sciencedirect.com/science/article/pii/S0022169421009483)__

This paper uses a topographic deep learning approach to predict the pluvial flood hazard in urban areas. The approach consists of a convolutional neural network that takes as input a set of spatial variables derived from high-resolution topographic data and rainfall. The results are comparable against Mike model.

__[A Framework for Modeling Flood Depth Using a Hybrid of Hydraulics and Machine Learning Sci. Rep.](https://www.nature.com/articles/s41598-020-65232-5)__

The authors use ANN and RF to emulate the behavior of a 2d hydrodynamic model FaSTMECH for a short river reach in Utah.

__[Rapid Spatio-Temporal Flood Modelling via Hydraulics-Based Graph Neural Networks](https://doi.org/10.5194/egusphere-2023-284)__

This article is first of its kind to predict flood inundation based on solving SWE with GNN that is analogy to FV scheme.
* The article introduces SWE-GNN, a hydraulics-inspired surrogate model based on Graph Neural Networks (GNN) that can be used for rapid spatio-temporal flood modelling.
* The model exploits the analogy between finite volume methods, used to solve the shallow water equations (SWE), and GNNs.
* The inputs are determined by the topographical properties of the domain and the initial hydraulic conditions.
* The GNN then determines how fluxes are exchanged between cells via a learned local function.
* The model predicts the spatio-temporal evolution of the flood for unseen topographies with a mean average error in time of 0.04 m for water depths and 0.004 m2/s for unit discharges.
* SWE-GNN has a computational speedup of up to two orders of magnitude faster than the numerical solver.
