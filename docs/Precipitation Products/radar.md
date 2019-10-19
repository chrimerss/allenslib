---
layout: default
title: radar
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
 
