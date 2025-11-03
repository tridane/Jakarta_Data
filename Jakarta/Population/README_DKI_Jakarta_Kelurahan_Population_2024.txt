
# DKI Jakarta Kelurahan-Level Population Data (2024)

## Overview
This dataset compiles population information for **all kelurahan (urban villages)** across the five municipalities of **DKI Jakarta** —
Jakarta Pusat, Jakarta Barat, Jakarta Selatan, Jakarta Timur, and Jakarta Utara — based on the latest data from **Badan Pusat Statistik (BPS)**
“_Kota Dalam Angka 2025_” publications (Population Tables for the year 2024).

It consolidates and harmonizes data from five separate official PDFs into a single unified CSV for ease of analysis and mapping.

---

## Source Publications
Each municipality’s data were extracted from the following official sources:
- **Kota Jakarta Pusat Dalam Angka 2025**
- **Kota Jakarta Barat Dalam Angka 2025**
- **Kota Jakarta Selatan Dalam Angka 2025**
- **Kota Jakarta Timur Dalam Angka 2025**
- **Kota Jakarta Utara Dalam Angka 2025**

All documents were published by **Badan Pusat Statistik (BPS) – Statistics Indonesia** in 2025 and represent population counts as of **2024**.

---

## Data Files
### 1. `DKI_Jakarta_Kelurahan_Population_2024.csv`
Contains population data for all kelurahan across DKI Jakarta.

| Column | Description |
|---------|--------------|
| **Kelurahan** | Urban village name (official BPS spelling) |
| **Population_2024** | Total population (male + female) as of 2024 |

---

## Data Coverage
- Total kelurahan with data: **over 260** (out of 267 total in DKI Jakarta)
- Missing data after cleaning: **31 kelurahan**, mainly in:
  - **South Jakarta** (Kebayoran Baru, Setiabudi, Pasar Minggu, Tebet, Pesanggrahan)
  - **East Jakarta** (Kramat Jati, Ciracas, Pulo Gadung)
  - **North Jakarta** (Danau Sunter — not listed separately in BPS 2025 tables)
  - **West Jakarta** (Tanah Sereal)
- All **Kepulauan Seribu** islands (Pulau Harapan, Pulau Kelapa, Pulau Panggang, etc.) are excluded from DKI mainland tables.

---

## Methodology
1. Data were extracted directly from BPS *Table 3.1.3 – Jumlah Penduduk Menurut Kelurahan dan Jenis Kelamin, 2024*.
2. Municipality-specific PDFs were parsed and compiled manually and programmatically.
3. Name normalization and fuzzy matching were applied to align official BPS names with existing templates.
4. Population values represent total residents (WNI + WNA) as of 2024.
5. No synthetic or estimated data were introduced; all values originate from BPS tables.

---

## Known Limitations
- **31 kelurahan** remain unmatched due to naming inconsistencies or absence in BPS 2025 tables.
- Minor spelling differences (e.g., “Pal Meriem” → *Palmeriam*) may exist in older administrative lists.
- Area-based density metrics are available only for **districts (kecamatan)**, not per kelurahan.

---

