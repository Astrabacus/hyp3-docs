# Available HyP3 Products

On-demand SAR products generated using HyP3 are currently available for the [Sentinel-1 mission](sentinel1.md "Sentinel-1 Mission" ){target=_blank} only.

## RTC

SAR datasets inherently contain geometric and radiometric distortions due to terrain
being imaged by a side-looking instrument. Radiometric Terrain Correction (RTC) removes
these distortions and creates analysis-ready data suitable for use in GIS applications.
RTC processing is a required first step for many amplitude-based SAR applications.

Sentinel-1 RTC products are generated leveraging GAMMA Software. Products are distributed as
UTM-projected GeoTIFFs with a pixel spacing of either 
[10 or 30 meters](guides/rtc_product_guide.md#pixel-spacing "RTC Pixel Spacing Documentation" ){target=_blank}. 
To learn more, refer to our [ASF Sentinel-1 RTC Product Guide](guides/rtc_product_guide.md 
"ASF Sentinel-1 RTC Product Guide" ){target=_blank}.

For step-by-step instructions for searching for, ordering, downloading and using On Demand RTC products, visit our [RTC On Demand!](https://storymaps.arcgis.com/stories/2ead3222d2294d1fae1d11d3f98d7c35 "RTC On Demand! StoryMap" ){target=_blank} tutorial.

A Digital Elevation Model (DEM) is required for processing RTC. ASF uses the
best publicly-available DEM with full coverage of the processing area. To learn more,
refer to our [Digital Elevation Models](dems.md "HyP3 DEM Documentation" ){target=_blank} documentation.

## InSAR

Interferometric SAR (InSAR) uses the phase differences from repeat passes over the
same area to identify regions where the distance between the sensor and the Earth's
surface has changed. This allows for the detection and quantification of deformation
or movement. To learn more, refer to our [ASF Sentinel-1 InSAR Product Guide](guides/insar_product_guide.md "ASF Sentinel-1 InSAR Product Guide" ){target=_blank}.

Use caution when generating interferograms for areas with extensive/dense vegetation cover.
Because Sentinel-1 is a C-band sensor, the waves will not penetrate very deeply into vegetation.
Imagery of densely vegetated areas likely represents the top of the canopy rather than the
actual terrain. In addition, vegetated areas tend to have low coherence, because plants can grow
or move from one acquisition to the next.

For step-by-step instructions for searching for, ordering and downloading On Demand InSAR products, visit our [InSAR On Demand!](https://storymaps.arcgis.com/stories/68a8a3253900411185ae9eb6bb5283d3 "InSAR On Demand! StoryMap" ){target=_blank} tutorial.

A Digital Elevation Model (DEM) is required for processing InSAR. ASF uses the
best publicly-available DEM with full coverage of the processing area. To learn more,
refer to our [Digital Elevation Models](dems.md "HyP3 DEM Documentation" ){target=_blank} documentation.

## autoRIFT

[AutoRIFT](https://github.com/leiyangleon/autoRIFT "https://github.com/leiyangleon/autoRIFT" ){target=_blank} produces a velocity map from
observed motion using a feature tracking algorithm developed as part of the 
[NASA MEaSUREs ITS_LIVE](https://its-live.jpl.nasa.gov/ "https://its-live.jpl.nasa.gov" ){target=_blank} project. To learn more,
visit the [ITS_LIVE project website](https://its-live.jpl.nasa.gov/ "https://its-live.jpl.nasa.gov" ){target=_blank}.

A Digital Elevation Model (DEM) is required for autoRIFT processing. ASF uses the
best publicly-available DEM with full coverage of the processing area. To learn more,
refer to our [Digital Elevation Models](dems.md "HyP3 DEM Documentation" ){target=_blank} documentation.
