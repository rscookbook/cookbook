# GEMx Mission Overview

## Mission Purpose
GEMx (Geological Earth Mapping Experiment) is a joint effort by NASA and the USGS, funded through the USGS Earth Mapping Resources Initiative (Earth MRI). The mission aims to map critical mineral resources in the Western U.S., especially in arid and semi-arid regions. It also serves as a technology and data precursor for NASA’s planned Surface Biology and Geology (SBG) mission, helping build high-resolution, spectrally rich datasets over regional scales.

## Mission Details & Capabilities
- **Timeframe**: Active mission, multiple deployments from 2023 through at least 2025.
- **Study Area**: Western U.S.—notably California, Nevada, Arizona, Oregon, New Mexico—focusing on arid to semi-arid landscapes.
- **Platforms & Altitude**: Flights are undertaken from high-altitude aircraft (NASA’s ER-2 and also Gulfstream V) at ~65,000 ft (≈20 km altitude), which allows wide swath and high-altitude coverage while preserving detail.
- **Sensors**:
  - MASTER (MODIS/ASTER Airborne Simulator)
  - AVIRIS (Airborne Visible/Infrared Imaging Spectrometer)
  - HyTES (Hyperspectral Thermal Emission Spectrometer)
- **Spectral & Spatial Resolution**: MASTER data have ~50 spectral bands spanning visible through thermal infrared (~0.460 to ~12.88 μm) with ~50-meter spatial resolution. Derived Level-2 products include emissivity in several thermal IR bands and land surface temperature.

## Data Access
- **Data Products**: For example, the Spring 2024 dataset includes Level-1B (L1B) calibrated radiance in 50 bands and Level-2 (L2) products (emissivity, land surface temperature) for many flight tracks.
- **File Formats**: L1B data are provided in HDF-4 format. L2 products are delivered in ENVI raster files, KMZ format, PNG/JPEG browse images.
- **Metadata & Ancillaries**: Flight paths, instrument configuration, spectral band calibration, browse images, quality assessment information are also included.
- **Archive & Access Portals**: Data are available via NASA’s Earthdata / ORNL DAAC (Oak Ridge National Lab Distributed Active Archive Center), and through campaign listings in NASA’s Airborne Science Program and USGS Earth MRI.

## What to Know Before You Use F-SAR Data
- **Preprocessing Needs:** Need to handle calibration, atmospheric correction, possible georeferencing. Thermal bands tend to be more difficult.
- **Sensor Differences:** Multi-instrument datasets (MASTER, AVIRIS, HyTES). Each has different spectral coverage, noise levels, and characteristics; integrating across sensors may require care.
- **Data Volume & Size:** Large number of flight tracks, big files (L1B especially). Browse images help but analyses will require substantial computing resources.
- **Spatial & Temporal Coverage Limits:** Not continuous; limited to specific flights / seasons. If doing time-series work, must check date & flight availability.
- **Interpretation of Mineral Signatures:** Mapping mineralogy from spectral data requires domain knowledge (spectroscopy, mineral alteration, reflectance/emissivity spectral interpretation). Ground truth / validation often needed.

## Summary Table

| **Aspect**              | **Key Points**                                                                                      |
|---------------------|-------------------------------------------------------------------------------------------------|
| Purpose             | Map mineral resources in Western U.S.; support USGS Earth MRI and serve as a precursor to NASA’s Surface Biology & Geology (SBG) mission                              |
| Timeframe | Campaign-based, flights ongoing since 2023 |
| Platform         | NASA ER-2 and Gulfstream V aircraft (high-altitude, ~20 km)              |
| Sensors         | MASTER (visible–TIR, 50 bands), AVIRIS (VNIR/SWIR hyperspectral), HyTES (TIR hyperspectral)                     |
| Spectral Range         | ~0.46 – 12.88 μm (VNIR–SWIR–TIR coverage, depending on sensor)                     |
| Spatial Resolution         | ~50 m (MASTER); varies for AVIRIS/HyTES                    |
| Data Products         | L1B calibrated radiance (HDF-4), L2 emissivity & land surface temperature (ENVI, KMZ, PNG/JPEG browse)                    |
| Coverage         | Western U.S. (CA, NV, AZ, OR, NM) – arid/semi-arid regions                     |
| Access         | Publicly available through NASA ORNL DAAC & Earthdata portals                     |
| Considerations         | Multi-sensor integration required; large data volumes; limited temporal coverage; spectral expertise needed for mineral mapping                     |


And there you have it, the basics of the GEMx mission!


