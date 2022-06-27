---
layout: default
title: Hydro-Climatology
parent: Extreme Events
nav_order: 3
---

# long-term extreme precipitation

## West US

Main driving agent is the Atmospheric river

__[Hourly storm characteristics along the U.S. West Coast: Role of atmospheric rivers in extreme precipitation GRL](https://agupubs.onlinelibrary.wiley.com/doi/10.1002/2017GL074193)__

Despite generally lower hourly intensities, precipitation totals along the U.S. West Coast (USWC) are comparable to those in southeast U.S. (SEUS). Storm durations, more so than hourly intensities, strongly modulate precipitation-total variability over the USWC, where the correlation coefficients between storm durations and storm totals range from 0.7 to 0.9. Atmospheric rivers (ARs) contribute 30–50% of annual precipitation on the USWC and make such large contributions to extreme storms that 60–100% of the most extreme storms, i.e., storms with precipitation-total return intervals longer than 2 years, are associated with ARs.

## US
[ENSO and Wintertime Extreme Precipitation Events over the Continuous US](https://journals.ametsoc.org/doi/pdf/10.1175/2007JCLI1705.1)

1. EOFs are used to analyze daily precipitation fields with compositing 500-mb heights
2. study domain CONUS but special focues on coastal regions
3. From PCs to infer large flood events;
4. Inspect how ENSO impact extreme precipitation (Gumbel PDF)

__Prat, O. P., & Nelson, B. R. (2015). Evaluation of precipitation estimates over CONUS derived from satellite, radar, and rain gauge data sets at daily to annual scales (2002–2012). Hydrology and Earth System Sciences, 19(4), 2037.__

The author adopts adaptive absolute rain rates to define extreme (i.e., WMMD=17.3 mm/day, 2 in/day, 4 in/day).

__[U.S. Hydrologic Design Standards Insufficient Due to Large Increases in Frequency of Rainfall Extremes](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019GL083235)__

Authors investigated the observed ARI (Annual recurrence interval) of extreme rainfall versus NOAA Atlas 14 product to show the trend.

The motivation is to amplify that Evidence for intensifying rainfall extremes has not translated into “actionable” information needed by engineers and risk analysts.

## China

[Spatial and temporal variation of extreme precipitation over the Yangtze River Basin](https://doi.org/10.1016/j.quaint.2007.09.001) 

1. Extreme precipitation analysis in Yangtze River in China
  a. Long-term trend is detected from non-parametric Sean's method
  b. REOF (rotated EOF) is used to find both spatial and temporal variability
  c. wavelet transform to decompose time series into time-frequency space to discover the periodicity;
  
2. Extreme events is defined as daily precipitation exceeding 95th percentile


__Miao, C., H. Ashouri, K. Hsu, S. Sorooshian, and Q. Duan, 2015: Evaluation of the PERSIANN-CDR Daily Rainfall Estimates in Capturing the Behavior of Extreme Precipitation Events over China. J. Hydrometeor., 16, 1387–1396, https://doi.org/10.1175/JHM-D-14-0174.1__

The main purpose of this study is to analyze the climatology of long-range rainfall simulation, particularly for PERSIANN-CDR, and also to validate the accuracy of it.

Three indices are used to perform evaluation: 1. percentile indices RR99, RR95; 2. Absolute threshold indices (R20mm etc.); 3. Maximum indices (Rx1day, Rx5day etc.)

The conclusion is that overall PERSIANN-CDR shows an agreement with ground observations for long-term climatological studies except for some reserved regions like Tibetan Plateau.

## Globe

[Westra, S., L.V. Alexander, and F.W. Zwiers, 2013: Global Increasing Trends in Annual Maximum Daily Precipitation. J. Climate, 26, 3904–3918, https://doi.org/10.1175/JCLI-D-12-00502.1](https://journals.ametsoc.org/doi/pdf/10.1175/JCLI-D-12-00502.1)

1. The dataset is from HadEX2 with Rx1day ranging from 1900 to date globally;

2. Annual maximum daily precipitation is analyzed in this study with two ways of testing the trends: (1) Mann-Kendall test; (2) GEV;

3. In their analysis, the significance is calculated based on a resampling procedure;

4. Near surface temperature is examined to test the relationship with extreme precipitation: they found most positive associations;

[Global trends in extreme precipitation: climate models versus observations (HESS)](https://www.hydrol-earth-syst-sci.net/19/877/2015/hess-19-877-2015.pdf)

1. different scenarios in CMIP5 model against HadEX2 are compared in terms of the extreme precipitation trends: most of the results showing positive extreme precipitation trends. Linear regression slope and Mann-Kendall test are used in this study.

2. different percent of change under global warming are tested to project the potential increase in extreme precipitation.


[Comparison of the GPCP and CMAP Merged Gauge–Satellite Monthly Precipitation Products for the Period 1979–2001](https://journals.ametsoc.org/doi/pdf/10.1175/JHM-392.1)

1. Normalized precipitation (remove climatological mean and divided by standard deviation)
2. EOF analysis: common EOF (cEOF) to study the common spatial patterns in the GPCP and CMAP. To perform this, GPCP and CMAP are concatenated along time dimension and then separated.
3. An interesting plot with x the month and y axis the year. In between is the spatial correlation
    Due to the variability nature of precipitation, the EOF modes only explain little amount of variations.
    


__[Stationary and non‐stationary detection of extreme precipitation events and trends of average precipitation from 1980 to 2010 in the Paraná River basin, Brazil](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/joc.6265)__

In this article, the authors investigated the trends and stationarity for extreme rainfall in Brazil.

They used three modes of GEV analysis: 1) stationary GEV; 2) non-stationary GEV with varing location parameter; 3) non-stationary GEV with varying both location and scale parameters.

They performed grid-based analysis towards stationarity check.

__[Rainfall statistics, stationarity, and climate change](https://www.pnas.org/content/115/10/2305)__

This work is published in PNAS.

The dataset used in the global land surface precipitation is GPCC Version 5.

They set criteria to check stationarity: 1) the mean of annual precipitation is constant and 2) the autocorrelation only depends on the relative position in the time series.

# How to define extreme rainfall events?

__Stevenson, S.N. and R.S. Schumacher, 2014: A 10-Year Survey of Extreme Rainfall Events in the Central and Eastern United States Using Gridded Multisensor Precipitation Analyses. Mon. Wea. Rev., 142, 3147–3162, https://doi.org/10.1175/MWR-D-13-00345.1__

The author constructed extreme rainfall events alike IDF curve but with radar gridded product, determining 100yr/50yr return plus the time accumulation (1h,6h,24h) with 10 years of data.

They analyzed the distribution of extreme rainfall events in terms of seasonality, diurnal effect, and topography based on these categories.

__Zhou, Y., Nelson, K., Mohr, K. I., Huffman, G. J., Levy, R., & Grecu, M. (2019). A spatial‐temporal extreme precipitation database from GPM IMERG. Journal of Geophysical Research: Atmospheres__

In this article, the authors proposed a way to identify extreme precipitation events with following approaches:
1. construct inventory (EXT) from grid exceeding the mean precipitation plus 2.5 standard deviation;
2. find the maximum in the EXT, and search for the neighboring grid (d<dis_threshold;t<time_threshold);
3. loop through all grids in the EXT
4. include light rain within the threshold basis;
5. repeat 2 until all grids in EXT are examined

__[Contribution of large-scale midlatitude disturbances to hourly precipitation extremes in the United States](https://link.springer.com/article/10.1007/s00382-018-4123-5)__

The authors analyzed the US extreme precipitation rates, attributed to jet streams and cutoff lows. Over 95% of 1-h annual maximum precipitation along west coast coincident with jet stream while 30% of interior western US is impacted by cutoff lows.

# Intense precipitation evaluations

__AghaKouchak, A., Behrangi, A., Sorooshian, S., Hsu, K., and Amitai, E. ( 2011), Evaluation of satellite‐retrieved extreme precipitation rates across the central United States, J. Geophys. Res., 116, D02115, doi:10.1029/2010JD014741.__

In this paper, authors addresses the extreme precipitation estimation with four satellite products. The metrics used in evaluating these satellite performance can be considered. Also intriguing, PERSIANN shows less bias than TMPA in the results from a purely data exploratory perspective.


# Climate change and extreme precipitation

__[Andreas Prein](https://scholar.google.com.sg/citations?user=kX-KiyIAAAAJ&hl=en&oi=sra)__

__[Increased rainfall volume from future convective storms in the US (Nature Climate Change)](https://www.nature.com/articles/s41558-017-0007-7)__

The authors used the CONUS-I dataset to diagnose future extreme precipitation changes from the perspective of MCSs by using a storm tracking algorithm object-based diagnostic evaluation (MODE).

What is interesting here is that they plotted the precipitation in terms of intensity-area curve, from which one can tell what the change would be for the storm characteristics. Finnaly, to attribute changes to warming environment, they compared the cloud top temperature for concatenated events.

<p>
<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41558-017-0007-7/MediaObjects/41558_2017_7_Fig3_HTML.jpg?as=webp">
</p>

__[Monitoring and understanding trends in extreme storms (BAMS)](https://journals.ametsoc.org/view/journals/bams/94/4/bams-d-11-00262.1.xml?tab_body=pdf)__

Extreme precipitation changes are analyzed using trustworthy rain gauges over the US since 1948. About 76% of all stations showing increasing, among which 15% shows significant increase. From the central United States to the North Atlantic, these exhibit a high degree of spatial coherence. 

2. Hurricane/TC activities are found to increase according to Power Dissipation Index. Connections with large scale oscillation and Atlantic Cyclones are a matter of debate. In addition, anthropogenic emissions and volcanic activities are less certain in terms of their roles in contributing to extreme precipitation.
3. Winter storms are discussed with ENSO, North Atlantic Oscillation, Arctic Oscillation.

__[Future changes to the intensity and frequency of short-duration extreme rainfall (Rev. Geophys.](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2014RG000464)__

A comprehensive review on climate change studies including theoritical explainations.

A common conclusion to these studies is that subdaily extreme rainfall is intensifying more rapidly than rainfall measured at daily time scales. This could have significant societal consequences, since floods produced by short-duration rainfall (often referred to as “flash” floods).

1. Hourly precipitation with temperature scaling ratio is discussed.
2. Moisture availability is discussed - Trends in precipitation extremes in the United States also have been linked to precipitable water changes
3. Influence of Rainfall Type on Scaling - convective extremes are by nature more intense and have shorter durations than large-scale rainfall and (b) the proportion of extreme rainfall which is convective increases with atmospheric temperature. higher CC scaling is found for convective system.
4. Cloud dynamics play a role in extreme precipitation changes.
5. Clausius-Claypean - In some dry areas, scaling appears to be lower than CC
6. Insights from Global Climate Models - Current convection parameterization schemes are not able to represent rainfall from storms that continually regenerate in the same location as a result of the storm dynamics or storms that are locally organized because of topographical influence.
7. Rainfall-flood association - it discusses how to define extreme rainfall
8. Relationship between rainfall duration and catchment size - smaller catchments are sensitive to short but intense bursts of rainfall, sometimes lasting only an hour or less, whereas larger catchments are sensitive to extended periods of heavy rainfall lasting for several days or longer.

<p align="center">
  <img src="https://agupubs.onlinelibrary.wiley.com/cms/asset/f3d36bc9-7ecb-4ef7-9dae-d5a7c7e9c50c/rog20045-fig-0004-m.jpg">
</p>

__[Resilience to Extreme Rainfall Starts with Science BAMS](https://journals.ametsoc.org/view/journals/bams/102/4/BAMS-D-20-0267.1.xml)__

In this article, the authors call for attention to update storm database to guide building resilient society. The out-of-date NOAA Atlas 14 poses hurdles to design up-to-date flood infrastructure and resilient measures.

__[Declining tropical cyclone frequency under global warming Nat Climate Change](https://www.nature.com/articles/s41558-022-01388-4)__

The authors reconstructed long-term TC frequency to show a decreasing trend in most of regionos, especially during the periods of post-industrialization

<src img="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41558-022-01388-4/MediaObjects/41558_2022_1388_Fig2_HTML.png?as=webp">

Beyond findings, the authors attributed the changes to (1) mid-tropospheric upward mass flux, (2) environmental vertical wind shear, and (3) saturation deficit (mid-tropospheric dryness).

# Hydroclimatology

__[Hydroclimatic trends during 1950–2018 over global land](https://link.springer.com/article/10.1007%2Fs00382-021-05684-1)__

the authors updated hydroclimatologic variables: precipitation, streamflow, evaporation from the period 1950 to 2018. He specifically analyzed the historical trends over global land surface.


