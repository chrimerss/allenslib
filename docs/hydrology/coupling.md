---
layout: default
title: Wearher, Hydrology coupling
parent: Hydrology
nav_order: 8
---

# Weather/Climate - Hydrologic model coupling

__[A review of fully coupled atmosphere-hydrology simulations](https://link.springer.com/article/10.1007/s11442-019-1610-5)__

in this paper, the authors analyzed publications regarding atmosperic model and hydrologic model interaction to reflect the challenges as well as opportunities for present-day model coupling strategies. They mentioned some points:

1. Two-way coupling processes
2. Scale dependence
3. improvement of model parameters and uncertainties
4. parameter transfer and regionalization
5. hyper-resolution simulation.

# Land-Atmosphere coupling

## Soil moisture and atmosphere feedback

### Positive feedback

__[Marshall Shepherd - Brown Ocean](https://scholar.google.com.sg/citations?view_op=list_works&hl=en&hl=en&user=0tsoNUYAAAAJ&sortby=pubdate&citft=1&email_for_op=chrimerss%40gmail.com)__

__[A soil moisture–rainfall feedback mechanism 1. Theory and observations](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/97WR03499)__

A theoritical examination or explaination of how soil moisture impact rainfall, one of the pioneering work to address such.

<img width="422" alt="image" src="https://user-images.githubusercontent.com/31950869/162550250-e98f599c-b5c6-461f-914e-0ec3badfc9ac.png">

__[The role of anomalous soil moisture on the inland reintensification of Tropical Storm Erin (2007)](https://link.springer.com/article/10.1007/s11069-011-9966-6)__

<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs11069-011-9966-6/MediaObjects/11069_2011_9966_Fig9_HTML.gif?as=webp">

__[Sensitivity in the Overland Reintensification of Tropical Cyclone Erin (2007) to Near-Surface Soil Moisture Characteristics](https://journals.ametsoc.org/view/journals/mwre/139/12/2011mwr3593.1.xml)__

__[Impacts of Soil Moisture on the Numerical Simulation of a Post-Landfall Storm](https://link.springer.com/article/10.1007%2Fs13351-019-8002-8)__

The authors suggested the increased soil moisture with SLAB scheme before storm’s landfall tends to produce a weaker storm after landfall and has negative impacts on storm track simulation, because wetter soils tend to cool down ambient environment and thus resulting in a less conducive condition for storm maintanance.

__[Enhancement of inland penetration of monsoon depressions in the Bay of Bengal due to prestorm ground wetness](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/wrcr.20301)__

SOM analysis showed that dry states are more likely to occur during monsoon season compared to wet states; however, the probability of genesis of MLPS during a wet-state day is about four times higher compared to a dry state day. These maps showed that in general, the mean inland penetration of wet-state MDs is longer than the MDs that form during dry state.

__[Possible relation between land surface feedback and the post-landfall structure of monsoon depressions GRL](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2009GL037781)__

warmer, wetter (cooler, drier) land surface can intensify (weaken) the landfalling MDs over the Indian monsoon region

__[Land surface-precipitation feedback analysis for a landfalling monsoon depression in the Indian region JAMES](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016MS000829)__

Detailed analysis of land-atmosphere interaction through water budget equation and formulation of recycling ratio.


__[The Inland Maintenance and Reintensification of Tropical Storm Bill (2015). Part I: Contributions of the Brown Ocean Effect](https://journals.ametsoc.org/view/journals/hydr/22/10/JHM-D-20-0150.1.xml#bib1)__

They used reanalysis data to investigate the TCMI and non-TCMI storms associated with 2-week antecedent environments. It was found that TCMI storms present greater latent heat than non-TCMI storms. The ET 24-hour to storm trajectory is also much greater for TCMI.

__[A global spatiotemporal analysis of inland tropical cyclone maintenance or intensification](https://rmets.onlinelibrary.wiley.com/doi/10.1002/joc.3693)__

They classified historical TCs from 1979-2008 into warm-core TC, cold-core TC, and hybrid, and used MERRA to analyze meteorological variables. They found the 850 hPa temperature gradient to be significantly associated with TCMI, provided by latent heat fluxes.

__[Quantifying Surface Energy Fluxes in the Vicinity of Inland-Tracking Tropical Cyclones](https://journals.ametsoc.org/view/journals/apme/52/12/jamc-d-13-035.1.xml)__

They identified 4 storms globally and use a 1D soil model to resolve water transport with GLDAS as input forcing. They found the soil texture has large impact on heat release and thus the magnitude of re-intensification.

<p align="center">
  <img src="https://journals.ametsoc.org/view/journals/apme/52/12/full-jamc-d-13-035.1-f1.jpg">
</p>

__[PhD thesis Brown Ocean effect](https://getd.libs.uga.edu/pdfs/andersen_theresa_k_201308_phd.pdf)__

Landfalling TCs are more likely to intensify over regions with above average rainfall antecedent to the warmest months of the hurricane season, which allows soils to be sufficiently warm and moist to transfer energy back to the storm.

__[Influence of Land Cover and Soil Moisture based Brown Ocean Effect on an Extreme Rainfall Event from a Louisiana Gulf Coast Tropical System](https://www.nature.com/articles/s41598-019-53031-6)__

The authors use WRF to discuss the impact of Brown Ocean to extreme rainfall event for Hurricane Florence. They purposely changed land cover to which favors storm reintensification such as open water, etc.

__[Impact of Soil Moisture Initializations on WRF-Simulated North American Monsoon System](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020JD033858)__

This study initializes soil moisture based on five sets of experiemnts: wet, dry, normal, GLDAS, and SMAP. It was found that initial soil moisture affects precipitation through modulating both surface energy partition and atmospheric circulation. It also showed the soil memory by defining how long it takes for the differences in soil moisture from the initializations to reach zero.

<p align="center">
  <img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/035ad946-980d-46a6-8dcf-e373c859091b/jgrd56795-fig-0011-m.jpg">
</p>

__[Simulating the Effects of Land Surface Characteristics on Planetary Boundary Layer Parameters for a Modeled Landfalling Tropical Cyclone  Atmosphere](https://www.mdpi.com/2073-4433/13/1/138)__

This study, authors looked into four scenarios with WRF Nature Hurricane simulation - Wet Rough Run, Wet Smooth RUn, Dry Rough Run, and Dry Smooth Run by perturbing both soil moisture and roughness length (because of changes in frictional velocity).

It was found that Wet Smooth run produce most intensive hurricanes by minimum pressure and wind speed. They also separated outer rainband and inner rain band to show the difference.

__[Influence of ASCAT soil moisture on prediction of track and intensity of landfall tropical cyclones](https://www.tandfonline.com/doi/full/10.1080/01431161.2022.2164232)__

The authors assimilated ASCAT satellite soil moisture onto the coupled land-atmosphere model. They show the improvement of storm prediction by using observation in lieu of reanalysis data sets.

__[Soil heat extremes can outpace air temperature extremes Nat Clim Chan](https://www.nature.com/articles/s41558-023-01812-3)__

In this article, the authors explained the soil moisture/temperature and air temperature feedback. But more importantly, they revealed that warm soil surface will contribute to heat extremes in the form of sensible heat, and such increasing trend in soil heat extremes is observed from in-situ measurements and satellite measures, and forecasted to increase in the future as well.

<p align="center">
<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41558-023-01812-3/MediaObjects/41558_2023_1812_Fig2_HTML.png?as=webp">
</p>


### Negative feedback

__[Dry soils can intensify mesoscale convective systems PNAS](https://www.pnas.org/doi/10.1073/pnas.2007998117)__

In this article, the authors composites ~6000 MCS events and analyzed the role that dry soils can reintensify the MCSs.
How this works?
Dry soils enhance sensible heat flux, although at the expense of latent heat flux. It deepens and warms PBL, creating a temperature gradient that is favorable for intense MCSs. At a synaptic scale, dry soils modulate moisture convergence via thermal wind and wind shear.

<img src="https://www.pnas.org/cms/10.1073/pnas.2007998117/asset/c25251aa-7324-4907-baec-61251c252493/assets/images/large/pnas.2007998117fig05.jpg">

__[Feedback between the Land Surface and Rainfall at Convective Length Scales](https://journals.ametsoc.org/view/journals/hydr/5/4/1525-7541_2004_005_0625_fbtlsa_2_0_co_2.xml#i1525-7541-5-4-625-f04)__

The authors investigated the impact of 10-20 km scale MCS and how soil states reshape the development of MCS. They look at subsequent rainfall development and also the displacement from soil states to rainfall.

<p align="center">
<img src="https://d3n9xgu0z4cjsp.cloudfront.net/view/journals/hydr/5/4/images/i1525-7541-5-4-625-f12.gif">
</p>

__[Modeling soil moisture-precipitation feedback in the Sahel: Importance of spatial scale versus convective parameterization GRL](https://agupubs.onlinelibrary.wiley.com/doi/10.1002/2013GL058511)__

This study raises awareness that precipitation-soil-moisture feedback is highly dependent on convective parameterization in a numeric simulation, which may mislead the investigation. This is especially important when dealing with GCMs or RCMs which normally cannot resolve convective-scale precipitation.

__[Reconciling spatial and temporal soil moisture effects on afternoon rainfall Nat. Commun.](https://www.nature.com/articles/ncomms7443#citeas)__

The authors investigated both the positive feedback and negative feedback from satellite observed precipitation and soil moisture. In some regions, negative feedback is present (dry soil -> precipitation) such as Central US, Western Amazon, but in general, most of the places show positive feedback (wet soils -> precipitation).

Also, precipitation is triggered preferentially over **heterogeneous** soil moisture conditions.

__[Afternoon rain more likely over drier soils. Nature](https://www.nature.com/articles/nature11377#citeas)__

The authors found negative feedback from satellite observations but an opposite signal in global climate models. They inferred that the coarse-scale climate models, which cannot resolve convective precipitation, is likely the case that they do not reconcile with observations.

__[Frequency of Sahelian storm initiation enhanced over mesoscale soil-moisture patterns Nat. Geos.](https://www.nature.com/articles/ngeo1173)__

Idealized soil-moisture-induced flows (blue arrows) under light synoptic winds (black arrow) create an ascent region (large red arrow) where the shallow, strong current opposes the mean wind. The preferred location for convective initiation in this study coincides with the ascent region induced by the heating gradient at the downwind edge of the dry patch. Additional convergence over the dry patch is provided by a deep, weaker current at its upwind edge, and cross-wind gradients in soil moisture.

<p align="center">
  <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fngeo1173/MediaObjects/41561_2011_Article_BFngeo1173_Fig4_HTML.jpg?as=webp">
</p>

## Dry soil moisture propogate to reduce downwind precipitation

__[Drought self-propagation in drylands due to land–atmosphere feedbacks](https://www.nature.com/articles/s41561-022-00912-7)__

<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41561-022-00912-7/MediaObjects/41561_2022_912_Fig4_HTML.png?as=webp">

## Water vapor residence/depletion time

__[A revised picture of the atmospheric moisture residence time](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2015gl067449)__

In this paper, the authors compared two different approaches to look at global water vapor residence time - a Lagrangian approach and an Eulerian approach. They found sizeable differences between the two approaches to depict global water vapor residence time.

The schematic shows how a Lagrangian approach work:

<img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/42838dc7-8932-4d3e-8221-cddbde364e22/grl53937-fig-0001-m.jpg">

The global distribution of water vapor residence time:

<img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/602b7fc7-6a97-4d89-a45f-b09ee228467c/grl53937-fig-0002-m.jpg">
