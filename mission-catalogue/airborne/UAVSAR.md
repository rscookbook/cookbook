# UAVSAR Mission Overview

## Mission Purpose
UAVSAR is a NASA airborne L-band synthetic aperture radar system designed to test and advance SAR techniques, provide targeted high-resolution datasets, and prepare for future spaceborne radar missions. It’s especially well known for repeat-pass InSAR measurements, enabling the study of surface deformation, earthquakes, volcanoes, ice dynamics, and vegetation structure.

## Mission Details & Capabilities
- **Platform**: Mounted on NASA’s Gulfstream-III aircraft (tail #N992NA), with a precision autopilot to ensure highly repeatable flight tracks.
- **Frequency & Polarimetry:**: Operates at L-band (~1.26 GHz), fully polarimetric (HH, HV, VH, VV).
- **Imaging Modes:**:
  - PolSAR (polarimetric SAR)
  - Repeat-pass InSAR for deformation
  - Single-pass along-track interferometry (when paired with JPL’s AirMOSS)
- **Resolution & Swath**: ~1–7 m resolution, ~20 km swath.
- **Geolocation Accuracy:** Precise autopilot and GPS/INS enable repeat-pass track accuracy better than 10 m.
- **Campaigns:** UAVSAR has flown extensively across the U.S. and internationally for tectonics, cryosphere, wetlands, and disaster response studies (e.g., earthquakes in Haiti, ice sheet mapping in Greenland, permafrost in Alaska).

## Data Access
- **NASA UAVSAR Portal:** uavsar.jpl.nasa.gov (search by region, flight line, date, product type).
- **Products**:
  - SLC (Single Look Complex)
  - GRD (Geocoded Radar Data)
  - INSAR (Interferograms)
  - POLSAR (Polarimetric stacks)
- **File Formats**: CEOS standard format, with annotation files (.ann), binary data, and KMZ quicklooks.
- **Access Requirements:** Publicly available; some datasets also archived via NASA DAACs (e.g., ASF DAAC for InSAR).

## What to Know Before You Use F-SAR Data
- **Large Data Volumes:** Single flight line products can be several GB. Plan storage and processing power accordingly.
- **Specialized Formats:** CEOS format may require tools like GDAL, PolSARpro, or custom Python scripts to parse. Annotation files (.ann) are essential for metadata.
- **Repeat-Pass Geometry:** For interferometry, precise co-registration is critical. Many interferogram products are pre-computed, but custom processing may be needed.
- **Not Global Coverage:** Campaign-based—data exist only for specific regions of interest.
- **Applications:** Earthquakes, volcanoes, subsidence, permafrost thaw, glacier motion, vegetation biophysics, disaster response (e.g., floods, oil spills).

## Summary Table

| **Aspect**              | **Key Points**                                                                                      |
|---------------------|-------------------------------------------------------------------------------------------------|
| Purpose             | Airborne L-band SAR for deformation, ecosystems, disaster response, and spaceborne SAR prep                              |
| Platform | NASA Gulfstream-III aircraft with precision autopilot |
| Frequency         | L-band (~1.26 GHz), fully polarimetric              |
|Resolution/Swath         | ~1–7 m, ~20 km                     |
| Data Products         | SLC, GRD, InSAR interferograms, PolSAR products                     |
| Spatial Resolution         | ~50 m (MASTER); varies for AVIRIS/HyTES                    |
| Access         | UAVSAR data portal (public), ASF DAAC for some products                    |
| Considerations         | Campaign-based (not global), large files, CEOS format, requires advanced SAR processing knowledge                     |


UAVSAR is one of the most important bridges between airborne science and space missions like NISAR, providing both operational datasets and a testbed for radar technology and science methods. Check out some other important airborne missions in our catalogue!



