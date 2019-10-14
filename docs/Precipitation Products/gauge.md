---
layout: default
title: Gauge products
parent: Precipitation Products
nav_order: 1
---

__NCEP Gridded Gauge Only__

Lin, Y. 2011. NCEP/EMC U.S. Gridded Gage Only Hourly Precipitation. Version 1.0. UCAR/NCAR - Earth Observing Laboratory. https://data.eol.ucar.edu/dataset/21.088. Accessed 14 Oct 2019.

__Seo, D.-J. (1998). "Real-time estimation of rainfall fields using rain gage data under fractional coverage conditions." Journal of Hydrology 208: 25-36.__

The interpolation techniques behind are described by (Seo 1998), which introduced Double Optimal estimation (DO) and Single Optimal estimation (SO) to gain conditional expectation of estimation. 

__Cecinati, F., Moreno-Ródenas, A., Rico-Ramirez, M., ten Veldhuis, M.-c., & Langeveld, J. (2018). Considering Rain Gauge Uncertainty Using Kriging for Uncertain Data. Atmosphere, 9(11). doi:10.3390/atmos9110446__

In another application example, (Cecinati, Moreno-Ródenas, Rico-Ramirez, ten Veldhuis, & Langeveld, 2018) compared the performance of four types of kriging (Ordinary Kriging, Ordinary Kriging for Uncertain Data, Kriging with External Drift with radar rainfall as covariate, Kriging for Uncertain Data with External Drift with radar rainfall as covariate). To leverage the spatial representativeness of radar data, variogram is first calculated as information for gauge interpolation in the frequency domain. Then fitted variogram provides covariance matrix for OK. To account for the uncertainty of gauge measurements, they included non-zero nugget so that the diagonal line of covariance does not equal to zero anymore.

__Fattoruso, G., Longobardi, A., Pizzuti, A., Molinara, M., Marocco, C., De Vito, S., . . . Di Francia, G. (2017). Evaluation and design of a rain gauge network using a statistical optimization method in a severe hydro-geological hazard prone area.__

(Fattoruso et al., 2017) formularized two objective functions, first to maximize the prediction accuracy, and second to minimize the cost due to maintenance, i.e. the minimum gauge number. The author also incorporated a time-dependent scaling factor in evaluating estimation variance. To solve for two optimization problem, the author utilized enumerative search algorithm and stop iteration when reaching pareto optimal.
