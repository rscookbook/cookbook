# UAVSAR Mission Overview

## Mission Purpose
UAVSAR is a NASA airborne L-band synthetic aperture radar system designed to test and advance SAR techniques, provide targeted high-resolution datasets, and prepare for future spaceborne radar missions. It’s especially well known for repeat-pass InSAR measurements, enabling the study of surface deformation, earthquakes, volcanoes, ice dynamics, and vegetation structure.

## Mission Details & Capabilities
- **Platform**: Mounted on NASA’s Gulfstream-III aircraft (tail #N992NA), with a precision autopilot to ensure highly repeatable flight tracks.
- **Frequency & Polarimetry:**: Operates at L-band (~1.26 GHz), fully polarimetric (HH, HV, VH, VV).
- **Imaging Modes:**:
  - PolSAR (polarimetric SAR)
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



