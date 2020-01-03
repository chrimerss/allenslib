---
layout: default
title: Satellite products
parent: Precipitation Products
nav_order: 3
---

# IMERG

Algorithm description:

IMERG data combined precipitation estimation from Passive Microwave (PMW) sensors comprising the GPM CO and then merged into half-hourly 0.1 by 0.1 degree fields using Goddard Profiling Algorithm (Olson, Yang, Stout, & Grecu, 2007) and intercalibrated with the GPM Combined Ku Radar-Radiometer Algorithm (CORRA) product [Grecu et al., 2016](https://journals.ametsoc.org/doi/10.1175/JTECH-D-16-0019.1). To fill in the gaps between PMW overpasses, the merged half-hourly 0.1°×0.1° is further recalibrated with Climate Prediction Center (CPC) Morphing-Kalman Filter (CMORPH-KF) Lagrangian time interpolation [Joyce & Xie, 2011](https://journals.ametsoc.org/doi/full/10.1175/JHM-D-11-022.1) and Precipitation Estimation from Remotely Sensed Information using Artificial Neural Networks Cloud Classification System (PERSIANN-CCS) [Hong, Hsu, Sorooshian, & Gao, 2004](https://journals.ametsoc.org/doi/full/10.1175/JAM2173.1). 
IMERG data archive consists of three stages, the first two is near-real-time as Early Run (~4 hour latency) and Late Run (~14 hour latency), and the latter post-analysis Final Run (~3.5 months latency). Early run uses only forward morphing, while late run and final run include both forward and backward morphing. Final run also incorporates monthly gauge adjustment with Global Precipitation Climatology Project (GPCP) at 1° grid box [Adler et al., 2003](https://journals.ametsoc.org/doi/full/10.1175/1525-7541%282003%29004%3C1147%3ATVGPCP%3E2.0.CO%3B2).


 
__Skofronick-Jackson, G., et al. (2017). "The Global Precipitation Measurement (Gpm) Mission for Science and Society." Bull Am Meteorol Soc 98(8): 1679-1695.__

This paper provides an overview about GPM and its auxiliary products (IMERG). It mentioned some constraints about GPM core constellation. 
 1. DPR has detectable rainfall range of (0.22, 110) mm/hour.
 2. GMI has detectable rainfall range of (0.2, 60) mm/hour.
 
and also some ground validation efforts e.g. with gauges, with mrms radars (conditional bias) to show whether it satisfies the goal.

At last, it wraps up some real-world applications of using GPM (IMERG) data.

## IMERG Stage intercomparison

__Mahmoud, M. T., Al-Zahrani, M. A., & Sharif, H. O. (2018). Assessment of global precipitation measurement satellite products over Saudi Arabia. Journal of Hydrology, 559, 1-12. doi:https://doi.org/10.1016/j.jhydrol.2018.02.015__

The author used IMERG 04 three stages: Early, Late, and Final to evaluate the accuracy of each stage for event-based, station-based, and region-based. All results suggest that Final is more accurate than both Early and Late.

__Chaoying Huang, J. H., Sheng Chen, Asi Zhang, Zhenqing Liang,Xinhua Tong ,Liusi Xiao, Chao Min,Zengxin Zhang (2019). "How Well Can IMERG Products Capture Typhoon Extreme Precipitation Events over Southern China? ." Remote Sensing 11(70): 1-22.__

Author in detail described difference between early product and final product (uncalibrated). He compared early product and final product
 with refered to gauge ground truth data for six extremely heavy precipitation events. The results indicated that IMERG final product
 can capture the spatial partterns of storm. with gauge calibrated is underestimated comapred to without gauge calibration over rainfall core. 
 

# PERSIANN

Author overviews three product: PERSIANN, PERSIANN-CCS, PERSIANN-CDR.

PERSIANN:
  1. infrared images transformed into hidden layer as a self-organizing feature map(SOFM) to classify the input data.
  2. discrete SOFM clusters are mapped to continuous space of outputs e.g. rainfall rate with comparing to PMW rainfall.
 
PERSIANN-CCS (cloud classification system):
  1. segament cloud imagery based on different temperature thresholds using incremental temperautre threshold (ITT).
  2. features i.e. coldness, geometry, texture are extracted from segamented imagery.
  3. For each group, relationship between brightness temperature and rain rate is constructed.
  
PERSIANN-CDR:
  1. it alternatively use NCEP stage IV hourly precipitataion data to train ANN model.
  2. uses GPCP monthly 2.5 degree precipitation data to reduce bias.
  
Evaluation:

  1. PERSIANN-CDR has least error and bias, mirrors the pattern of rainfall captured by CPC gauge data over CONUS for a long-run.
  2. for extreme events (>10mm), PERSIANN-CDR outperforms than PERSIANN-CCS and PERSIANN, but still underestimate.
  3. For global comparison, PERSIANN and PERSIANN-CDR exhibit good performance over mountainous regions while underperforming coastal regions.
  
# Satelite Precipitation intercomparison

__Chen, H., et al. (2019). "Comparison Analysis of Six Purely Satellite-derived Global Precipitation Estimates." Journal of Hydrology: 124376.__

The author compared six satellite QPEs e.g., IMERG-E, IMERG-L, PERSIANN-CCS, TRPA-NR, GSMaP-NRT, GSMap-MAK at daily global scale and hourly and daily over mainland China. And author decomposes BIAS into hits Bias, misses Bias, false Bias

Globally:
1. IMERG-L is the best among the other five, while GSMaP is the worst. 
2. IMERG suite reduced underestimation compared to GSMaP but still remain problematic in complex terrains.

Author decomposed RMSE with respect to rain rate, and found that 30% around of RMSE is comming from rain rate>32mm/day.

Over mainland China:  
1. IMERG overestimates light precipitation.
2. all products overestimate over semi-arid regions by false bias.
3. PERSIANN-CCS underestimates in humid regions, GSMaP overestimates semi-humid regions in warm season.

# Advanced Microwave Sounding Unit (AMSU)

[__Advanced microwave sounding unit cloud and precipitation algorithms__](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2002RS002679%4010.1002/%28ISSN%291944-799X.MARS01)

Author descibed algorithms for precipitation retrieval, cloud liquid water, and also including how to eliminate bias of AMSU-A NOAA-15 and NOAA-16 caused by asymeteric scaning.


# Satellite Precipitation Retrieval

Frequencies useful to infer rain rate [Source: CoMet course](https://www.meted.ucar.edu/satmet/microwave_topics/clouds_precip_wv_v2/navmenu.php?tab=1&page=2-11-0&type=flash):

1. 23-24 GHz: Weak water vapor absorption region, sensitive to water vapor through the entire depth of the atmosphere, sensitive to large cloud water content, sensitive to larger raindrops and low rain rates. Used mainly for water vapor estimation, water cloud and rainfall retrieval especially over oceans. (TPW used to observe ARs and storms)

2. 31-37 GHz: Window region, sensitive to large cloud water content, sensitive to medium to large drops and low rain rates.Used mainly for cloud and rainfall retrieval especially over oceans, and for surface feature characterization.(used to classify convective core in low clouds)

3. 50-60 GHz: Oxygen absorption region, sensitive to atmospheric temperature at different levels, sensitive to moderate cloud water content, sensitive to medium sized drops. Used mainly for temperature sounding and rainfall estimation.

4. 85-89 GHz: Atmospheric window region, sensitive to low cloud water content, sensitive to small drops, sensitive to precipitation-size ice particles.Used mainly for cloud and precipitation retrieval, and for surface feature characterization (used to identify deep convection.

5. 165 GHz: Atmospheric window region with some absorption by water vapor and oxygen, very sensitive to precipitation-size ice particles and small drops. Used mainly for cloud and precipitation retrieval especially over land, and surface feature characterization.

6. 175-190 GHz: Strong water vapor absorption region, sensitive to water vapor at various levels through the atmosphere, very sensitive to precipitation-size ice particles and small drops. Used mainly for moisture sounding and precipitation estimation, especially over land.
