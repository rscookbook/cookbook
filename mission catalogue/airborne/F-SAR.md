# DLR F-SAR Overview

## Mission Purpose
F-SAR (Flugzeug-Synthetic Aperture Radar) is an advanced airborne SAR testbed developed by the German Aerospace Center (DLR) to support research and pave the way for future spaceborne SAR technologies. It succeeds DLR’s E-SAR system and is used extensively for developing and evaluating innovations like polarimetric SAR interferometry, tomography, digital beamforming, and more.

## Mission Details & Capabilities
- **Platform**: Installed on a Dornier DO-228-212 research aircraft with antennas mounted near the fuselage.
- **Frequency Bands & Polarimetry**: Operates across X, C, S, L, and P bands, offering fully polarimetric imaging and even single-pass interferometry in X and S bands.
- **Resolution**: Range from sub-meter to meter-level depending on band (e.g., X-band: ~0.3 m range / 0.2 m azimuth; P-band: ~2.25 m range)
- **Operational Altitude & Swath**: Flown at up to 6,000 m altitude, covers off-nadir angles of 25–60°, swath width between 1–5 km.
- **Campaign Examples**: Deployed in Arctic/Permafrost campaigns (e.g., ABoVE 2018–19) alongside AirSWOT for boreal hydrology and subsidence studies.

## Data Access
- **Data Products:** F-SAR offers various processed formats:
-   RGI (Radar Geometry Image)
-   GTC (Geocoded, Terrain-Corrected)
-   INF (Interferometric stacks)

- **File Formats & Tools:**
-   Data often stored in RAT binary format with accompanying `.hdr` files (ENVI-compatible). Tools like GDAL and QGIS support conversion to GeoTIFF.
-   Python support via PyRAT, enabling low-level data access, and the command-line tool fsar_applyLUTs allows radar-slant-range to geocoded grid transformations using LUTs.

- **Request & Access:**
  - F-SAR data is available on request—typically via DLR's EOWEB GeoPortal or by contacting their airborne SAR missions team. Data access agreements apply.

## What to Know Before You Use F-SAR Data
- **Research-Oriented & Flexible:** It’s an experimental system designed for cutting-edge SAR mode development—not a routine operational mission. Expect varied configurations based on campaign objectives.
- **Complex Data Handling:** Multi-band, polarimetric, and interferometric datasets require advanced processing workflows and specialized tools (e.g., PyRAT, LUT-based geocoding).
- **High Accuracy Requirements:** Precise GNSS/INS navigation enables repeat-pass interferometry with meter-level geolocation accuracy—critical for elevation mapping and forest structure studies.
- **Applications:** Ideal for research in terrain deformation, forest height (Pol-InSAR/TomoSAR), permafrost monitoring, SAR mode development, and satellite mission preparation.

## Summary Table

| **Aspect**              | **Key Points**                                                                                      |
|---------------------|-------------------------------------------------------------------------------------------------|
| Purpose             | Airborne SAR testbed for R&D, innovation, satellite mission prep                              |
| Capabilities | Multi-band (X/C/S/L/P), polarimetric, single-pass interferometry |
| Platform & Coverage         | Dornier DO-228, up to 6000 m, swath 1–5 km, sub-meter resolution              |
| Data Products         | RGI, GTC, INF; RAT & COG formats; support via PyRAT, LUT tools                     |
| Access         | Request-based, contact via DLR, usage agreements required                     |
| Considerations         | Complex, research-focused data; requires technical expertise                     |


Ready to explore? Check out EarthExplorer for browsing, use GEE for analysis-ready workflows, or dive into cloud-based processing via AWS.

