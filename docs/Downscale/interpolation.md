---
layout: default
title: Spatial interpolation
parent: Downscale
nav_order: 2
---

# Flow interpolation

__Chokmani, K., and T. B. M. J. Ouarda (2004), Physiographical space-based kriging for regional flood frequency estimation at ungauged sites, Water Resour. Res., 40, W12514, doi:10.1029/2003WR002983.__

This paper attempted to better estimate regional flood frequency estimation using kriging.
The data was obtained from 151 gauging stations in Quebec and interpolated flow quantities over
the physiographical space rather than the conventional geographical space. Using this method, flood
quantiles could be interpolated at any ungauged location based on coordinates. Multivariate analysis
defining the physiographical space was conducted using canonical correlation analysis and the principal
component analysis. The nugget effect added to the Gaussian model to display the discontinuity at the
origin displayed in the experimental variograms, and yielded 10, 50, and 100-year return results similar
to conventional CCA and PCA calculations. The study concluded that the estimation method that was investigated
produced similar results to the traditionally used canonical correlation analysis based regional estimation
approach, where longer return periods were less predictable than shorter period.

# Rainfall interpolation

__Grimes, D.I., E. Coppola, M. Verdecchia, and G. Visconti, 2003: A Neural Network Approach to Real-Time Rainfall Estimation for Africa Using Satellite Data. J. Hydrometeor., 4, 1119–1133, https://doi.org/10.1175/1525-7541(2003)004<1119:ANNATR>2.0.CO;2__

This paper proposed a new approach to rainfall estimation in Africa using 4 years of rain gauge data from Zambia.
The current approach, Cold Cloud Duration, defines pixels as the number of hours the temperature is colder than
a defined temperature and applies a linear relationship between this duration and the rainfall amount. The new 
method improved this Cold Cloud Duration by kriging guage pixel data on three different timescales; daily rainfall
qualities with a scale of 1 pixel per day, daily ranfall average with scale if 10 pixels per day, and daily rainfall
average over 10 day period with scale of 100 pixels per day. Grimes’ et al approach showed a consistent, small
improvement over the standard Cold Cloud Duration method, but was better at modeling higher precipitation totals.
Application outside of central Africa still needs to be determined.
