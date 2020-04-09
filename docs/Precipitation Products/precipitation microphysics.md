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

# Snowfall evaluation

__Wen, Y., Behrangi, A., Lambrigtsen, B., Kirstetter, P. (2016). Evaluation and Uncertainty Estimation of the Latest Radar and Satellite Snowfall Products Using SNOTEL Measurements over Mountainous Regions in Western United States. Remote Sensing. 8. 904. 10.3390/rs8110904.__

In this article, the authors used MRMS radar-only and IMERG liquidPrecipitationPercent field to conduct snow identification and quantification comparison with daily accumulations with specific snowfall-suited gauges. 

Conclusions:

1. Severe underestimation of daily snowfall accumulations for MRMS and IMERG. IMERG Final Cal outperforms MRMS and Uncal;
2. radar and satellite retrievals may not be able to capture increasing snowfall mass flux caused by temperature;
3. remote sensing retrievals have better performance in light snowfall events. For heavy snow, the underestimation is worse.
