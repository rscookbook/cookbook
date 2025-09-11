# Landsat Mission Overview

## Mission Purpose
Landsat, a joint NASA/USGS satellite program, stands as the longest-running continuous record of Earth’s land surfaces, dating back to the 1972 launch of Landsat 1. Initially designed to monitor natural resources, it now plays an essential role in observing deforestation, agriculture, urban expansion, glacier retreat, wildfires, and land cover change.

## Mission Details
- **Continuity & Coverage**: Landsat satellites have recorded moderate-resolution imagery (visible to thermal) consistently over five decades. The latest, Landsat 9, launched 27 September 2021, continuing this legacy with consistent calibration for seamless comparisons across time.
- **Orbital Specs**: Generally, Landsat operates in a sun-synchronous orbit (~705 km altitude) with a 16-day revisit cycle, ~185×185 km scene footprint.
- **Instruments by Generation**:
  - The original Multispectral Scanner (MSS) aboard Landsat 1–5 captured key early images and even played a role in establishing the NDVI vegetation index.
  - Thematic Mapper (TM) on Landsat 4–5 offered seven spectral bands at ~30 m resolution.
  - Landsat 8 introduced the Operational Land Imager (OLI) and Thermal Infrared Sensor (TIRS), improving spectral coverage with new bands for cirrus detection and coastal observations, enhanced thermal sensitivity, and precise calibration.

## Data Access
- **Free & Open Access**: All Landsat data (Level-1, Level-2, ARD, Level-3) is available at no charge via USGS portals like EarthExplorer, GloVis, and ESPA, tailored for both GUI and API-driven workflows.
- **Cloud Platforms**:
  - AWS provides Landsat Collection 2 data in STAC format for scalable, on-demand access.
  - Google Earth Engine (GEE) offers seamless Landsat datasets with analytical capabilities and tutorials for NDVI, land change detection, and more.
- **Apps & Viewers**: Tools like AppEEARS, Esri Landsat Explorer, and USGS’s spectral viewers help users explore and subset data via easy interfaces.

## What to Know Before You Use Landsat Data
- **Rich Yet Complex Archive**: Landsat’s multi-sensor history delivers incredible long-term insights—but users must navigate varying spectral bands, sensor calibrations, and processing levels across generations.
- **Preprocessing Needs**: Calibration, cloud masking, and atmospheric corrections are essential—especially for cross-sensor consistency. Leverage ARD or Level-2 products when possible.
- **Applications & Impact**: Landsat data supports agricultural monitoring, environmental change detection, urban planning, ecosystem assessments, disaster response, and more.
- **Legacy & Research Value**: Its archive enables “Earth time‐lapse” analyses—documenting glacier melt, land cover transitions, and fire impacts. For example, Landsat data is pivotal in mapping wildfires and their emissions over time.

## Summary Table

| **Aspect**              | **Key Points**                                                                                      |
|---------------------|-------------------------------------------------------------------------------------------------|
| Purpose             | Global, multi-decadal Earth land observation, resource monitoring                              |
| Satellite & Sensors | From MSS to TM, OLI, TIRS; improvements in spectral and spatial detail |
| Data Access         | Free via USGS (EarthExplorer, ESPA), AWS (STAC), GEE, and various analytical interfaces              |
| Usage Notes         | Sensor continuity, calibration, preprocessing needed for consistent analysis                      |


Ready to explore? Check out EarthExplorer for browsing, use GEE for analysis-ready workflows, or dive into cloud-based processing via AWS.
