---
layout: default
title: Climatology
parent: Extreme Events
nav_order: 3
---

# long-term extreme precipitation (annual daily maximum)

[Spatial and temporal variation of extreme precipitation over the Yangtze River Basin](https://doi.org/10.1016/j.quaint.2007.09.001) 

1. Extreme precipitation analysis in Yangtze River in China
  a. Long-term trend is detected from non-parametric Sean's method
  b. REOF (rotated EOF) is used to find both spatial and temporal variability
  c. wavelet transform to decompose time series into time-frequency space to discover the periodicity;
  
2. Extreme events is defined as daily precipitation exceeding 95th percentile

[Westra, S., L.V. Alexander, and F.W. Zwiers, 2013: Global Increasing Trends in Annual Maximum Daily Precipitation. J. Climate, 26, 3904–3918, https://doi.org/10.1175/JCLI-D-12-00502.1](https://journals.ametsoc.org/doi/pdf/10.1175/JCLI-D-12-00502.1)

1. The dataset is from HadEX2 with Rx1day ranging from 1900 to date globally;

2. Annual maximum daily precipitation is analyzed in this study with two ways of testing the trends: (1) Mann-Kendall test; (2) GEV;

3. In their analysis, the significance is calculated based on a resampling procedure;

4. Near surface temperature is examined to test the relationship with extreme precipitation: they found most positive associations;

[Global trends in extreme precipitation: climate models versus observations (HESS)](https://www.hydrol-earth-syst-sci.net/19/877/2015/hess-19-877-2015.pdf)

1. different scenarios in CMIP5 model against HadEX2 are compared in terms of the extreme precipitation trends: most of the results showing positive extreme precipitation trends. Linear regression slope and Mann-Kendall test are used in this study.

2. different percent of change under global warming are tested to project the potential increase in extreme precipitation.


[ENSO and Wintertime Extreme Precipitation Events over the Continuous US](https://journals.ametsoc.org/doi/pdf/10.1175/2007JCLI1705.1)

1. EOFs are used to analyze daily precipitation fields with compositing 500-mb heights
2. study domain CONUS but special focues on coastal regions
3. From PCs to infer large flood events;
4. Inspect how ENSO impact extreme precipitation (Gumbel PDF)

[Comparison of the GPCP and CMAP Merged Gauge–Satellite Monthly Precipitation Products for the Period 1979–2001](https://journals.ametsoc.org/doi/pdf/10.1175/JHM-392.1)

1. Normalized precipitation (remove climatological mean and divided by standard deviation)
2. EOF analysis: common EOF (cEOF) to study the common spatial patterns in the GPCP and CMAP. To perform this, GPCP and CMAP are concatenated along time dimension and then separated.
3. An interesting plot with x the month and y axis the year. In between is the spatial correlation
    Due to the variability nature of precipitation, the EOF modes only explain little amount of variations.
