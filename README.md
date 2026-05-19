# Fuel-Monitoring-Dashboard
Fuel monitoring dashboard for identifying potential monitoring priority areas using terrain, fuels, vegetation structure, and fuel moisture data in the central coast of California.
# Fuel Monitoring Dashboard

This project is an open-source dashboard being developed to help identify potential fuel monitoring priority areas using spatial layers related to terrain, fuels, vegetation structure, and fuel moisture.

## Project goal

The goal of this project is to develop a spatial dashboard that helps explore where terrain conditions, fuel structure, and fuel moisture stress may overlap. These areas may be useful to prioritize for field-based fuel monitoring.

## Current dashboard layers

The current dashboard includes terrain layers derived from a 10 m digital terrain model:

- Study area boundary
- Slope classes
- Aspect classes

## Planned layers

Future versions will include:

- Live Fuel Moisture Content (LFMC), 2016–2022
- Vapor Pressure Deficit (VPD), 2016–2022
- Lagged VPD relationships with LFMC
- Canopy height
- Fuel model or fuelscape data
- Fuel monitoring priority index

## Analysis approach

The final analysis will combine terrain, vegetation structure, fuels, LFMC, and lagged VPD layers into a fuel monitoring priority index.

Because the input layers have different spatial resolutions, the combined analysis will use a common analysis grid. Continuous variables, such as slope, canopy height, LFMC, and VPD, can be resampled or aggregated. Categorical layers, such as aspect classes and fuel model classes, should use nearest neighbor resampling so class values are preserved.

## Open-source direction

The long-term goal is to develop this workflow using open-source tools, including Python, Leafmap, GeoPandas, rasterio, Jupyter, and Voilà. This would allow the workflow to be shared, modified, and expanded without requiring proprietary GIS software.

For this stage, ArcGIS Pro was used for some raster preprocessing and validation, while the dashboard framework is being developed in Python.
