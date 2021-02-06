---
layout: default
title: Flood-affecting factors
parent: Hydrology
nav_order: 4
---

# Terrain

__[The Need for a High-Accuracy, Open-Access Global DEM](https://www.frontiersin.org/articles/10.3389/feart.2018.00225/full)__

# Canopy interception

__[Canopy precipitation interception in urban forests in relation to stand structure](https://link.springer.com/article/10.1007/s11252-017-0689-7)__

In this paper, the authors split bulk precipitation into throughfall, stemfall, and canopy interception with gauged observations. They evaluated compositions of each during leafness and leafed period for three types of forests: mixed forest, riparian pine forest, and floodplain hardwood forest.

The composition is shown as below where in Leafed period and mixed forest, the interception could take up over 20% of the total precipitation.

<p align="center">
  <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs11252-017-0689-7/MediaObjects/11252_2017_689_Fig4_HTML.gif?as=webp">
</p>

__[Evaluation of canopy interception schemes in land surface models](https://www.sciencedirect.com/science/article/pii/S0022169407004866?via%3Dihub)__

Canopy interception is evaluated with Land surface models, in which the authors proposed a scheme that differentiates rain type (convective or straitiform).

They claimed that the global average interception loss is around 0.31 for 60-min resolution, concentrated on rain forests, but even higher for 20-min resolution. convective storm will have higher positive impact on interception loss.

# Soil/Infiltration

__[Estimating dominant runoff modes across the conterminous United States](https://onlinelibrary.wiley.com/doi/full/10.1002/hyp.13296)__

In this paper, the authors classified US into their dominant hydrologic processes: 1) infiltration-excess flow and 2) suturation-excess flow.

"Infiltration‐excess processes (hereafter referred to as IE) follow from precipitation intensities that exceed soil permeability, for example, in places with soils having high clay content, compaction, or impervious surfaces. Conversely, saturation‐excess runoff (hereafter referred to as SE) is more likely in regions where infiltration capacity exceeds precipitation, for example, in places which have humid, well‐vegetated, and low‐lying areas where surface and subsurface flows converge. For instance, where and when SE dominates, a topographic wetness index can effectively depict fine‐scale spatial moisture patterns by revealing variable runoff source areas with lower gradients and greater contributing areas"

"The intensity or likelihood of IE runoff, as indicated by the degree to which 1‐hr storm depths exceed representative surficial KSAT, is the greatest in portions of Texas, Louisiana, Kansas, Missouri, Iowa, Nebraska, and Western South Dakota. SE runoff, on the other hand, is more likely in Florida, Southern Georgia, Southeastern California, and Nevada, as well as western Oregon and coastal areas of the Great Lakes region"

A CONUS-wide Ksat exceedance is provided as follows:

<p align="center">
  <img src="https://onlinelibrary.wiley.com/cms/asset/ba0a915e-4dc8-4668-8423-6bc17bdbda35/hyp13296-fig-0004-m.jpg">
</p>

__[Understanding the re-infiltration process to simulating streamflow in North Central Texas using the WRF-hydro modeling system](https://www.sciencedirect.com/science/article/pii/S0022169420303620)__

In this paper, the authors comprehensively investigated the significance of run-on infiltration for WRF-Hydro. A few model parameters are cross-correlated with reinfiltration ratio (defined as reinfiltration / total infiltration).

# Urbanization
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

__[Beyond imperviousness: the role of antecedent wetness in runoff generation in urbanized catchments](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2020WR028060)__

In this article, the authors attempt to examine the interplay of imperviousness and antecedent soil moisture to runoff generation in the US with a large samples.

They considered a range of climate variables and land use variables and morphology variables and geopedology variables. Storm event separation is discussed in this methodology

__[Causal Effect of Impervious Cover on Annual Flood Magnitude for the United States](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019GL086480)__

In this work, authors adopts causual inference on flood magnitude changes due to the increase in imperviousness. They concluded that one percent increase in impervious basin cover causes a 3.3% increase in annual flood magnitude in the US.

They summarized main three approaches to study on this topic:

1) Case study focusing on temporal variations.  
2) paired catchment with contrast experiment variable.  
3) Model simulations.  

# Climate Change

