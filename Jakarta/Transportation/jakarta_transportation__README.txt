README - Jakarta Transportation Statistics (2024)
=================================================
Compiled from: Badan Pusat Statistik (BPS) – Statistik Transportasi Provinsi DKI Jakarta 2024 (Volume 17, 2025)

This repository includes three datasets extracted and translated into English from the official BPS publication:
1. land_transportation_english.csv
2. sea_transportation_english.csv
3. air_transportation_english.csv

Each dataset includes both annual and monthly data covering the years 2012–2024 for the province of DKI Jakarta.

=================================================
SECTION 1: LAND TRANSPORTATION
=================================================
README - land_transportation_english.csv
=================================================
Title: Land Transportation Statistics — DKI Jakarta 2024
Source: Badan Pusat Statistik (BPS) – Statistik Transportasi Provinsi DKI Jakarta 2024 (Volume 17, 2025)
Coverage: 2012–2024 (annual and monthly data)
Area: Province of DKI Jakarta (South, East, West, North, Central Jakarta, and Thousand Islands)

Purpose:
This dataset compiles statistics on land-based transportation infrastructure and mobility in DKI Jakarta,
including roads, vehicles, public transport, and railways. It consolidates multiple tables and appendices
from the official BPS report.

-------------------------------------------------
Data Structure
-------------------------------------------------
Columns:
- Mode: Always “Land”
- Category: Type of transportation or infrastructure (e.g., Roads, Vehicles, TransJakarta, MRT Jakarta, Licensing)
- Subcategory: Specific grouping (e.g., “South Jakarta”, “Corridor 1 Blok M–Kota”, “SIM C”)
- Metric: What the row measures (e.g., “Registered vehicles”, “Monthly passengers”, “Issued licenses”)
- Unit: Measurement unit (e.g., unit, km, people, ton, licenses)
- Year: Year of observation (2012–2024)
- Month: Month (if applicable; blank for annual data)
- Value: Numeric value (no commas or thousand separators)
- Notes: Table source or description from the BPS report
- Source: Official citation of the publication

-------------------------------------------------
Contents Overview
-------------------------------------------------
1. Vehicles (Tabel 2.1)
   - Registered motor vehicles by type (Passenger Cars, Buses, Trucks, Motorcycles, Total), 2022–2024

2. Roads (Tabel 2.2, Lampiran 1–2)
   - Road length by city and condition (Good, Fair, Lightly Damaged, Heavily Damaged), 2024
   - Road length by jurisdiction (South, East, West, North, Central Jakarta, Thousand Islands)
   - Total: 6,504.71 km (2024)

3. Public Transport Fleets (Tabel 2.3–2.4, Gambar 2.4)
   - Buses by operator and class (large, medium, small)
   - Bajaj & Kancil (three-wheelers) 2019–2024
   - Other fleets: Taxi, Intercity Bus (AKAP), Tourist Bus, Goods Vehicles 2023–2024

4. TransJakarta (Tabel 2.5)
   - Passengers by corridor (Corridor 1–14 + Non-corridor), 2023–2024

5. Rail Transport
   - Intercity Train: Monthly passengers 2023–2024 (Lampiran 7)
   - Rail Freight: Monthly cargo by commodity 2024 (Lampiran 8)
   - KRL Commuter Line: Daily trips by route 2022–2024; monthly passengers 2023–2024; fleet additions 2012–2024
   - MRT Jakarta: Monthly passengers 2023–2024 (Tabel 2.8)
   - LRT Jakarta: Monthly passengers 2023–2024 (Tabel 2.9)

6. Licensing (Lampiran 5–6)
   - Issued driving licenses (SIM) by type and year (2019–2023)
   - Monthly breakdown for 2023 by license category (A, B, C, D)

Notes:
All figures are official data from PT Transportasi Jakarta, PT KAI, and Dinas Perhubungan DKI Jakarta.
Units are standardized for analysis (no thousands separators).


