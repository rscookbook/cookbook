# Sentinel Missions (Copernicus Programme) Overview

## Mission Purpose
The Sentinel satellites are the spaceborne backbone of the Copernicus Programme, led by the European Commission and European Space Agency (ESA). They provide free, open-access Earth observation data to support environmental monitoring, climate research, disaster response, land/ocean/atmosphere studies, and operational services for governments, researchers, and industry.

## Mission Details & Fleet
- **Sentinel-1 (C-band SAR):** Radar imaging for all-weather, day/night monitoring. Key applications: land motion (InSAR), sea ice, oil spills, disaster mapping.
- **Sentinel-2 (Optical multispectral):** 13 bands (VNIR + SWIR), 10–60 m resolution. Applications: vegetation, agriculture, forestry, land use/land cover.
- **Sentinel-3 (Ocean & land monitoring):** Instruments for sea surface topography, ocean color, land surface temperature.
- **Sentinel-4 (Atmospheric composition):** Geostationary payload for air quality monitoring (launched as payload on Meteosat Third Generation).
- **Sentinel-5 Precursor (5P) (Atmospheric composition):** Carries TROPOMI, measuring trace gases like NO₂, O₃, CH₄.
- **Sentinel-5 (Future mission):** Full atmospheric composition satellite.
- **Sentinel-6 (Michael Freilich) (Ocean topography):** Successor to Jason altimetry missions, focused on sea level rise.

## Data Access
There are a few different ways to access Sentinel data:
  - **Copernicus Open Access Hub** scihub.copernicus.eu (main ESA portal; includes Sentinel-1, 2, 3, 5P)
  - **Copernicus Data Space Ecosystem** dataspace.copernicus.eu (next-generation portal with APIs, cloud access, processing tools)
  - **NASA Earthdata & Google Earth Engine** host Sentinel products for direct analysis.
  - **Tools:** ESA SNAP Toolbox (Sentinel Application Platform), QGIS, Google Earth Engine, Python libraries

## What to Know Before Working with Sentinel Data
- **Data Volume:** Sentinel-1 and Sentinel-2 datasets are very large (GBs per scene); efficient workflows & cloud tools recommended.
- **Preprocessing:** Some products (esp. Sentinel-1 SAR) require calibration, speckle filtering, terrain correction. Optical data may need atmospheric correction (e.g., Sen2Cor).
- **Naming Conventions:** Filenames contain sensing mode, orbit, tile info — learn to parse for efficient filtering.
- **Temporal Coverage:** Sentinels provide high revisit frequency (e.g., Sentinel-2: 5 days at equator with both satellites; Sentinel-1: 6–12 days depending on orbit).
- **Licensing:** All Sentinel data are **free and open** under the Copernicus data policy.

## Summary Table

| **Sentinel**              | **Research Focus**           | **Key Instruments**              | **Resolution**           | **Applications**              |
|---------------------|----------------------------|---------------------|----------------------------|---------------------|
| Sentinel-1            | C-band SAR (radar)| SAR (VV, VH, HH, HV)             | 5–40 m (depending on mode)| InSAR, land motion, sea ice, floods             |
| Sentinel-2            | Optical multispectral | MSI (13 bands, VNIR–SWIR)             | 10–60 m  | Vegetation, LULC, agriculture             |
| Sentinel-3            | C-band SAR (radar)| SAR (VV, VH, HH, HV)             | 5–40 m (depending on mode)| InSAR, land motion, sea ice, floods             |
| Sentinel-4            | C-band SAR (radar)| SAR (VV, VH, HH, HV)             | 5–40 m (depending on mode)| InSAR, land motion, sea ice, floods             |
| Sentinel-5P            | C-band SAR (radar)| SAR (VV, VH, HH, HV)             | 5–40 m (depending on mode)| InSAR, land motion, sea ice, floods             |
| Sentinel-6            | C-band SAR (radar)| SAR (VV, VH, HH, HV)             | 5–40 m (depending on mode)| InSAR, land motion, sea ice, floods             |


Ready to dive in? Explore the SWOT Data User Handbook, check out the PO.DAAC Cookbook, and join the Earthdata Forum to engage with the SWOT user community.

