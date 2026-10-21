# Colony and inshore comparisons of trace elements and stable isotopes

Code and data for manuscript MPB-D-26-02679.

## Contents

- `data/`
  - `all_data_wide.RDS`: trace element and stable isotope data
  - `icelandic_data.xlsx`: Icelandic data
  - `locations.xlsx`: sampling locations for both the Canadian and Icelandic birds (used for the map)
- `scripts/`
  - `col_bayes.qmd`: Bayesian models (brms), sensitivity analyses, figures and tables
  - `map.qmd`: study area map

## Data availability

The data are archived in Borealis, the Canadian Dataverse Repository:

- Canadian birds: https://doi.org/10.5683/SP3/KDXLHK (Ausems et al., 2026b)
- Icelandic birds: https://doi.org/10.5683/SP4/ULR9MW (Ausems et al., 2026a)

The copies in `data/` are included so the scripts run directly. Please cite the
Borealis datasets when using the data. The terms of use are given on each
dataset's Borealis page.

## Running the analysis

Open `github.Rproj` in RStudio and render the Quarto files in `scripts/`.
The scripts read from `data/` and create `models/`, `output/` and `figures/`
themselves, so those folders are not included in the repository.

Most packages are on CRAN. `rnaturalearthhires` is installed from rOpenSci:

```r
install.packages("rnaturalearthhires", repos = "https://ropensci.r-universe.dev")
```

## License

The code in `scripts/` is released under the MIT License (see `LICENSE`).
The MIT License does not cover the data in `data/`; see Data availability above.

## Contact

Anne Ausems (anneausems@ecos.au.dk)
