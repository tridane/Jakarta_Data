
# DKI Jakarta District Population Data (2024)

## Overview
This dataset consolidates population statistics for **all districts (kecamatan)** within the five municipalities of **DKI Jakarta** — Jakarta Pusat, Jakarta Barat, Jakarta Selatan, Jakarta Timur, and Jakarta Utara — based on data from *Badan Pusat Statistik (BPS) Kota Administrasi* publications titled **“Kota Dalam Angka 2025”**.

The data represents the most recent (2024) administrative demographic figures available for each district.

---

## Source Files
Each municipality’s data was extracted from the following BPS publications:
- *Kota Jakarta Pusat Dalam Angka 2025*
- *Kota Jakarta Barat Dalam Angka 2025*
- *Kota Jakarta Selatan Dalam Angka 2025*
- *Kota Jakarta Timur Dalam Angka 2025*
- *Kota Jakarta Utara Dalam Angka 2025*

All publications were released by **BPS-Statistics Indonesia (Badan Pusat Statistik)**.

---

## Data Description

| Column | Description |
|---------|--------------|
| **Municipality** | Administrative city/region (e.g., Jakarta Selatan) |
| **District** | Sub-administrative district (*kecamatan*) within the municipality |
| **Population_2024** | Total population of the district in 2024 |
| **Growth_Rate_2020_2024_%** | Annual population growth rate from 2020 to 2024 (%) |
| **Share_of_Total_%** | Percentage of district’s population relative to total municipality population |
| **Density_per_km2** | Population density (people per square kilometer) |
| **Sex_Ratio_M_per_100_F** | Number of males per 100 females in the population |

---

## Notes
- The dataset aggregates verified BPS table “3.1.1” data for each city’s “Population by District (2024)”.
- Some districts have missing values (`None`) where BPS did not publish data for growth rates or ratios.
- Totals are included for each municipality.

---

## File Details
**Filename:** `DKI_Jakarta_District_Population_2024.csv`  
**Format:** Comma-separated values (UTF-8 encoded)  
**Total Entries:** 55 rows (including municipal totals)

---

