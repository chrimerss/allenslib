---
layout: default
title: Satellite products
parent: Precipitation Products
nav_order: 3
---

# IMERG

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
  