__[Continental‑scale convection‑permitting modeling of the current and future climate of North America](https://link.springer.com/article/10.1007/s00382-016-3327-9)__

Physical downscaling of global climate model with convection-permitting feature, which can be used as input to investigate the impact of climate change on fine-scale hydrologic responses.

__[Changes in Future Flash Flood–Producing Storms in the United States](https://journals.ametsoc.org/jhm/article/21/10/2221/354228/Changes-in-Future-Flash-Flood-Producing-Storms-in)__

The authors adopted datasets from Dr. Liu for 13-year convective-permitting model and coupled with Noah-MP community model to investigate the flood (i.e., flash flood) response due to a warming climate. They compared CRTL and PWG precipitation against NCEP stage IV dataset using the SSMI index to investigate the structural similarity. But not much traditional quantification has been done. Without any doubts, climate change changes the frequency of flash flood and rainfall intensity. 7.5%/K increase in hourly max. rain rates is observed, but medium rain rates are on par with Clausius-Clapeyron theory.

__[Using machine learning models, remote sensing, and GIS to investigate the effects of changing climates and land uses on flood probability](https://www.sciencedirect.com/science/article/pii/S0022169420311240)__

In this article, the authors seek to investigate flood risks based on a host of environmental variables, including hydrometrological, topographic, and geological factors. Climate change is factored based on statistical downscaling from long series of gauge data for the change of precipitation, and ANN based methods take account the landuse changes. It is insightful to consider the varibles that could affect flood risks.

__[Comparing Flood Projection Approaches Across Hydro-Climatologically Diverse United States River Basins]()__

In this article, the authors pointed out three approaches to investigate the climate change impact on flooding. (1) Assuming stationarity, (2) hydrologic simulation under general circulation models, and (3) informed-parameter (e.g., time or trend analysis, climate indices, infrastructure development indices, land use indices.They also reviewed lots of literatures and found their limitations.

They specifically look at several questions: (1) how does out-of-sample bias compare between stationary assumption and other approaches, (2) can the direction of change at a gage be projected?, (3) can regional change be projected?, and (4) how much additional bias is introduced when GCM outputs are used to force the climate-based approaches.

In methodology, they first regionalize US basins with self-organising approach, and measured by sihouette width and physical meaning. Then they compared stationarity, climate-informed, precipitation-informed, and hydrologic simulation under the context of Bayesion inference. To conclude, they found precipitation and hydrologic simulation are statstically significant to reveal the flood projection. 

__[Global flood risk under climate change](https://www.nature.com/articles/nclimate1911)__

This paper published in Nature climate change is one of the highly reputed articles that studied flood intensity/frequency changes under a warming climate. It classifies major global river basins and finds a heterogenous feature for future flood response as below. They also simulated number of impacted and exposed people in a future scenario.

<p align="center">
<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fnclimate1911/MediaObjects/41558_2013_Article_BFnclimate1911_Fig1_HTML.jpg" width="100%">
</p>

<p align="center">
<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fnclimate1911/MediaObjects/41558_2013_Article_BFnclimate1911_Fig2_HTML.jpg" width="100%">
</p>

__[Future projections of flood dynamics in the Vietnamese Mekong Delta](https://www.sciencedirect.com/science/article/pii/S0048969720341188#bb0260)__

In this paper, the authors collectively evaluated the change of flood dynamics under the impact of climate change, hydropower regulation, sea-level rise, sustainable development, and floodplain restoration. They not only quantitatively assessed flood hazards (inundation extent, depth, and duration), but also focused on impacts, specifically on rice damages.

__[Characterizing Uncertainty of the Hydrologic Impacts of Climate Change](https://link.springer.com/article/10.1007%2Fs40641-016-0034-x)__

This paper, Clark et al. reviewed the uncertainties inherent to climate-driven hydrologic studies from different perspectives as shown in the figure below.

<p align="center">
  <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs40641-016-0034-x/MediaObjects/40641_2016_34_Fig1_HTML.gif?as=webp">
</p>

__[Going beyond the ensemble mean: assessment of future floods from global multi‐models](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2020WR027897)__

the authors discussed the advantages of using multi-model ensembles to replace "one-model-one-vote" approach.

"There is indeed a growing interest in the scientific community dealing with climate impact studies on the opportunity of going beyond the ‘one-model onevote approach’ (or “model democracy” (Knutti, 2010)) and favouring model runs with a better historical performance in reproducing observations with the aim to reduce uncertainty"

In peak flow distributions, the authors assessed the time series with three tests: 1) same distribution (KS test), 2) equal median (Wilcoxon rank-sum), and 3) equal variance (Ansari-Bradley).

Flood timing shifts are also investigated in this study, pointing to a general conclusion of earlier peaking time.

Interestingly, they found flood magnitude for all models indicates a genearl decrease in future over southeast U.S. These features are explained by two-fold: 1) uncertainties due to representation of precipitation and sub-grid soil infiltration; 2) total runoff contributions from saturation excess flow and infiltration excess flow.

"If on the one hand GCMs are responsible for regional runoff biases due to uncertainties in the representation of precipitation and sub-grid soil infiltration and flow; on the other hand the GIMs’ total runoff include contributions from surface runoff – function of saturation and infiltration excess – and subsurface runoff – function of impermeable area and water table depth"

"The prevalence of infiltration (IE) or saturation (SE) excess runoff depends on the type of soil and its capacity to become saturated / infiltrate. A sandy soil in the southeast will yield a higher flux (i.e., will transmit water faster) than a clayey soil under a given hydraulic gradient, reducing the effects of high-intensity precipitation."
