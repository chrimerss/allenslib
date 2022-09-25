---
layout: default
title: Flood Validation, Uncertainty, and Impact
parent: Hydrology
nav_order: 6
---

# Ensemble Flood Forecasting

__[New dimensions in early flood warning across the globe using grand-ensemble weather predictions](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2008GL033837)__

In this paper, the authors propose to use the grand ensemble to take place individual forecast members in order to capture the uncertainties. In their result, they claim that the grand ensemble indeed greatly reduces the miss of the event detections, even though the false alarm raises.

__[A first large scale flood inundation forecasting model, Water Resour. Res., 49, 6248–6257, doi:10.1002/wrcr.20521.](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/wrcr.20521)__

In this paper, the authors coupled ECMWF ensemble forecast with VIC model and LISFLOOD-FP to simulate/forecast the flood inundation as a regional analysis. It demonstrates promising accuracy with reference to LandSat derived river stage, and interestringly, this framework is calibrated based on ICESat derived water stage.

__[When does spatial resolution become spurious in probabilistic flood inundation predictions?](https://onlinelibrary.wiley.com/doi/full/10.1002/hyp.10749)__

In this paper, the authors present inherent uncertainties for producing flood maps by comparing to deterministic approach. They also pointed out the circumstances when the model performance degrades the most under which resolution.

In terms of probabilistic flood map, they build up a probability distribution to consider the percentiles or probabilities when a grid cell is flooded or not. In addition, they proposed a error metrics to account for uncertainties, in which they decompose the hits into different percentiles.

__[Flood-plain mapping: a critical discussion of deterministic and probabilistic approaches](https://www.tandfonline.com/doi/full/10.1080/02626661003683389)__

In this paper, the authors discussed the importance to embrace a probabilistic approach, in which they considered the uncertainties coming from model parameters (manning's n) and perturbed upstream discharge. They used a more sophiscated model (full 2D finite element approach) to compared with ensemble predictions by a simpler model. In this comparison, they found the ensemble prediction could replace the sophisticated model.

They also discussed the limitations in terms of calibration process, in which they forced a SAR derived flood extent to gain the best-of-fitness value.

__[A methodology for the validation of uncertain flood inundation models](https://www.sciencedirect.com/science/article/pii/S0022169405005615#bib12)__

In this paper, the authors proposed two ways of evaluating probabilistic flood maps: precision (with information theory; entropy) and accuracy (with number of hits). It is a balance to precision and accuracy when considering how many simulations to retain.

They applied this methorology to LISFLOOD-FP model, at odds with two SAR derived flood map.

__[A Path Towards Short-Term Probabilistic Flash Flood Prediction BAMS](https://journals.ametsoc.org/view/journals/bams/aop/BAMS-D-22-0026.1/BAMS-D-22-0026.1.xml?tab_body=pdf)__

The authors started claiming that annual flash flood warnings issued by NWS average 4287. The improvement of accuracy according to the contigency table has been slow since 1997, with POD around 0.85-0.89, FAR around 0.5. So to say, false alarms regarding flash flooding is present and calling immediate attention. The authors propose a probabilistic prototype PRO-FLASH for flash flood warning underlying the FACET umbrella.

They envisioned two approches: (1) probability-related binary warning (flash flooding or no flash flooding) and (2) probability-related category warning (minor, moderate, major risks).

# Flood events validations

__[Detailed data is welcome, but with a pinch of salt: Accuracy, precision, and uncertainty in flood inundation modeling](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/wrcr.20406)__

1. Accuracy and Precision: "more information" in hydraulic modelling relating to higher model performance is misleading (reductionist). There are model accuracy and precision to distinguish. accuracy refers to model ability to correctly reproduce variables of interest, but precision relates to resolution of computational grid, where each variable is computed. There two only partially overlap.

2. Data Uncertainty. Topographic data; boundary conditions; urban drainage; interaction with small-scale features (ditches, embankments, etc.); Buildings, transportations; 

3. The Problem of Model Evaluation. No consensus on the reliability and accuracy criteria. Pros and Cons of different reference data are discussed.

4. Do we really need 1m res. in flood mapping? "Indeed, this loss of modeling detail can be advisable, as in our opinion the use of too high resolution outputs can generate a false confidence on obtained results."

5. Keep it as simple as possible: the use of high-res. data in flood models. building-gole method to represent buildings.

__[Remote sensing and flood inundation modelling](https://onlinelibrary.wiley.com/doi/pdf/10.1002/hyp.5649)__

The author deems that model validation relied on bulk flow data that represented the aggregate response of the catchment to that point. However, for any given model and discretization, many different spatial patterns of grid-square effective parameter values can lead to the same aggregate response, but give different spatial predictions and thus process inferences. Lack of distributed validation data is a significant cause of equifinality and leads to tolerance of the physically unrealistic spatial lumping of parameter values and processes.

They appraised satellite SAR (res. 12.5 m ) and airborne SAR (res. 0.5 m) in predicting flood extent, and involved in calibration and validation process.

__[Utility of different data types for calibrating flood inundation models within a GLUE framework](https://hess.copernicus.org/articles/9/412/2005/)__

The authors assessed different means of calibrating the hydrodynamic model with respect to all available data (flood marks, aerial photography, and SAR flood extent). They calibrated based on time-varing stage and discharge; flood extent; maximum flood depth.

Given the relatively short interval between stations and the inherent uncertainties of stage-discharge relationships at each station, water levels recorded internal to the model domain are likely to prove a more valuable asset than discharges in conditioning model performance, particularly in the detection of erroneous compensating errors.

By using time-varing stage or discharge, only parameters in the upstream of gauges are sensitive, while downstream parameters are insensitive.

SAR extent is relatively insensitive to changes in parameters, and potentially there will be only a small reduction in parameter uncertainty from calibrating with these data and objective functions. But it is reconcilable with response fro the air photo data.

To conclude, stage data help to reduce uncertainty over effective parameter specification; air photo data has similar properties as it provides aneffective surrogate measure of water surface elevation; discharge data is less effective because of the essentially mass conservative nature of the model and the flow dynamics of this particular event.

## Flood extent map

### Crowdsourcing data

1. https://cordis.europa.eu/project/id/730082/results

2. https://www.globalfloodmonitor.org/

__[A novel approach to leveraging social media for rapid flood mapping: a case study of the 2015 South Carolina floods](https://www.tandfonline.com/doi/full/10.1080/15230406.2016.1271356)__

<p align="center">
<img src="https://github.com/chrimerss/allenslib/blob/master/src/comp_remote_crowd.png" width="100%">
</p>

In this paper, the authors proposed a kernel-based method to delineat flood extent based on Twitter activity and USGS stream gauges.

__Scotti, V, Giannini, M, Cioffi, F. Enhanced flood mapping using synthetic aperture radar (SAR) images, hydraulic modelling, and social media: A case study of Hurricane Harvey (Houston, TX). J Flood Risk Management. 2020;e12647. https://doi.org/10.1111/jfr3.12647__

In this paper, authors reviewed advantages or deficiencies of current available ways of obtaining flood extent (SAR, model, and social media marks).

Social media marks:

They are also useful for post event, rapid flooding mapping, as they can provide timely localised information about water depth of inundated areas and damages (Fohringer et al., 2015). However, errors affect the quantitative assessment of flooding by social markers. These can be due to differences between the place where the photo is taken and the location of the tweet posted online, as well as, an incorrect photo‐interpretations of the photo perspective. Such errors could be reduced by combining high resolution DEM and social markers (Mandlburger, Hauer, Höfle, Habersack, & Pfeifer, 2009). A generalised use of social markers makes it necessary to filter a huge amount of information from social media. Recently, several approaches have been pursued. These include: (a) filtering by keywords or by geographic queries (Rogstadius, Kostakos, & Laredo, 2011 or Joseph et al., 2014), (b) filtering by crowdsourcing (Howe, 2006), (c) automatic filtering utilising machine learning and natural language processing (Sakaki, Okazaki, & Matsuo, 2010); Yin, Lampert, Cameron, Robinson, & Power, 2012) and (d) interactive visual spatiotemporal analysis/geovisual analytics (MacEachren et al., 2011); Morstatter, Kumar, Liu, & Maciejewski, 2013). None of such approaches is completely satisfying, and often a rather empirical post‐processing phase which involves a subjective judgement of the operator is required.

__[The importance of volunteered geographic information for the validation of flood inundation models](https://www.sciencedirect.com/science/article/pii/S0022169418303299#b0340)__

In this paper, the authors proposed a way to validate LISFLOOD-LP model based on crowdsourcing data, focused on three aspects: impact (flood extent), flowpath (velocity), and timeline.

__[Hyper-resolution monitoring of urban flooding with social media and crowdsourcing data](https://www.sciencedirect.com/science/article/pii/S009830041730609X#!)__

The use of Twitter and MyCoast App, with Natural Language Processing and Computer Vision to construct urban flooding

### Aerial photography

__[Probabilistic Flood Mapping Using Synthetic Aperture Radar Data](https://ieeexplore.ieee.org/abstract/document/7548327/authors)__

They constructed a reliability diagram to evaluate the SAR derived flood extent against aerial photographs to test the proposed probabilistic flood map.

### Wracks and Water marks

__[Reducing Inconsistencies in Point Observations of Maximum Flood Inundation Level](https://journals.ametsoc.org/ei/article/17/6/1/500/Reducing-Inconsistencies-in-Point-Observations-of)__

In this paper, the authors detailed uncertainties coming from flood marks. These water marks often use as supplementary data to more conventional flood extent data. 

Wracks underestimate peak flood depth as compared to water marks by 0.51 m.

They proposed a algorithm to smooth the uncertainty of all water marks.

__[Distributed whole city water level measurements from the Carlisle 2005 urban flood event and comparison with hydraulic model simulations](https://www.sciencedirect.com/science/article/pii/S002216940900047X#bib20)__

In this paper, the authors discussed the uncertainties from flood marks, they indicate flood marks bear more uncertainties than modelling results. 

Advantage: 

they can be collected post event, negating the need to pre-empt the flood or have equipment on-site during the flood itself. 

Disadvantage:

However, unlike gauge time-series and multi-temporal imagery (see [Bates et al., 2006](https://www.sciencedirect.com/science/article/pii/S0022169406000047) for a non-urban example) these data cannot be used to validate inundation dynamics because they do not convey temporal information. Furthermore, water and wrack marks are deposited at both peak levels and as the water line recedes, meaning that although it is potentially possible to measure elevation to <1 cm, deciding which elevation to survey can be more problematic. Moreover, water levels will be underestimated if no identifiable mark was produced at the maximum level. The magnitude of this bias is typically unknown and likely to vary from event to event depending on: (1) how conducive the conditions at peak level were to wrack and water mark deposition; and (2) the skill of the surveyor.

# Flood impact-forecasting

__[Impact Forecasting to Support Emergency Management of Natural Hazards](https://agupubs.onlinelibrary.wiley.com/doi/pdfdirect/10.1029/2020RG000704)__

In this paper, the authors exhaustively examined a set of natural hazards forcasting, and projected the opportunities and challenges on harzard forecasting and impact forecasting. Of them, providing uncertainty estimation on not only hazard-forecasting, but impact-forecasting would be critical.

The majority of flood impact models focus on direct economic damage mostly to the residential and commercial sector, but also impact models for agriculture and the public sector are available (Gerl et al., 2016). Approaches to estimate, for instance, damage to critical infrastructure or indirect impacts barely exist (Merz et al., 2010, Koks, 2018, Bubeck et al.,2019)

Ensemble based impact forecasting is possible and will lead to probabilistic impact predictions that incorporate uncertainties (Brown et al., 2016, Cole et al., 2018, Dale et al., 2014).

__[Leveraging machine learning for predicting flash flood damage in the Southeast US](https://iopscience.iop.org/article/10.1088/1748-9326/ab6edd)__
<p align="center">
<img src="https://cfn-live-content-bucket-iop-org.s3.amazonaws.com/journals/1748-9326/15/2/024011/2/erlab6eddf1_hr.jpg?AWSAccessKeyId=AKIAYDKQL6LTV7YY2HIK&Expires=1612539253&Signature=MXNSBIabN7Mrkj71QELL62I126A%3D">
</p>

[List of publications using ML to predict flood risks](https://cfn-live-content-bucket-iop-org.s3.amazonaws.com/journals/1748-9326/15/2/024011/2/ERL_15_2_024011_suppdata.pdf?AWSAccessKeyId=AKIAYDKQL6LTV7YY2HIK&Expires=1612538885&Signature=KTVxXl2J%2FXVLzEdA5HeauUEHD7k%3D)

# Flood hazard, vulnerability, risk, and resilience

__[Review article “Assessment of economic flood damage”](https://gfzpublic.gfz-potsdam.de/rest/items/item_241074_1/component/file_241073/content)__

In this paper, the authors reviewed a set of literatures that concern the flood damages in varying angles.

__[Flood resilience: a systematic review, Journal of Environmental Planning and Management](https://www.tandfonline.com/doi/full/10.1080/09640568.2019.1641474)__

Kerri McClymont, David Morrison, Lindsay Beevers & Esther Carmen (2020) Flood resilience: a systematic review, Journal of Environmental Planning and Management, 63:7, 1151-1176, DOI: 10.1080/09640568.2019.1641474
