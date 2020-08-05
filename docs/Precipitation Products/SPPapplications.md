---
layout: default
title: Satellite Precipitation Applications
parent: Precipitation Products
nav_order: 6
---

# IMERG

## IMERG Stage intercomparison

__Mahmoud, M. T., Al-Zahrani, M. A., & Sharif, H. O. (2018). Assessment of global precipitation measurement satellite products over Saudi Arabia. Journal of Hydrology, 559, 1-12. doi:https://doi.org/10.1016/j.jhydrol.2018.02.015__

The author used IMERG 04 three stages: Early, Late, and Final to evaluate the accuracy of each stage for event-based, station-based, and region-based. All results suggest that Final is more accurate than both Early and Late.

__Chaoying Huang, J. H., Sheng Chen, Asi Zhang, Zhenqing Liang,Xinhua Tong ,Liusi Xiao, Chao Min,Zengxin Zhang (2019). "How Well Can IMERG Products Capture Typhoon Extreme Precipitation Events over Southern China? ." Remote Sensing 11(70): 1-22.__

Author in detail described difference between early product and final product (uncalibrated). He compared early product and final product
with refered to gauge ground truth data for six extremely heavy precipitation events. The results indicated that IMERG final product
can capture the spatial partterns of storm. with gauge calibrated is underestimated comapred to without gauge calibration over rainfall core. 
 
__Tapiador, F.J., A. Navarro, E. García-Ortega, A. Merino, J.L. Sánchez, C. Marcos, and C. Kummerow, 2020: The Contribution of Rain Gauges in the Calibration of the IMERG Product: Results from the First Validation over Spain. J. Hydrometeor., 21, 161–182, https://doi.org/10.1175/JHM-D-19-0116.1__
 
The author compared three stages of IMERG along with GPCP/GPCC and local gauge-derived products as reference. The overarching goal is to investigate the importance of gauge contributing to the performance of IMERG-F.
 
Author evaluated this point from different perspectives:
 
  1. annual 4 year mean of daily precipitation -> statement 1
  2. Seasonal comparisons -> statement 2
  3. Three versions comparison -> the difference is due to tuning procedures;
  4. PDF distribution of IMERG products and reference in seasons -> E and L better in winter (DJF) but F better in Spring (MAM);
  5. Time series in selected locations -> F is close to reference;
  6. Spatial structure using variogram in seasons and annual -> E has better spatial structure -> suspect a coincidence;
  
  
Some statements from this article include:
 
  1. The climatological gauge adjustment is expected to work well over long time scales while specific issues related to missing or capturing individual storm systems should create only random differences;
  2. Generally, IMERG-E and IMERG-L overestimate seasonal precipitation in summer but underestimate the precipitation in mountainous areas;
  3. All IMERG versions have larger MAPE (Mean Absolute Percentage Error) for light rainfall, with decreasing the error as the rainfall intensity increases;
  4. Aside from algorithm issues that are always exacerbated by coastal locations, another likely cause is that coastal areas in the Mediterranean are frequency affected by heavy precipitation events due to cuoff lows;

In the Discussion, the author described the uncertainties of the reference:

  1. Localized rainfall (induced by orographic precipitation and summer convection in semi-arid regions) is not well captured by interpolated gauge products because the decorrelation distance is high;
  2. 
 
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

# Integrated SPP product

__Brocca, L., Massari, C., Pellarin, T. et al. River flow prediction in data scarce regions: soil moisture integrated satellite rainfall products outperform rain gauge observations in West Africa. Sci Rep 10, 12517 (2020). https://doi.org/10.1038/s41598-020-69343-x__

In this paper, the authors compared a suite of SPPs mainly stemmed from top-down measurement and bottom-up inferred product. The top-down products involves GPM IMERG products, ERA5, GPCC, EOBS, and the inferred products are from soil moisture product, such as GPM-SM2RAIN, PRISM-SMAP, PRISM-SMOS.

Because these SPPs are highly associated with river flow prediction, the authors complemented with hydrologic evaluations, and they found that GPM-SM2RAIN performs the best in the data scarce regions (Africa).
