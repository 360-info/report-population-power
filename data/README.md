# `/data`

## `dependency-ratios-selectedcountries.csv`

Processed data with the number of elderly people in each country over time, as well as the ratios of working (aged 15 to 64) and dependent (other ages) people.

The ratio of dependent people to working people is called the "Dependency ratio" and can be thought of as the number of dependent people for every working age person (the ratio is usually multiplied by 100, but raw ratios are given here).

Figures to 2021 are observed. Figures from 2022 to 2100 are projected based on a medium scenario. This medium scenario is the median of many probabilistic scenarios, but these figures do not include projection intervals.

> As well as the medium scenario, UN Population offers figures (in 5 year groups) for a number of special scenarios like constant-fertility or constant-mortality (see [scenario definitions](https://population.un.org/wpp/DefinitionOfProjectionScenarios/)).

Columns include:

- `ISO3_code`:          3 letter ISO 3166-1 alpha-3 code for the country
- `Location`:           name of the country
- `Time`:               the year
- `n_male_dependent`:   number of dependent males
- `n_male_working`:     number of working males
- `n_female_dependent`: number of dependent females
- `n_female_working`:   number of working females
- `n_total_dependent`:  number of dependent people
- `n_total_working`:    number of working people
- `r_male_dependent`:   ratio of dependent males to working males
- `r_male_working`:     ratio of working males to dependent males
- `r_female_dependent`: ratio of dependent females to working females
- `r_female_working`:   ratio of working females to dependent females
- `r_total_dependent`:  ratio of dependent people to working people
- `r_total_working`:    ratio of working people to dependent people
- `time_period`:        either `observed` (until 2021) or `projected` (from 2022)

## Files not included

`WPP2022_PopulationBySingleAgeSex_Medium_1950-2021.csv` is downloaded from [population.un.org](https://population.un.org) by `index.qmd`.
