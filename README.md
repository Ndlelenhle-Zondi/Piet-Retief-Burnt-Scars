# Piet-Retief-Burnt-Scars
Automated Sentinel-2 L2A pipeline using odc-stac and Planetary Computer to map wildfire burn severity (dNBR) and damaged hectares across forestry plantations in Mkhondo / Piet Retief, Mpumalanga.

Suggested Repository Topics / Tags
sentinel-2 • earth-observation • planetary-computer • stac • wildfire • burn-severity • dnbr • gis • qgis • geopandas • forestry • mpumalanga

Project Summary (for your README.md Overview)
Wildfire Burn Severity & Compartment Impact Pipeline (Mkhondo / Piet Retief)

This repository provides an end-to-end Python and STAC geospatial pipeline designed to monitor and quantify wildfire burn severity across commercial timber plantations (Pinus & Eucalyptus) in the Piet Retief / Mkhondo corridor of Mpumalanga, South Africa.

Core Pipeline Features:

Satellite Ingestion: Queries Microsoft Planetary Computer STAC for pre- and post-fire Sentinel-2 L2A surface reflectance scenes.

Metric Band Processing: Streams narrow Near-Infrared (B8A) and Shortwave-Infrared (B12) bands reprojected to WGS 84 / UTM Zone 36S (EPSG:32736) at 20 m resolution.

Spectral Change Detection: Calculates pre- and post-fire Normalized Burn Ratio (NBR) and differenced NBR (ΔNBR).

Severity Classification: Applies standard USGS FireMon thresholds (Unburned, Low, Moderate, High) and computes damaged surface area in hectares.

GIS-Ready Deliverables: Exports continuous floating-point GeoTIFFs, discrete classified rasters with embedded color tables, and vectorized ESRI Shapefiles for analysis and cartographic display in QGIS
