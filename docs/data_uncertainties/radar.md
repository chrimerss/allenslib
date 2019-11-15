---
layout: default
title: radar
parent: Data Uncertainties
nav_order: 2
---

__He, X., et al. (2013). "Evaluation of the value of radar QPE data and rain gauge data for hydrological modeling." Water Resources Research 49(9): 5989-6005.__

The author compared rain gauge raw data and radar-gauge collicated QPE product by feeding into hydrologic simulations, and results suggest the improvement introduced by using radar QPE data is in fact more obvious to groundwater than to surface water at daily scale.The radar QPE based model demonstrates the added value of the extra information from radar when rain gauge density decreases; however it is not able to sustain the level of model performance preceding the reduction in number of rain gauges.

__Medlin, J. M., et al. (2007). "Radar and Rain Gauge Analysis of the Extreme Rainfall during Hurricane Danny’s (1997) Landfall." Monthly Weather Review 135(5): 1869-1888.__

It is shown that both gauges and radar seriously underestimated event rainfall, and the Z-R relation should be ajusted during extreme events to get better estimation.

**Summary**

Radar QPE is normally evaluated in different scenarios i.e. extreme weather condition, hydrologic evaluation etc. (Medlin, Kimball et al. 2007) analysed the performance of radar QPE and also gauge data in hurricane Danny (1997), and found that both radar and gauge are severely underestimated the event. Thus they came up with the conclusion that we should apply different Z-R relationships regarding different weather conditions. (He, Sonnenborg et al. 2013) collocated radar-gauge QPE and performed hydrologic analysis. They concluded that radar QPE had limited improvement over the regions where gauge density are sparse. In order to account for uncertainties in radar QPE, (Kirstetter, Gourley et al. 2015) proposed a stochastic approach PQPE (Probabilistic Quantitative Precipitation Estimation) in which the author included range of Z-R relations, and computed range of rain rate by ensembles.
It is with no doubt that the coupled radar and gauge products will bring added information than any single product. Researchers have been looking for alternative ways to merge these products. In MRMS (multi-radar multi-sensor) product (Zhang, Howard et al. 2016), They adjusted mosaicked radar imagery by around 7000 hourly operational gauge data interpolated by inverse distance weighting. It is also possible to perform kriging analysis for both radar and gauge combination, specifically kriging with external-drift and kriging with radar-based error correction (Jewell and Gaussiat 2015, Cecinati, Moreno-Ródenas et al. 2018). 

**References**   
_Cecinati, F., A. Moreno-Ródenas, M. Rico-Ramirez, M.-c. ten Veldhuis and J. Langeveld (2018). "Considering Rain Gauge Uncertainty Using Kriging for Uncertain Data." Atmosphere 9(11)._ 
_He, X., T. O. Sonnenborg, J. C. Refsgaard, F. Vejen and K. H. Jensen (2013). "Evaluation of the value of radar QPE data and rain gauge data for hydrological modeling." Water Resources Research 49(9): 5989-6005.    
Jewell, S. A. and N. Gaussiat (2015). "An assessment of kriging-based rain-gauge-radar merging techniques." Quarterly Journal of the Royal Meteorological Society 141(691): 2300-2313._   
_Kirstetter, P.-E., J. J. Gourley, Y. Hong, J. Zhang, S. Moazamigoodarzi, C. Langston and A. Arthur (2015). "Probabilistic precipitation rate estimates with ground-based radar networks." Water Resources Research 51(3): 1422-1442._   
_Marian, E. P., P. Siska (2000). "Understanding Anisotropy Computations." Mathematical Geology 32: 683-700.   
Medlin, J. M., S. K. Kimball and K. G. Blackwell (2007). "Radar and Rain Gauge Analysis of the Extreme Rainfall during Hurricane Danny’s (1997) Landfall." Monthly Weather Review 135(5): 1869-1888.  
Zhang, J., K. Howard, C. Langston, B. Kaney, Y. Qi, L. Tang, H. Grams, Y. Wang, S. Cocks, S. Martinaitis, A. Arthur, K. Cooper, J. Brogden and D. Kitzmiller (2016). "Multi-Radar Multi-Sensor (MRMS) Quantitative Precipitation Estimation: Initial Operating Capabilities." Bulletin of the American Meteorological Society 97(4): 621-638._   

