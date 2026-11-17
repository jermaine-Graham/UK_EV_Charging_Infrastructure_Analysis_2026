UK EV Charging Infrastructure Analysis (2026)

## Interactive Tableau Dashboard
Explore the live interactive dashboard on Tableau Public:
**[View Live Interactive Dashboard on Tableau Public](https://public.tableau.com/authoring/UKevChargingInfrastructureAnalysis2026/June2026DftCPO#1)**

![UK EV Charging Infrastructure Tableau Dashboard](tableau_dashboard_preview)


## Project Overview
An interactive Excel and Google Sheets commercial analysis of public electric vehicle (EV) charging device deployment across 361 UK Local Authorities** (January 2026 – July 2026), built using official Department for Transport (DfT) statistical data (`EVCI0102`).

This project demonstrates end-to-end spreadsheet modelling, automated KPI aggregation, dynamic lookup tools, and exception/data-anomaly handling suitable for automotive and fleet operations reporting.

## Key Features & Spreadsheet Architecture

### 1. `Executive_Summary` (KPI Dashboard & Interactive Lookup)
* **National Totals Summary (`SUMIFS`):** Aggregates total EV chargers, rapid 50kW+ chargers, and rapid charger share (%) across **England**, **Wales**, **Scotland**, and **Northern Ireland** as of 1 July 2026.
* **Local Authority Lookup Tool (`XLOOKUP` & `IFERROR`):** Interactive dropdown selector allowing stakeholders to query any of the 361 UK councils to retrieve its ONS code, July 2026 charger count, net quarterly change (Apr–Jul 2026), and percentage growth rate with built-in zero-division error handling.

### 2. `Pivot_Analysis` (Multi-Dimensional Reporting)
* **Quarterly Charger Growth by Nation:** Cross-tabulated Pivot Table tracking regional infrastructure expansion across Q1, Q2, and Q3 2026.
* **Rapid 50kW+ Density Ranking:** Sorted Pivot Table ranking all 361 local authorities by rapid charging availability per 100,000 population.

### 3. `Clean_Data` (Structured & Standardised Dataset)
* Cleaned and standardised 4,332-row vertical dataset derived from the DfT machine-readable extract (`EVCI0102e`).
* Engineered a dynamic `Nation` classification column using nested `IFS` and `LEFT` string functions mapped to ONS local authority prefixes (`E`, `W`, `S`, `N`).

## Technical Skills Demonstrated
* **Advanced Formulas:** `XLOOKUP`, `SUMIFS`, `IFS`, `IFERROR`, `LEFT`, `DATE`
* **Data Validation & UX:** Dynamic range-based dropdown lists, locked cell references (`$`), and executive number/percentage formatting
* **Data Summarisation:** Multi-filter Pivot Tables with custom sorting and calculated aggregations
* **Data Governance & Audit Notes:** Documented quarterly reporting variances, including the June 2026 Charge Point Operator (CPO) data cleanup (~1,270 decommissioned/reclassified devices).

## Data Source
* **Source:** UK Department for Transport (DfT) — *Electric Vehicle Public Charging Infrastructure Statistics (`EVCI0102`)*
* **Coverage:** 361 UK Local Authorities (England, Wales, Scotland, Northern Ireland)
* **Reporting Dates:** 1 January 2026, 1 April 2026, 1 July 2026
