README — Jakarta Kelurahan Monthly Climate Dataset (ERA5-Land 2015–2024)
=========================================================================

Overview
--------
This dataset provides monthly average temperature, total rainfall, and relative humidity 
for each *kelurahan* (urban village) in Jakarta mainland. It was derived using ERA5-Land 
Daily Aggregated reanalysis data from the European Centre for Medium-Range Weather Forecasts (ECMWF), 
processed in Google Earth Engine (GEE).

Data Coverage
--------------
Variable         | Description                               | Units | Source Band                  | Aggregation
-----------------|-------------------------------------------|--------|-------------------------------|-------------
temp_c           | Mean 2-meter air temperature              | °C     | temperature_2m                | Monthly mean
rainfall_mm      | Total monthly rainfall                    | mm     | total_precipitation_sum       | Monthly sum
humidity_pct     | Mean relative humidity                    | %      | Derived from temp & dewpoint  | Monthly mean

Spatial Extent
---------------
- Region: Jakarta Mainland, Indonesia
- Number of kelurahan: 262
- Resolution: ~9 km (ERA5-Land grid)
- Method: Mean value of each variable per kelurahan polygon using zonal reduction (reduceRegions)

Temporal Coverage
-----------------
- Years: 2015–2024
- Months: January (1) through December (12)
- Temporal Resolution: Monthly
- Time Zone: UTC (ERA5 native time)

Column Descriptions
--------------------
Column        | Type     | Description
--------------|----------|-----------------------------------------
kelurahan     | String   | Name of the kelurahan (NAME_4 field)
year          | Integer  | Year of observation (2015–2024)
month         | Integer  | Month of year (1=Jan, ..., 12=Dec)
temp_c        | Float    | Mean air temperature (°C)
rainfall_mm   | Float    | Total rainfall (mm)
humidity_pct  | Float    | Mean relative humidity (%)

Processing Workflow
-------------------
1. Jakarta kelurahan shapefile and template CSV loaded into Google Earth Engine.
2. Normalized kelurahan names (uppercased, trimmed, punctuation removed) for matching.
3. Filtered ERA5-Land daily data to monthly periods (2015–2024).
4. Computed for each kelurahan and month:
   - Mean temperature from `temperature_2m`
   - Dewpoint from `dewpoint_temperature_2m`
   - Rainfall sum from `total_precipitation_sum` × 1000 (m→mm)
   - Relative humidity via Magnus formula: RH = 100 * (es(Td)/es(T))
5. Reduced each variable spatially using mean per polygon (`reduceRegions`).
6. Exported as CSV to Google Drive.

File Details
-------------
File name: jakarta_kelurahan_monthly_era5land_FULL_2015_2024.csv
Format: CSV (comma-separated)
Rows: ~31,000 (262 kelurahan × 10 years × 12 months)
Columns: kelurahan, year, month, temp_c, rainfall_mm, humidity_pct

Attribution
------------
- Data Source: ECMWF ERA5-Land via Google Earth Engine
- Processing: Google Earth Engine (GEE)
- Date generated: October 2025
