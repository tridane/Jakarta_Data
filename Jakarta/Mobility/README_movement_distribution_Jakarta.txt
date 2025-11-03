README — Jakarta Mobility Dataset (Facebook “Movement Distribution”)

File Name:
movement_distribution_Jakarta.csv

Data Source:
This dataset originates from the Meta Data for Good – Movement Distribution dataset,
available on the Humanitarian Data Exchange (HDX):
https://data.humdata.org/dataset/movement-distribution
The data represents aggregated mobility patterns inferred from anonymized Facebook users’
location information during the COVID-19 and post-pandemic periods.

Geographic Scope:
Filtered for DKI Jakarta, Indonesia — including:
- Jakarta Barat
- Jakarta Pusat
- Jakarta Selatan
- Jakarta Timur
- Jakarta Utara
- Kepulauan Seribu

Description:
Each record represents a measurement of population mobility for a given district and date,
showing the distribution of distances traveled by users from their home locations.

Columns Description:
gadm_id : Unique GADM identifier for the administrative unit (e.g., IDN.7.3_1 for Jakarta Selatan)
gadm_name : Name of the district (e.g., Jakarta Selatan, Jakarta Utara)
country : ISO3 country code (IDN for Indonesia)
polygon_level : Administrative boundary level (2 = city/district level)
home_to_ping_distance_category : Movement range category:
    0           – Stayed at home
    (0, 10)     – Moved up to 10 km
    [10, 100)   – Moved 10–100 km
    100+        – Moved more than 100 km
distance_category_ping_fraction : Fraction of user pings in that category
ds : Observation date (YYYY-MM-DD)
_source_file : Original source filename from HDX archive

Sorting and Grouping:
1. Date (ds): descending (latest first)
2. District (gadm_name): Jakarta Barat → Jakarta Pusat → Jakarta Selatan → Jakarta Timur → Jakarta Utara → Kepulauan Seribu
3. Distance Category (home_to_ping_distance_category): 0 → (0, 10) → [10, 100) → 100+

Data Coverage:
- Temporal Range: December 2022 – October 2025
- Frequency: Daily (aggregated per district per day)
- Spatial Level: District level within DKI Jakarta

Notes:
- All data are aggregated and privacy-preserving.
- Units are fractions (not absolute counts).
- The dataset reflects relative movement intensity.
