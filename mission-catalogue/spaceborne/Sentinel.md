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
| Sentinel-3            | Ocean & land monitoring| OLCI, SLSTR, SRAL             | 300 m – 1 km| SST, ocean color, altimetry             |
| Sentinel-4            | Atmosphere (air quality)| UVN spectrometer (geo)             | ~8 km (geo footprint)| Trace gas monitoring             |
| Sentinel-5P            | Atmosphere (TROPOMI)| UVN spectrometer             | 3.5 × 7 km| Monitoring NO₂, O₃, CH₄, SO₂ levels             |
| Sentinel-6            | Ocean topography| Poseidon-4 altimeter, radiometer             | ~cm vertical precision| Sea level rise, ocean currents             |

The Sentinel series is one of the most comprehensive EO fleets ever launched, and learning to work with its datasets (SAR, optical, atmospheric, oceanic) is essential for modern remote sensing research. Check out our forum to submit questions or comments regarding Sentinel!
