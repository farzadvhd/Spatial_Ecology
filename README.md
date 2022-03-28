# Aim of the the project:

1. Calculating landcover distribution in our wetlands based on 10 m landcover map of Sweden
2. Open water and flooded vegetation extraction in one of our wetlands.
## Calculating landcover distribution
we use two different layer:
1. [National landcover map of Sweden in 10m resolution](https://www.swedishepa.se/State-of-the-environment/Maps-and-map-services/National-Land-Cover-Database/)
2. [vector layer of Ramsar sites in Sweden](https://rsis.ramsar.org/ris-search/?f[0]=regionCountry_en_ss%3ASweden)

## Open water and flooded vegetation extraction


### Open water extraction
- Layers: SAR intensity sentinel-1 image. 
data source: [Google Earth Engine](https://code.earthengine.google.com)
we use thresholding method to extract open water from S1 layer 
### Flooded vegetation extraction by using unsupervised Kmean classification
- Layers: 1. Coherence layer
          2. slope layer (generated from SRTM DEM)
