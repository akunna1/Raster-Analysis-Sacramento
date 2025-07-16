# Raster-Analysis-Sacramento

## Overview

This project analyzes the relationship between vegetation health and socio-economic factors in Sacramento County, California, focusing on NDVI (Normalized Difference Vegetation Index) and household income.

---

## Purpose

To examine how vegetation health, measured by NDVI derived from Landsat satellite imagery, correlates with socio-economic status, specifically the percentage of households earning less than \$35,000 annually, across Sacramento County census tracts.

---

## Tools & Technologies

* **R** (dplyr, tidyverse, tidyr, sf, tidycensus)
* **ArcGIS Pro**
* **Microsoft Excel**

---

## Methodology

1. **NDVI Calculation:**

   * Combined the red and near-infrared bands of Landsat multispectral satellite imagery in ArcGIS Pro.
   * Calculated NDVI to assess vegetation density and health; higher values indicate healthier vegetation.

2. **Socio-Economic Data Integration:**

   * Retrieved 2019 5-year ACS income data using the tidycensus package in R.
   * Computed the percentage of households with incomes below \$35,000 per census tract.
   * Acquired census tract spatial boundaries from the Census Bureau’s TIGER/Line data and joined it with income data for spatial visualization.

3. **Zonal Statistics:**

   * Used ArcGIS Pro to perform zonal statistics, calculating mean NDVI values within each census tract.
   * Aggregated vegetation health data at the tract level to enable localized socio-environmental analysis.

4. **Analysis:**

   * Plotted average NDVI against the percentage of low-income households in Excel.
   * Found a low correlation (R² = 0.1605), indicating limited relationship between vegetation health and household income in Sacramento County.

---

## Data Files

* Landsat satellite imagery bands (red and near-infrared)
* Census tract shapefiles (TIGER/Line)
* ACS income datasets (2019 5-year estimates)
* Resulting NDVI rasters and zonal statistics outputs

---

## Conclusion

The study suggests that vegetation health, as represented by NDVI, is not strongly dependent on household income levels within Sacramento County census tracts, providing insights into the complex socio-environmental dynamics in urban areas.

---

Feel free to explore the code and data files to reproduce or expand upon this analysis.
