---
layout: default
title: precipitation microphysics
parent: Precipitation Products
nav_order: 5
---
# Convective or Stratiform?

[Separation of Convective and Stratiform Precipitation Using Microwave Brightness Temperature](https://journals.ametsoc.org/doi/pdf/10.1175/1520-0450%281999%29038%3C1195%3ASOCASP%3E2.0.CO%3B2)

Key insights:

1. convective takes up 70% of total rainfall volume while stratiform takes the rest while the pixels for stratiform account for 70%.
This feature is at fine scale (2km). when increase the spatial footprint, this feature is lessened, and smoothed.

2. they propose an algorithm to separate convective and stratiform by taking the neighboring cells into account and evaluate the brightness temperature spatial variations.

3. features extracted VI - brightness temperature absolute difference between center pixel and surrounding pixels; VC - brightness temperature difference
between the center pixel and the averaged value of the surrounding pixels; VM - is the maximum temperature enhancement due to emission for the 19- and 37-GHz
channels or the maximum depression due to scattering at 85 GHz.

# Snowfall/Ice evaluation

__Wen, Y., Behrangi, A., Lambrigtsen, B., Kirstetter, P. (2016). Evaluation and Uncertainty Estimation of the Latest Radar and Satellite Snowfall Products Using SNOTEL Measurements over Mountainous Regions in Western United States. Remote Sensing. 8. 904. 10.3390/rs8110904.__

In this article, the authors used MRMS radar-only and IMERG liquidPrecipitationPercent field to conduct snow identification and quantification comparison with daily accumulations with specific snowfall-suited gauges. 

Conclusions:

1. Severe underestimation of daily snowfall accumulations for MRMS and IMERG. IMERG Final Cal outperforms MRMS and Uncal;
2. radar and satellite retrievals may not be able to capture increasing snowfall mass flux caused by temperature;
3. remote sensing retrievals have better performance in light snowfall events. For heavy snow, the underestimation is worse.

__Behrangi, A., Bormann, K. J., & Painter, T. H. ( 2018). Using the Airborne Snow Observatory to assess remotely sensed snowfall products in the California Sierra Nevada. Water Resources Research, 54, 7331– 7346. https://doi.org/10.1029/2018WR023108__

In this paper, authors compared all-possible satellite precipitation estimates along with MRMS against gauge references to evaluate the respective performance of satellite sensors in snowfall estimates.

Surprisingly, IR (PERSIANN) sensor outperforms than PMW (IMERG) even though IR lacks scattering channels. The author attributes this to the icy/snowy surface in extreme winter storms.

__[A Polarimetric Analysis of Ice Microphysical Processes in Snow, Using Quasi-Vertical Profiles](https://journals.ametsoc.org/view/journals/apme/57/1/jamc-d-17-0033.1.xml)__

__[Quasi-Vertical Profiles—A New Way to Look at Polarimetric Radar Data](https://journals.ametsoc.org/view/journals/atot/33/3/jtech-d-15-0020_1.xml)__

In this paper, the authors proposed a new way (Quasi-vertical-profile) to interpret the hydrometeors.

# Impact of Aerosal to precipitation

__Li, Z., Niu, F., Fan, J. et al. Long-term impacts of aerosols on the vertical development of clouds and precipitation. Nature Geosci 4, 888–894 (2011). https://doi.org/10.1038/ngeo1313__

In this big paper, the author described the impact of aerosols, particularly cloud nuclei concentration (CCN) to cloud top height with classification on cloud top temperatures;

In the second part, the author investigated the impact of CCN to precipitation, and found a significant impact for liquid phase precipitation while weak relation to solid precipitaion;

To corroborate the finding, the author conducted simulations (cloud-resolving model) to correlate the observations with model simulations.


__Yang, Y., J. Fan, L.R. Leung, C. Zhao, Z. Li, and D. Rosenfeld, 2016: Mechanisms Contributing to Suppressed Precipitation in Mt. Hua of Central China. Part I: Mountain Valley Circulation. J. Atmos. Sci., 73, 1351–1366, https://doi.org/10.1175/JAS-D-15-0233.1__

In this article, the author found a scheme which describes the increase of aerosols leading to the decrease in rainfall-frequency because of the change of orographic lifting.

To do that, they conducted simulations on changing aerosol loadings with WRF-Chem.

" Aerosols can impact precipitation through ACI by 1) producing more cloud droplets of smaller drop size that changes cloud microphysics (Twomey 1977), 2) releasing latent heat as a result of changes in microphysical processes that modulate cloud dynamics (e.g., Wang 2005; Khain et al. 2005; van den Heever et al. 2006; Tao et al. 2007; Rosenfeld et al. 2008; Fan et al. 2012; Altaratz et al. 2014), and 3) changing atmospheric stability through radiation feedback from microphysical changes (Fan et al. 2013; Morrison and Grabowski 2012)."

# Techniques for ice precipitation observations

## Quasi-vertical profile (QVP)

__[Quasi-vertical profiles: A new way to look at polarimetric radar data](https://journals.ametsoc.org/view/journals/atot/33/3/jtech-d-15-0020_1.xml)__
<p align="center">
  <img src="https://journals.ametsoc.org/view/journals/atot/33/3/images/full-jtech-d-15-0020_1-f2.jpg">
</p>


## Range-defined quasi-vertical profile (RD-QVP)

__[Polarimetric Radar and Surface-Based Precipitation-Type Observations of Ice Pellet to Freezing Rain Transitions](https://journals.ametsoc.org/view/journals/wefo/32/6/waf-d-17-0054_1.xml)__

<p align="center">
<img src="https://journals.ametsoc.org/view/journals/wefo/32/6/images/full-waf-d-17-0054_1-f1.jpg">
</p>

## Columnar Vertical Profile (CVP)

__[Polarimetric Radar Retrievals in Ice Using In Situ Aircraft Measurements](https://journals.ametsoc.org/view/journals/atot/37/9/jtechD200011.xml)__

<p align="center">
<img src="https://journals.ametsoc.org/view/journals/atot/37/9/full-jtechD200011-f4.jpg">
</p>
