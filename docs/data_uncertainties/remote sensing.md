---
layout: default
title: satellite
parent: Data Uncertainties
nav_order: 3
---

__Sarachi, S., K. Hsu, and S. Sorooshian, 2015: A Statistical Model for the Uncertainty Analysis of Satellite Precipitation Products. J. Hydrometeor., 16, 2101–2117, https://doi.org/10.1175/JHM-D-15-0028.1__

Author utlized different distributions i.e. Generalized Normal Distribution (GND) to fit satellite precipitation data. The best model is found based on different aggregation levels e.g. spatial, temporal. Also, the author decomposed precipitation into summer and winter seasons because of the different characteristics.


__Hong, Y., et al. (2006). "Uncertainty quantification of satellite precipitation estimation and Monte Carlo assessment of the error propagation into hydrologic response." Water Resources Research 42(8).__
	
Author compared satellite data from PERSIANN-CCS, and NCEP stage IV radar data as reference from temperal, and spatial scale. From the analysis, satellite errors (RMSE) is mitigated as aggreated space and time, but the percentage of error (normalized) indicated that satellite tends to have larger relative error in lower range of rainfall intensity. What's more, author evaluated the error propogation by a hydrologic simulation, and offered an uncertainty estimation.

__Guo, H., et al. (2016). "Early assessment of Integrated Multi-satellite Retrievals for Global Precipitation Measurement over China." Atmospheric Research 176-177: 121-133.__

The author evaluated IMERG PrecipUncal and PrecipCal, found that calibrated precipitation improved the accuracy dramatically, while both Uncal and Cal suffer from light precipitation and winter, overestimating in these range in China.

__Sharifi, E., et al. (2016). "Assessment of GPM-IMERG and Other Precipitation Products against Gauge Data under Different Topographic and Climatic Conditions in Iran: Preliminary Results." Remote Sensing 8(2).__

Author compared IMERG final product with TMPA-3B42 and ECMWF, found that Overall, in daily scale the results reveal that all three products lead to underestimation but IMERG performs better than other products and underestimates precipitation slightly in all four regions. Good results were obtained with rainfall amounts greater than 15 mm/day during rainy periods or in humid regions. 

__Prakash, S., et al. (2016). "From TRMM to GPM: How well can heavy rainfall be detected from space?" Advances in Water Resources 88: 1-7.__

Author showed an improvement if IMERG data compared to TMPA data in detecting extreme rainfall events in India. Even though the TMPA data showed a larger probability of detection of heavy rainfall events most parts of the country, it showed a large false alarm ratio and a relatively small critical success index.

In this paper, authors utilized 75 percentile as a threshold to diffentiate heavy or normal events, and computed POD, FAR, CSI based on that criterion.

[__A global map of uncertainties in satellite‐based precipitation measurements__](https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/2010GL046008)

Author intercompared different products but all derived from TRMM, 3B42, 3B42RT, CMORPH, GSMaP, PERSIANN, NRL. The uncertainties are relatively small (40–60%) over the oceans, especially in the tropics, and over southern South America. There are large uncertainties (100–140%) over high latitudes (poleward of 40° latitude), especially during the cold season.

[__A TenYear Tropical Rainfall Climatology Based on a Composite of TRMM Products__](https://www.jstage.jst.go.jp/article/jmsj/87A/0/87A_0_281/_pdf/-char/en)

Author analyzed three composite products derived from TRMM, and used climatological statistics to estimate the uncertainties.

__O, S., et al. (2017). "Evaluation of GPM IMERG Early, Late, and Final rainfall estimates using WegenerNet gauge data in southeastern Austria." Hydrology and Earth System Sciences 21(12): 6559-6572.__

1. IMERG underestimates at high rain intensity, and overestimates at low rain intensity.  
2. IMERG-L only provides marginal benefits for IMERG-E.  
3. IMERG-F outperforms than early and late products.   

__Chen, S., et al. (2013). "Performance evaluation of radar and satellite rainfalls for Typhoon Morakot over Taiwan: Are remote-sensing products ready for gauge denial scenario of extreme events?" Journal of Hydrology 506: 4-13.__

Author compared four remote sensing products and ground based radar during excessive rainfall events in Taiwan. They compared the hourly rainfall and rainfall accumulation with metrics that conditioned at different percentiles. Overall, the results suggest that ground based radar is more close to referenced gauge data and thus can be replaced in gauge denial regions. Satellite QPE tends to underestimate extreme rainfall due to gauge smoother, missed precipitation outside of PMW overpass, iced areas assigned with 0 precipitation.

__Scofield, R. A. and R. J. Kuligowski (2003). "Status and Outlook of Operational Satellite Precipitation Algorithms for Extreme-Precipitation Events." Weather and Forecasting 18(6): 1037-1051.__

Geostationary satellites are especially important for their unique ability simultaneously to observe the atmosphere and its cloud cover from the global scale down to the storm scale at high resolution in both time (every 15 min) and space (1?4 km). This capability makes geostationary satellite data ideally suited for estimating and predicting heavy precipitation, especially during flash-flood events. Presented in this paper are current and future efforts in the National Environmental Satellite, Data, and Information Service that support National Weather Service River Forecast Centers and Weather Forecast Offices during extreme-precipitation events.


__Stampoulis, D. and E. N. Anagnostou (2012). "Evaluation of Global Satellite Rainfall Products over Continental Europe." Journal of Hydrometeorology 13(2): 588-603.__

The error statistics presented herein indicate that both orography and seasonal variability affect the efficiency of the satellite rainfall retrieval techniques. Specifically, both satellite techniques underestimate rainfall over higher elevations, especially during the cold season, and their performance is subject to seasonal changes. A significant difference between the two satellite products is that TRMM 3B42 V6 generally overestimates rainfall, while CMORPH underestimates it. CMORPH?s mean error is shown to be of higher magnitude than that of 3B42 V6, while in terms of random error variance, CMORPH exhibits lower (higher) values than those of 3B42 V6 in the winter (summer) months.

# Complex Terrain

__Mei, Y., E.N. Anagnostou, E.I. Nikolopoulos, and M. Borga, 2014: Error Analysis of Satellite Precipitation Products in Mountainous Basins. J. Hydrometeor., 15, 1778–1793, https://doi.org/10.1175/JHM-D-13-0194.1__

The author proposed a new metrics (AI) that is used to quantify false detection and difference: 

$$AI=\frac{2\sqrt{I}\sqrt{R}}{IR}$$

Further they seperates AI into three events and ploted in a radar graph.


