---
layout: default
title: Flood
parent: Hydrology
nav_order: 3
---

# Flood detection from remotely sensed products

<p align="center">
<img src="https://github.com/chrimerss/allenslib/blob/master/src/Flood%20detection.png?raw=true" width="100%">
</p>


__L. Landuyt, A. Van Wesemael, G. J. -. Schumann, R. Hostache, N. E. C. Verhoest and F. M. B. Van Coillie, "Flood Mapping Based on Synthetic Aperture Radar: An Assessment of Established Approaches," in IEEE Transactions on Geoscience and Remote Sensing, vol. 57, no. 2, pp. 722-739, Feb. 2019, doi: 10.1109/TGRS.2018.2860054.__

In this paper, the authors reviewed most commonly used techniques to derive flood extent from Sentinental missions and compared with real applications. They found the stable performance of active countour method in the flood monitoring.

__Chini, M.; Pelich, R.; Pulvirenti, L.; Pierdicca, N.; Hostache, R.; Matgen, P. Sentinel-1 InSAR Coherence to Detect Floodwater in Urban Areas: Houston and Hurricane Harvey as A Test Case. Remote Sens. 2019, 11, 107.__

In this paper, the authors proposed a way to map the flood extent with respect to bare soils and urban areas. For bare soil flooding, the adaptive thresholds are applied to mask flooded regions; for urban areas with building, multi-temporal images are acquired to compute the cross-correlation, Temporal Average Intensity, Temporal Average Coherence, and Local Incidence Angle.

They also showcased this methodology to Harvey events in 2017, demonstrated the ability to map the floodplains.

