# King County Metro Transit Accessibility

*By Jerome Orille | GEOG 458 | Winter Quarter 2021*

## Project Details

This project is a web map that goes over metro transit accessibility. This topic
is important to me because before COVID-19, I commuted to and from school
everyday. Having access to commuting routes is important for many reasons, which
include saving money, having a healthy work/school schedule and having an
increased ecological footprint. The goal of this project is to assess the state
of metro transportation in King County.

## Methodology

My analysis was done using ArcGIS Pro. The variables I assessed were the following:
- Number of bus stops per census tract
- Population weighted centroids (PWCs) and the distance toward the closest Park and Ride
- Railways in King county
I calculated the number of bus stops per census tract by intersecting the bus stop
points with the census tracts. The PWCs were calculated by using the population field
in the census tract data to find the mean centers. Afterwards, I did a spatial join
to find the closest Park and Ride station (in miles) toward each PWC. The King
County railways were last; I included them to give an idea of where the other
variables are spatially with regards to the railways.

## Findings

Based on looking at the census tracts, the west side of King County has much more
bus stops than the east side overall. I personally can see this; I frequented
the SeaTac light rail often and the light rail only goes through the west side
of King County. However, I noticed that Seattle census tracts tend to be further
away from Park and Ride stations, which I thought was interesting considering
that the majority of railway stations travel through Seattle. The census tracts
in the far east have long railways that go through the region, yet the railways
do not cover enough ground. Most of the metro transportation covers the western
side of King County.

## Data sources

The following data sources are all from [King County Open GIS Data](https://gis-kingcounty.opendata.arcgis.com/).
- [Census Tracts](https://gis-kingcounty.opendata.arcgis.com/datasets/consolidated-demographics-index-for-king-county-census-tracts-demographic-index-area)
- [Transit Stops](https://gis-kingcounty.opendata.arcgis.com/datasets/transit-stops-for-king-county-metro-transitstop-point)
- [Park and Ride Lots](https://gis-kingcounty.opendata.arcgis.com/datasets/king-county-metro-park-and-ride-lots-parkride-point)
- [Railways](https://gis-kingcounty.opendata.arcgis.com/datasets/metro-transportation-network-tnet-in-king-county-for-railway-mode-trans-network-rail-line)

## Libraries

*Styles:*
- Leaflet CSS
- Font Awesome
- Open Sans from Google fonts

*Javascript:*
- Leaflet Javascript (along with Ajax)
- jQuery
- Chroma

## Acknowledgment

I would like to thank Bo Zhao and Tyler McCrea for teaching me this course.
