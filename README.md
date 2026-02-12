# Cantonal-Development-Index-for-Ecuador
Research dataset containing the final database (13 variables + outcome) and basic documentation for reuse and citation.
# Dataset accompanying the paper

**Dataset title:** Cantonal Development Index - Ecuador

This repository contains the final cantonal-level datasets used in the paper:

- **Inputs / explanatory variables**: a cantonal database with **13 indicators** (plus identifiers) for **2010** and **2022**.
- **Outcomes**: the **normalized Cantonal Development Index (IDC\_norm)** and its **quintile/stratum** for 2010 and 2022.

## Files
- `DataBase_2010.xlsx` — cantonal indicators for 2010 (**221** cantons; 3 identifiers + 13 indicators).
- `DataBase_2022.xlsx` — cantonal indicators for 2022 (**221** cantons; 3 identifiers + 13 indicators).
- `IDC Outcomes.xlsx` — outcome variables: `IDC_norm 2010`, `IDC_norm 2022`, and strata.

## How to merge (recommended)
Use the canton identifier to merge:
- `DataBase_2010.xlsx` / `DataBase_2022.xlsx`: variable `CANTON`
- `IDC Outcomes.xlsx`: variable `Canton code`

## Data structure and units
Unless otherwise stated, percentages are expressed in **percentage points** (0–100). Units for a few rate/level variables follow the **original data source**.

---

## Variable dictionary (main datasets: `DataBase_2010.xlsx`, `DataBase_2022.xlsx`)

| Variable | Description |
|---|---|
| `PROVINCIA` | Province name (Ecuador). |
| `CANTON` | Cantonal code (INEC/administrative identifier). |
| `NOMBRE_CANTON` | Canton name. |
| `VAB_PERCAPITAL_CANTONAL` | Cantonal gross value added (GVA) per capita (units as in the original source). |
| `tasa_deanalfabetismo` | Illiteracy rate (share of population that cannot read/write). |
| `Tasadeparticipacionlaboral` | Labor force participation rate. |
| `promedioescolaridad` | Average years of schooling. |
| `tasaprimaria` | Share of population whose highest completed level is primary education (percentage points). |
| `Tasasecundaria` | Share of population whose highest completed level is secondary education (percentage points). |
| `tasasuperior` | Share of population whose highest completed level is tertiary/higher education (percentage points). |
| `porcentajehohareshancinados` | Share of households *without* overcrowding (i.e., 1 − overcrowding rate), in percentage points. |
| `Deficithabitacional` | Housing adequacy indicator (percentage points; higher values indicate fewer/less housing deficits as in the original source). |
| `Viviendaseliminacionbasura` | Share of dwellings with garbage collection / solid-waste disposal service (percentage points). |
| `Camasdispo` | Hospital bed availability rate (beds per population, as reported by the original source). |
| `tasademortalidad` | Mortality rate (deaths per population, as reported by the original source). |
| `Viviendastotalservicios` | Share of dwellings with basic services (percentage points; definition as in the original source). |

---

## Variable dictionary (outcomes file: `IDC Outcomes.xlsx`)

| Variable | Description |
|---|---|
| `Canton code` | Cantonal code (INEC/administrative identifier). Matches `CANTON` in the main datasets. |
| `Province code` | Province administrative code. |
| `Province` | Province name. |
| `Canton` | Canton name. |
| `IDC_norm 2010` | Normalized Cantonal Development Index (IDC) for 2010 (outcome variable used in the paper). |
| `Stratum (2010)` | IDC quintile/stratum for 2010 (1=lowest development, 5=highest), based on the paper’s cutoffs. |
| `IDC_norm 2022` | Normalized Cantonal Development Index (IDC) for 2022 (outcome variable used in the paper). |
| `Stratum (2022)` | IDC quintile/stratum for 2022 (1=lowest development, 5=highest), based on the paper’s cutoffs. |

---

## How to cite
If you use these data, please cite the dataset DOI (recommended):

> **Author(s). (Year). Cantonal Development Index - Ecuador (Version). Zenodo. https://doi.org/DOI**

After connecting this GitHub repository to Zenodo, create a GitHub **Release** (e.g., `v1.0.0`) so Zenodo archives that version and assigns a DOI. Replace `DOI` above with the assigned DOI.

## License
This dataset is licensed under CC BY 4.0. You must give appropriate credit.

## Contact
For questions, please open an issue in this repository.
