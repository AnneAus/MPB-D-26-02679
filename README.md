# Colony and inshore comparisons of trace elements and stable isotopes

Code and data for manuscript MPB-D-26-02679.

## Contents

- `data/`
  - `all_data_wide.RDS`: trace element and stable isotope data
  - `icelandic_data.xlsx`: Icelandic data
  - `locations.xlsx`: sampling locations (used for the map)
- `scripts/`
  - `col_bayes.qmd`: Bayesian models (brms), sensitivity analyses, figures and tables
  - `map.qmd`: study area map

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
The MIT License does not cover the data in `data/`.

## Contact

Anne Ausems (anneausems@ecos.au.dk)
