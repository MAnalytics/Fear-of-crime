# Fear of Crime and Institutional Preferences in a Hybrid Security Environment: Replication Data

This repository contains the replication data and codebook supporting a study of fear of crime and institutional trust (formal police vs. informal vigilante security) among residents of five contiguous Local Government Areas in metropolitan Lagos, Nigeria.

## Study Summary

The study examines:
1. The determinants of trust in formal police and informal vigilante security providers (H1, H2)
2. Whether fear of crime mediates the relationship between victimisation, environmental conditions, social context, and institutional trust (H3)

Data were collected via a randomised household survey (N = 665) combined with systematic environmental observation at each interview location.

## Files

| File | Description |
|---|---|
| `Paper2_AnalysisData_N666_Narrow.csv` | Analytic dataset, N = 666 (2 respondents recorded as a non-binary gender category are excluded). Contains only variables retained in at least one final regression model or tested as a mediation treatment in the associated paper — see the codebook for exactly which analysis each variable feeds into. |
| `Paper2_Codebook_Narrow.csv` | Variable-by-variable documentation: description, coding, and the specific table/analysis each variable is used in. |

## Sample

- **N = 668** total completed interviews across five contiguous Lagos LGAs (Shomolu, Mushin, Oshodi–Isolo, Surulere, Lagos Mainland), treated as a single study area.
- **N = 666** analytic sample used throughout this repository (2 respondents excluded for a non-binary gender category).
- A further subset of **N = 616** is used specifically in the regression models reported in the paper (50 respondents are additionally excluded from those models only, due to "not sure" responses on the observed street-lighting item); this restriction does not apply to the full dataset shared here.

## Key Variables

- **Outcome variables:** `police_trust_index` (composite), `vigilante_safe` (single item), `trust_gap` (vigilante_safe − police_trust_index)
- **Primary mediator:** `fear_index1` (Affective Fear Index — worry-based)
- **Alternative measure:** `fear_index2` (Perceived Risk Index — used for a regression robustness check only)
- **Predictors:** retained victimisation, environmental, social-context, and demographic variables — see codebook for the full list and which model each appears in

Composite indices (`disorder_index`, `collective_index`, `fear_index1`, `fear_index2`, `police_trust_index`) are provided both as pre-computed columns and via their constituent raw items, so derivations can be independently verified.

## Variable Naming Conventions

- Variables ending in `_bin` are binary (0/1) indicators derived from the corresponding raw text/categorical column.
- Variables ending in `_index` are composite scores (row means of their constituent items).
- Multi-select observational fields (e.g., `informal_security`, `activity_node`) are retained in their raw text form alongside their derived binary indicators.

## Data Cleaning Notes

- Raw survey responses were cleaned for whitespace, casing, and delimiter inconsistencies; multi-select fields were parsed into individual binary indicators.
- Reporting-behaviour fields (`reported`, `reported_to`, `nonreport_reason`, and derived categories) are only populated for the subsample of respondents who reported direct victimisation (burglary, theft, or assault) in the preceding 12 months; all other respondents show missing values for these fields by design.

## Methodology

Full survey instrument, sampling design, variable construction, and analytical strategy (stepwise regression, bootstrap mediation) are described in the associated manuscript. This repository provides the data underlying that analysis; it does not include the full survey instrument or raw uncleaned export.

## Citation

*A full citation will be added here once the associated manuscript is published. In the interim, please contact the corresponding author for permission to use this data.*

## License

*[Specify a license, e.g., CC BY 4.0, once decided.]*

## Contact

*[Corresponding author name and email]*