=================================================
SECTION 2: SEA TRANSPORTATION
=================================================
README - sea_transportation_english.csv
=================================================
Title: Sea Transportation Statistics — DKI Jakarta 2024
Source: Badan Pusat Statistik (BPS) – Statistik Transportasi Provinsi DKI Jakarta 2024 (Volume 17, 2025)
Coverage: 2018–2024 (annual and monthly data)
Area: Port of Tanjung Priok, DKI Jakarta

Purpose:
This dataset summarizes maritime transport activities in DKI Jakarta, focusing on ship traffic, passenger
flows, and cargo handled through the Port of Tanjung Priok.

-------------------------------------------------
Data Structure
-------------------------------------------------
Columns:
- Mode: Always “Sea”
- Category: Transport or port category (“Tanjung Priok”)
- Subcategory: Passenger, Inter-Island, or International cargo
- Metric: Type of measurement (e.g., “Vessels berthed”, “Cargo unload”, “Cargo load”)
- Unit: Measurement unit (ships, people, ton)
- Year: Year of observation (2018–2024)
- Month: Month (for monthly data only)
- Value: Numeric value
- Notes: Original table/figure reference
- Source: BPS Publication citation

-------------------------------------------------
Contents Overview
-------------------------------------------------
1. Ships (Gambar 3.1)
   - Total vessels berthed at Tanjung Priok, 2018–2024

2. Passengers (Tabel 3.1, Lampiran 11)
   - Annual and monthly passenger data (Arrivals and Departures), 2020–2024
   - Monthly 2024 breakdown (January–December)

3. Cargo (Tabel 3.2, Lampiran 12)
   - Cargo volumes by route and flow: Inter-Island (Domestic) and International (Foreign)
   - Split by Unload and Load
   - Annual 2020–2024; Monthly breakdown for 2024

Notes:
Data sourced from PT Pelabuhan Indonesia II (Persero), Tanjung Priok Branch.
Cargo includes both domestic and international trade.


=================================================
SECTION 3: AIR TRANSPORTATION
=================================================
README - air_transportation_english.csv
=================================================
Title: Air Transportation Statistics — DKI Jakarta 2024
Source: Badan Pusat Statistik (BPS) – Statistik Transportasi Provinsi DKI Jakarta 2024 (Volume 17, 2025)
Coverage: 2020–2024 (annual and monthly data)
Area: Halim Perdanakusuma Airport, East Jakarta

Purpose:
This dataset provides flight, passenger, and air cargo statistics for Jakarta’s domestic and international
air transport handled through Halim Perdanakusuma Airport.

-------------------------------------------------
Data Structure
-------------------------------------------------
Columns:
- Mode: Always “Air”
- Category: Transport mode (“Halim Perdanakusuma”)
- Subcategory: Flights, Passengers, Cargo (Domestic / International)
- Metric: Type of data (e.g., “Total flights”, “Arrivals”, “Outbound cargo”)
- Unit: Measurement unit (trips, people, kg)
- Year: Observation year (2020–2024)
- Month: Month (for monthly data only)
- Value: Numeric value
- Notes: Reference to source table
- Source: BPS Publication citation

-------------------------------------------------
Contents Overview
-------------------------------------------------
1. Flights (Tabel 4.1, Gambar 4.1, Lampiran 13)
   - Annual total flights (2020–2024)
   - Domestic vs International flights (Arrivals / Departures)
   - Monthly 2024 flight breakdown

2. Passengers (Tabel 4.2, Gambar 4.2, Lampiran 14)
   - Annual passengers by domestic/international and direction
   - Monthly data (2024): arrivals and departures for each category

3. Cargo (Tabel 4.3, Lampiran 15)
   - Annual and monthly cargo tonnage (2020–2024)
   - Domestic (Inbound/Outbound) and International (Import/Export)

Notes:
All data sourced from PT Angkasa Pura II, Halim Perdanakusuma Airport.
2024 includes full monthly breakdown of flights, passengers, and cargo.

