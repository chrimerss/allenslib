---
layout: default
title: Detecting Flood from Earth Observation
parent: Hydrology
nav_order: 5
---

# Flood detection from remotely sensed products

<p align="center">
<img src="https://github.com/chrimerss/allenslib/blob/master/src/Flood%20detection.png?raw=true" width="100%">
</p>


__L. Landuyt, A. Van Wesemael, G. J. -. Schumann, R. Hostache, N. E. C. Verhoest and F. M. B. Van Coillie, "Flood Mapping Based on Synthetic Aperture Radar: An Assessment of Established Approaches," in IEEE Transactions on Geoscience and Remote Sensing, vol. 57, no. 2, pp. 722-739, Feb. 2019, doi: 10.1109/TGRS.2018.2860054.__

In this paper, the authors reviewed most commonly used techniques to derive flood extent from Sentinental missions and compared with real applications. They found the stable performance of active countour method in the flood monitoring.

__Chini, M.; Pelich, R.; Pulvirenti, L.; Pierdicca, N.; Hostache, R.; Matgen, P. Sentinel-1 InSAR Coherence to Detect Floodwater in Urban Areas: Houston and Hurricane Harvey as A Test Case. Remote Sens. 2019, 11, 107.__

In this paper, the authors proposed a way to map the flood extent with respect to bare soils and urban areas. For bare soil flooding, the adaptive thresholds are applied to mask flooded regions; for urban areas with building, multi-temporal images are acquired to compute the cross-correlation, Temporal Average Intensity, Temporal Average Coherence, and Local Incidence Angle.

They also showcased this methodology to Harvey events in 2017, demonstrated the ability to map the floodplains.

__[Near-real-time non-obstructed flood inundation mapping using synthetic aperture radar; Shen et al. 2018](https://www.sciencedirect.com/science/article/pii/S0034425718305169#!)__

![data processing streamlines](https://ars.els-cdn.com/content/image/1-s2.0-S0034425718305169-gr1_lrg.jpg)

__[Geodetic corrections to Amazon River water level gauges using ICESat altimetry](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2011WR010895)__

In this paper, the authors introduced a proof-of-concept study to derive water level from ICESat altimetry, and the accuracy to be found as 0.19 m in Amazon river basin.

__[Normalized Difference Flood Index for rapid flood mapping: Taking advantage of EO big data](https://doi.org/10.1016/j.rse.2018.03.006)__

In this article, the authors proposed a index called NDFI and NDFVI for flood mapping, taking advantage of big earth observation data (Sentinel-1 specifically).

They also reviewed 21 methodologies developed since 2000 for flood inundation mapping.

__[Flood Inundation Mapping from Optical Satellite Images Using Spatiotemporal Context Learning and Modest AdaBoost](https://www.mdpi.com/2072-4292/9/6/617)__

In this paper, the authors proposed a novel flood detection framework applied in two Chinese optical satellite (HJ and GF).

__[settings Open AccessFeature PaperArticle Fusion of SAR, Optical Imagery and Airborne LiDAR for Surface Water Detection](https://www.mdpi.com/2072-4292/9/9/890/htm)__

In this paper, the authors used three remotely sensed products: SAR, Optical Imagery and LiDAR to construct and fuse to one single possibly best flood/water extent map.

__[Real-time flood detection for video surveillance](https://ieeexplore.ieee.org/abstract/document/7392736)__

Using ground-based cameras to segment flooded areas, which could also be used as a means of flood extent delineation.


# Earth Observation Timeline

<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fncomms13844/MediaObjects/41467_2016_Article_BFncomms13844_Fig2_HTML.jpg?as=webp">


SOURCE: Elliott, J., Walters, R. & Wright, T. The role of space-based observation in understanding and responding to active tectonics and earthquakes. Nat Commun 7, 13844 (2016). https://doi.org/10.1038/ncomms13844


# Estimating discharge from satellite

__[RODEO: An algorithm and Google Earth Engine application for river discharge retrieval from Landsat](https://www.sciencedirect.com/science/article/pii/S1364815221002966#!)__

A GEE application that produces rating curves and discharge time series on-the-fly/.

They relate river width to modeled discharge data (GRADES), so called rating curve, and produce time series of discharge over the globe. They assessed the performance at ~500 in-situ gauge locations, achieving an median KGE value of 0.3.
