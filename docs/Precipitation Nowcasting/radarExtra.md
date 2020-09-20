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