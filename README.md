# Differences in trace element concentrations and stable isotope values among juvenile Leach's storm-petrels (*Hydrobates leucorhous*) from colonies in the North Atlantic

Anne N.M.A. Ausems, Sophie Roy, Alexander L. Bond, Laura Crick, Joshua T.
Cunningham, Erpur S. Hansen, April Hedd, Stephen Hurling, Trevor MacLaurin,
Laura A. McFarlane Tranquilla, Jennifer C. Rock, Robert A. Ronconi, Manon
Sorais, Katharine R. Studholme, Christopher R.E. Ward, Sabina I. Wilhelm,
Sarah N.P. Wong, Glenn T. Crossin

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

### References

Ausems, A.N.M.A., Hurling, S., Bond, A.L., Crick, L., Hansen, E.S., Hedd, A.,
Studholme, K.R., Ronconi, R.A., Crossin, G.T., 2026a. Trace element
concentrations of juvenile fourth secondary feathers of Leach's storm-petrel
from Iceland. https://doi.org/10.5683/SP4/ULR9MW

Ausems, A.N.M.A., Roy, S., Bond, A., Crick, L., Hedd, A., Studholme, K.,
Ronconi, R., Crossin, G., 2026b. Trace element concentrations and stable
isotope values of juvenal fourth secondary feathers of Leach's storm-petrels.
https://doi.org/10.5683/SP3/KDXLHK

## Running the analysis

The analysis was run with R 4.6.1 and Quarto 1.10.18. The exact package
versions are recorded with [renv](https://rstudio.github.io/renv/) in
`renv.lock`.

1. Open `github.Rproj` in RStudio. renv installs itself on first opening.
2. Install the recorded package versions:

   ```r
   renv::restore()
   ```

3. Render the Quarto files in `scripts/`.

The scripts read from `data/` and create `models/`, `output/` and `figures/`
themselves, so those folders are not included in the repository.

## License

The code in `scripts/` is released under the MIT License (see `LICENSE`).
The MIT License does not cover the data in `data/`; see Data availability above.

## Contact

Anne Ausems (anneausems@ecos.au.dk)
