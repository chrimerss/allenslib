---
layout: default
title: Radar Echo Extrapolation
parent: Precipitation Nowcasting
nav_order: 1
---

# Methodology

[Ph.D. Thesis of radar nowcasting: from methodology to verification](https://github.com/chrimerss/allenslib/tree/master/src/PhD_dissertation_v1_0.pdf)


__[A Reduced-Space Ensemble Kalman Filter Approach for Flow-Dependent Integration of Radar Extrapolation Nowcasts and NWP Precipitation Ensembles](https://journals.ametsoc.org/mwr/article/147/3/987/107474/A-Reduced-Space-Ensemble-Kalman-Filter-Approach)__

In this paper, the authors detailed a way to blend radar nowcasting with NWP data via a space-reduced Kalman filter approach.

They transform the high-dimention space data to low space with the PCA, and reconstruct back after the correction stage in the Ensemble Kalman Filter.

The result extends the nowcasting range further than without blending.

## STEPS

__[Development and verification of a real-time stochastic precipitation nowcasting system for urban hydrology in Belgium](https://hess.copernicus.org/articles/20/505/2016/)__

The description of STEPS system is as follows:

1. spatial scaling of precipitation fields (scale the precipitation fields based on FFT)

2. dynamic scaling of precipitation fields (scale the field dynamically by fitting a power law function of spatial scale)

3. spatial correlation of forecast errors (power law filter to white noise field in FFT field and inverse back)

4. temporal correlation of the forecast errors (Auto-regressive regression)

They verified the STEPS-BE algorithm with statistics within 2 hours leading time.

# Warn-on-Forecast

__[Jones, T. A., and Coauthors, 2020: Assimilation of GOES-16 Radiances and Retrievals into the Warn-on-Forecast System. Mon. Wea. Rev., 148, 1829–1859, https://doi.org/10.1175/MWR-D-19-0379.1.](https://journals.ametsoc.org/mwr/article/148/5/1829/346741)__

In this paper, the authors introduced the methodologies for developing the WoF system for 0-6h weather nowcasting.
