---
layout: default
title: Radar QPE
parent: Precipitation Products
nav_order: 2
---

__MRMS__

__Zhang, J., et al. (2016). "Multi-Radar Multi-Sensor (MRMS) Quantitative Precipitation Estimation: Initial Operating Capabilities." Bulletin of the American Meteorological Society 97(4): 621-638.__

__Measurements__

1)	MRMS radar data
MRMS network is comprised of 146 S-band (dual polarization) radar (typically frequency ranges from 2-4 Ghz, and wavelength 7.5-15 cm) and 30 C-band (single polarization) radar (typically frequency ranges from 4-8 Ghz, and wavelength 3.8-7.5 cm).
Quality control . 

    1.	Separation between hydrometeor and non-hydrometeor:
    
        a.	Correlation coefficient filter
        
        b.	Spatial (vertical and horizontal) filters to check the consistency
        
    2.	WF (wind farm) and AP (anomalous propagation) ground clutter
    
        a.	Remove WF from recorded data (under development?)
        
        b.	ANN based ground clutter removal/heuristic rule to remove by inspecting reflectivity intensity, echo depth, velocity gradient etc. (deployed in Canadian radars)
        
        c.	Attenuation (not applied yet)
        
    3.	Blockage
    
        a.	Linear interpolation to fill gaps (small)
        
        b.	Filled with upper tilt (large)
        
    4.	Overestimation in the bright band zone(intersection with melting layer)
    
        a.	Apparent vertical profile reflectivity correction (assume vertical variation is horizontally uniform)
        
    5.	Quality index is provided by taking blockage and vertical distance of bin into account
    
__Mosaic__   
Pixel point precipitation measurements are weighted by both relative distance from neighboring radar and also vertical distance of radar bin after fitting into an exponential function. The philosophy is trying to minimize false echo by relying more on low datum radar.
Precipitation type
Fall into 7 categories by classification algorithm (decision tree)
Quantification
Rain rate is estimated based on R-Z relationship after classification, and combine each R with associated type.


2)	Gauge data

7,000 hourly rain gauges from the Hydrometeorological Auto¬mated Data System from NOAA.
Quality control
The Gauge data are quality controlled by identifying ‘frozen’, ‘false zero’, ‘false precipitation’, ‘outliers too high’, ‘outliers too low’
Integration with radar

    1)	Calculate hourly rainfall difference
    
    2)	Interpolate hourly difference into gridded by inverse distance weighting
    
    3)	Bias correction with radar only product
    
    
3)	NWP model data

Numerical weather prediction data are integrated in mrms to provide information on type of precipitation (surface temp./wet bulb temp.), suitability for producing precipitation (relative humidity, wind field etc.)
Integration with radar
Provide information in classify precipitation type

4)	Precipitation climatology data

The gridded gauge data set called mountain mapper is a quality controlled, spatial representative data from PRISM over the US.
Integration with radar
Bias were calculated from mountain mapper product and gauge, followed by inversed-distance interpolation.

__Products__

Raw reflectivity – 2min/~1km   
Quality index – 2min   
Precipitation type – 2min   
Radar based QPE – 2min, 1h, 3h, 6h, 12h, 24h   
Gauge based QPE – 1 (3, 6, 12, 24) h   
Local gauge bias corrected QPE – 1 (3, 6, 12, 24) h   
gauge-and-precipitation-clima¬tology-merged QPE. 48 (72) h    


__Challenges__   
1)	Blockage and orographic enhanced precipitation remain unsolved.
2)	Vertical variability of reflectivity
3)	Uncertainty remained for frozen precipitation due to lack of in situ monitoring measurements.
4)	Potential usage of R-Kdp or R-A based on different schemes.


__Saltikoff, E., et al. (2019). "An Overview of Using Weather Radar for Climatological Studies: Successes, Challenges, and Potential." Bulletin of the American Meteorological Society 100(9): 1739-1752.__

Table 2. Data portals where radar data or archived images can be downloaded.

|Area|Provider|Since|Radars|URL|
|:--:|:------:|:---:|:----:|:-:|
|Australia|BoM|1998|79|http://openradar.io/au|
|Europe|OPERA|2012|140|Ask for license from info@eumetnet.eu|
|Germany|DWD|2001|17|https://opendata.dwd.de|
|Netherlands|KNMI|1998/2008|2|https://data.knmi.nl/datasets?q=radar(https://climate4impact.eu)|
|New Zealand|MetService|2011|9|https://about.metservice.com/our-company/about-this-site/open-access-data/|
|Norway|Met|2010|9|http://thredds.met.no/thredds/remotesensingarchive.html|
|United States|NEXRAD|1991|160|www.ncdc.noaa.gov/data-access/radar-data/nexrad|

"In our experience, the added value of radar for climate monitoring is particularly high for convective precipitation with high spatial and temporal variations, which cannot correctly be captured by rain gauge networks."

# Precipitation classification

__[The NSSL Hydrometeor Classification Algorithm in Winter Surface Precipitation: Evaluation and Future Development](https://journals.ametsoc.org/view/journals/wefo/26/5/waf-d-10-05011_1.xml)__

In this study, the authors investigated NSSL hydrometeor classification algorithm against near ground reportings. They found:

1. HCA appears to classify too many cases as liquid when either frozen or none is reported.
2. HCA seems work in identifying precipitation.
3. HCA does no better than linear discriminant analysis
4. In summary, HCA is not suitable for determining hydrometeor type near the ground in winter precipitation

Explainations:

The poor performance of the HCA on frozen precipitation may be explained in part because frozen precipitation is sometimes mixed with varying amounts of rain. Observers are not asked to report mixed precipitation because doing so reliably requires unavailable training. Another likely contributor is that the current HCA does not account for refreezing below the melting level, a common occurrence in winter precipitation.

__[Classification of Precipitation Types during Transitional Winter Weather Using the RUC Model and Polarimetric Radar Retrievals](https://journals.ametsoc.org/view/journals/apme/51/4/jamc-d-11-091.1.xml)__

The authors discussed three main issues relating to HCA algorithms:

1. the existing HCA was primarily developed for warm-season weather, it may not work efficiently for cold-season storms for which the height of melting layer is below 1km
2. it is essentially ‘‘local.’’ That is, it provides class designations at everyelevation sweep, using only radar information collected at that sweep rather than in a full 3D volume.
3. the existing polarimetric HCA is entirely radar based; no thermodynamic information is utilized in the classification process.
4. The classification of cold-season precipitation type at the surface is further complicated by the broad range of precipitation types that might result from processes that occur below the primary melting level


# Snow-ice

__[Sergey Y. Matrosov](https://cires.colorado.edu/researcher/sergey-matrosov)__

__[The Use of CloudSat Data to Evaluate Retrievals of Total Ice Content in Precipitating Cloud Systems from Ground-Based Operational Radar Measurements](https://journals.ametsoc.org/view/journals/apme/54/7/jamc-d-15-0032.1.xml)__


Even in tropics about 40% of rain is stratiform-like (Houze 1997). In midlatitudes often more than half of total liquid precipitation comes from stratiform-like systems (e.g., Matrosov et al. 2014). Such systems are considered in this study.

It elaborates radar beam broadening in a graph.

<p align="center">
<img src="https://journals.ametsoc.org/view/journals/apme/54/7/full-jamc-d-15-0032.1-f1.jpg" height="50%">
</p>

from the results, a good correlation is found (r=0.7) between WSR-88D ground radar and CloudSat satellite, without obvious systematic bias.

