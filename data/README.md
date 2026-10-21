# Data description

## `all_data_wide.RDS`

Canadian birds (Ausems et al., 2026b; https://doi.org/10.5683/SP3/KDXLHK).
One row per individual (456 birds, sampled 2018–2021).

| Column | Description |
|---|---|
| `ID` | Unique identifier for each individual |
| `year` | Sampling year (equal to hatch year) |
| `source` | Sampling location |
| `Cu`, `Zn`, `As`, `Mn`, `Co`, `Hg`, `V`, `Cd`, `Tl`, `Pb` | Trace element concentrations (µg/g dry weight). Where the matching `_BDT` column is `TRUE`, the value is below the case-specific limit of quantification (LOQ) and the value given is the LOQ |
| `d13C`, `d15N` | Stable isotope values (‰): δ13C relative to VPDB, δ15N relative to atmospheric N2 (air) |
| `stranded` | Whether a bird was stranded or sampled as a nestling. Not used in this paper, but included in the full data set |
| `pool_source` | Pooled sources: either colony or stranding location (inshore/offshore). Not used in this paper, but included in the full data set |
| `Cu_BDT`, `Zn_BDT`, `As_BDT`, `Mn_BDT`, `Co_BDT`, `Hg_BDT`, `V_BDT`, `Cd_BDT`, `Tl_BDT`, `Pb_BDT`, `d13C_BDT`, `d15N_BDT` | Whether a value was censored, i.e. below the LOQ (`TRUE`) or not (`FALSE`) |

## `icelandic_data.xlsx`

Icelandic birds (Ausems et al., 2026a; https://doi.org/10.5683/SP4/ULR9MW).
One row per individual (12 birds).

| Column | Description |
|---|---|
| `ID` | Unique identifier for each individual |
| `V`, `Mn`, `Co`, `Cu`, `Zn`, `As`, `Cd`, `Hg`, `Tl`, `Pb` | Trace element concentrations (µg/g dry weight). Any value reported as `<[value]` is below the case-specific limit of quantification (LOQ), where `[value]` is the LOQ |

## `locations.xlsx`

Sampling locations used for the study area map (`scripts/map.qmd`), for both
the Canadian and Icelandic birds.

| Column | Description |
|---|---|
| `Location` | Name of the sampling location |
| `Country` | Country of the sampling location |
| `Lat` | Latitude (decimal degrees) |
| `Lon` | Longitude (decimal degrees) |