__[Near-real-time non-obstructed flood inundation mapping using synthetic aperture radar; Shen et al. 2018](https://www.sciencedirect.com/science/article/pii/S0034425718305169#!)__

![data processing streamlines](https://ars.els-cdn.com/content/image/1-s2.0-S0034425718305169-gr1_lrg.jpg)

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

## Urbanization
__Zhou, Z., J. A. Smith, L. Yang, M. L. Baeck, M. Chaney, M.-C. Ten Veldhuis, H. Deng, and S. Liu (2017), The complexities of urban flood response: Flood frequency analyses for the Charlotte metropolitan region, Water Resour. Res., 53, 7401–7425, doi:10.1002/2016WR019997.__

In this paper, the authors examined the urban flood characteristics in Charlotte metropolitan area. They addressed basin attributes, stationarity, flood agents, the attributes of antecedent rainfall (wettness) to urban floods, flood response time, runoff ratio to drainage area, correlation of basin-average rainfall to runoff, etc.

The methodlogies in flood analysis could be adopted and some of the conclusions could be cited as well.

__[The impact of urban development on hydrologic regime from catchment to basin scales](https://www.sciencedirect.com/science/article/pii/S0169204611002489#bib0175)__

In this paper, the authors evaluated the flood magnitude, frequency, travel times on which the urbanization would impact. They designed experiments determining the spatial variability of impervious areas. Before that, they cautiously divided total impervious area by effective or non-effective impervious area to discriminate the different response by fitting a statistical method.


"This analysis supports the suggestion that the impact of urbanization on flood magnitude decreases as flood recurrence intervals increases as was found by Hollis (1975)."

"watersheds with urban land use located close to the outlet tend to produce smaller peak flows than ones with urban land uses located far from the outlet for the same storm events."

"restricting infiltration rate does not have much impact on high flows during the snow melt season if urban area was located near the basin outlet"

"It demonstrates that antecedent soil moisture could play an important role in assessing the impact of urbanization on flood peaks"

__[by Smith et al. 2001]()__

The authors characterize the response time (V/P) by the flow volume (V) that is calculated as the integral of flows 1 day prior to the peak flow and 2 days after divided by the flow rate (P). 

They investigated the impact due to land cover properties interms of flood magnitude and flood response time; antecedent soil conditions play an important role; the spatial variability of rainfall affects the flood response; storm structure and motion also has marked impact.

# Ensemble Flood Forecasting

__[Pappenberger, F., J. Bartholmes, J. Thielen, H. L. Cloke, R. Buizza, and A. de Roo (2008), New dimensions in early flood warning across the globe using grand-ensemble weather predictions, Geophys. Res. Lett., 35, L10404, doi:10.1029/2008GL033837.](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2008GL033837)__

In this paper, the authors propose to use the grand ensemble to take place individual forecast members in order to capture the uncertainties. In their result, they claim that the grand ensemble indeed greatly reduces the miss of the event detections, even though the false alarm raises.

__[Schumann, G. J.-P., J. C. Neal, N. Voisin, K. M. Andreadis, F. Pappenberger, N. Phanthuwongpakdee, A. C. Hall, and P. D.
Bates (2013), A first large scale flood inundation forecasting model, Water Resour. Res., 49, 6248–6257, doi:10.1002/wrcr.20521.](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/wrcr.20521)__

In this paper, the authors coupled ECMWF ensemble forecast with VIC model and LISFLOOD-FP to simulate/forecast the flood inundation as a regional analysis. It demonstrates promising accuracy with reference to LandSat derived river stage, and interestringly, this framework is calibrated based on ICESat derived water stage.

__[When does spatial resolution become spurious in probabilistic flood inundation predictions?](https://onlinelibrary.wiley.com/doi/full/10.1002/hyp.10749)__

In this paper, the authors present inherent uncertainties for producing flood maps by comparing to deterministic approach. They also pointed out the circumstances when the model performance degrades the most under which resolution.

In terms of probabilistic flood map, they build up a probability distribution to consider the percentiles or probabilities when a grid cell is flooded or not. In addition, they proposed a error metrics to account for uncertainties, in which they decompose the hits into different percentiles.

__[Flood-plain mapping: a critical discussion of deterministic and probabilistic approaches](https://www.tandfonline.com/doi/full/10.1080/02626661003683389)__

In this paper, the authors discussed the importance to embrace a probabilistic approach, in which they considered the uncertainties coming from model parameters (manning's n) and perturbed upstream discharge. They used a more sophiscated model (full 2D finite element approach) to compared with ensemble predictions by a simpler model. In this comparison, they found the ensemble prediction could replace the sophisticated model.

They also discussed the limitations in terms of calibration process, in which they forced a SAR derived flood extent to gain the best-of-fitness value.

# Flood events validations

## Social media data

1. https://cordis.europa.eu/project/id/730082/results

2. https://www.globalfloodmonitor.org/

__Scotti, V, Giannini, M, Cioffi, F. Enhanced flood mapping using synthetic aperture radar (SAR) images, hydraulic modelling, and social media: A case study of Hurricane Harvey (Houston, TX). J Flood Risk Management. 2020;e12647. https://doi.org/10.1111/jfr3.12647__


# Flood impact-forecasting

__[Impact Forecasting to Support Emergency Management of Natural Hazards](https://agupubs.onlinelibrary.wiley.com/doi/pdfdirect/10.1029/2020RG000704)__

In this paper, the authors exhaustively examined a set of natural hazards forcasting, and projected the opportunities and challenges on harzard forecasting and impact forecasting. Of them, providing uncertainty estimation on not only hazard-forecasting, but impact-forecasting would be critical.

The majority of flood impact models focus on direct economic damage mostly to the residential and commercial sector, but also impact models for agriculture and the public sector are available (Gerl et al., 2016). Approaches to estimate, for instance, damage to critical infrastructure or indirect impacts barely exist (Merz et al., 2010, Koks, 2018, Bubeck et al.,2019)

Ensemble based impact forecasting is possible and will lead to probabilistic impact predictions that incorporate uncertainties (Brown et al., 2016, Cole et al., 2018, Dale et al., 2014).
