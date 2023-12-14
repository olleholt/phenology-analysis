# phenology-analysis

Author: Olivia Holt note: from eds 223 course in the MEDS program at UCSB

# Overview

Phenology is the timing of life history events. Important phenological events for plants involve the growth of leaves, flowering, and senescence (death of leaves). Plants species adapt the timing of these events to local climate conditions to ensure successful reproduction. Subsequently, animal species often adapt their phenology to take advantage of food availability. As the climate shifts this synchronization is being thrown out of whack. Shifts in phenology are therefore a common yardstick of understanding how and if ecosystems are adjusting to climate change.

Plant species may employ the following phenological strategies:

-   winter deciduous: lose leaves in the winter, grow new leaves in the spring

-   drought deciduous: lose leaves in the summer when water is limited

-   evergreen: maintain leaves year round

credit: this lab is based on a materials developed by Chris Kibler.

### Tasks

To analyze plant phenology near the Santa Clara River which flows from Santa Clarita to Ventura and investigate the phenology of the following plant communities:

-   riparian forests: grow along the river, dominated by winter deciduous cottonwood and willow trees

-   grasslands: grow in open spaces, dominated by drought deciduous grasses

-   chaparral shrub lands: grow in more arid habitats, dominated by evergreen shrubs

A time series of Landsat imagery and polygons identifying the locations of study sites within each plant community will be used to investigate the phenology of the specified plant communities.

### Data

**Landsat Operational Land Imager (OLI sensor)**

-   8 pre-processed scenes

    -   Level 2 surface reflectance products

    -   erroneous values were set to NA

    -   scale factor set to 100

    -   bands 2-7

    -   dates in filenname

**Study sites**

-   polygons representing sites

    -   study_site: character string with plant type

### Summary of approach

-   Convert spectral relfectance into a measure of vegetation productivity (NDVI)

-   Calulate NDVI throughout the year

-   Summarize NDVI values within vegetation communities

```{=html}
<!-- -->
```
-   Visualize changes in NDVI within vegetation communities

EDS223-assignment3

│ README.md

│ phenology-analysis.Rmd

│

└───data

│ landsat_20180815.tif

│ landsat_20181018.tif

\| landsat_20181103.tif

\| landsat_20190122.tif

\| landsat_20190223.tif

\| landsat_20190412.tif

\| landsat_20190701.tif

\| landsat_20180612.tif

│

\| study_sites.dbf

\| study_sites.prj

\| study_sites.shp

\| study_sites.shx
