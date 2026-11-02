# PHPstats datasets

Public datasets that the PHPstats examples and comparisons read by URL, so
anyone can run them. Each file is a CSV with a header row; where present, `rownames` holds the
row names the data had in R.

```php
$data = 'https://raw.githubusercontent.com/phpstats/datasets/main/csv';
$mroz = \Phibble\DataFrame::fromCsv("$data/mroz.csv");
```

| File | Rows | From | License |
|---|---|---|---|
| [`csv/mtcars.csv`](csv/mtcars.csv) | 32 | R `datasets` package (`mtcars`) | GPL-2 or GPL-3, as part of R |
| [`csv/mroz.csv`](csv/mroz.csv) | 753 | R `carData` package 3.0-6 (`Mroz`) | GPL (≥ 2) |
| [`csv/sleepstudy.csv`](csv/sleepstudy.csv) | 180 | R `lme4` package 2.0.6 (`sleepstudy`) | GPL (≥ 2) |
| [`csv/cbpp.csv`](csv/cbpp.csv) | 56 | R `lme4` package 2.0.6 (`cbpp`) | GPL (≥ 2) |
| [`csv/insurance.csv`](csv/insurance.csv) | 64 | R `MASS` package 7.3-65 (`Insurance`) | GPL-2 or GPL-3 |
| [`csv/weather.csv`](csv/weather.csv) | 26,115 | R `nycflights13` package (`weather`) | CC0 |
| [`csv/schools.csv`](csv/schools.csv) | 8 | Rubin (1981), as tabulated in *Bayesian Data Analysis* | Published summary statistics |

Except `schools.csv`, which is written from its published table, the files are copied unchanged from the CSV exports in
[Rdatasets](https://vincentarelbundock.github.io/Rdatasets/), maintained by
Vincent Arel-Bundock. The GPL texts are in [`LICENSES`](LICENSES); `weather` is in the public domain under CC0. The
data remain under their packages' licenses; this repository adds nothing to
them.

## Sources

### mtcars

Fuel consumption and ten aspects of design and performance for 32
cars (1973–74 models), from the 1974 *Motor Trend* US magazine. Henderson, H.
V. and Velleman, P. F. (1981), Building multiple regression models
interactively, *Biometrics* 37, 391–411.

### mroz

Labor force participation of 753 married women in 1975, from the
Panel Study of Income Dynamics. Mroz, T. A. (1987), The sensitivity of an
empirical model of married women's hours of work to economic and statistical
assumptions, *Econometrica* 55, 765–799. Distributed in `carData` by J. Fox,
S. Weisberg, and B. Price.

### sleepstudy

Average reaction time per day for 18 subjects in a sleep
deprivation study, days 0–9. Belenky, G. et al. (2003), Patterns of
performance degradation and restoration during sleep restriction and
subsequent recovery, *Journal of Sleep Research* 12, 1–12.

### cbpp

Serological incidence of contagious bovine pleuropneumonia in 15
herds of zebu cattle in Ethiopia, over four periods. Lesnoff, M. et al.
(2004), Within-herd spread of contagious bovine pleuropneumonia in Ethiopian
highlands, *Preventive Veterinary Medicine* 64, 27–40.

### insurance

Car insurance claims made in the third quarter of 1973 by the policyholders of
an insurance company, by district of residence (4 is the major cities), car
group, and age group, with the number of policyholders exposed to risk. Baxter,
L. A., Coutts, S. M. and Ross, G. A. F. (1980), Applications of linear models
in motor insurance, *Proceedings of the 21st International Congress of
Actuaries*, Zurich, 11–29. Distributed in `MASS` by W. N. Venables and B. D.
Ripley.

### weather

Hourly weather at the three New York City airports (EWR, JFK, and LGA) in
2013: temperature, dew point, humidity, wind, precipitation, pressure, and
visibility, with missing readings left empty. From the Iowa Environmental
Mesonet, as distributed in `nycflights13` by H. Wickham.

### schools

Estimated effects of a coaching program on SAT-V scores in eight high schools
(A–H), with their standard errors: `y` is the estimated effect and `sigma` its
standard error. Rubin, D. B. (1981), Estimation in parallel randomized
experiments, *Journal of Educational Statistics* 6(4), 377–401; as tabulated
in Gelman, A. et al., *Bayesian Data Analysis* (3rd ed.), Table 5.2. Written
out here from the published table; `rownames` is not used for this file.

## Checksums

SHA-256:

```
4d6dfa9b029dbcc15333a6e3598803fae8ae7c4d08605040b1706e6367695058  csv/mtcars.csv
e7d618f518d247ce0ef29ff551b28d4c2d260faabad4955cf9164f2908fbd0b5  csv/mroz.csv
20922ddc87d538bf2344f73d49000eeb2d7e14934b6191a3e071fefc329942c4  csv/sleepstudy.csv
8919ad586aabfa75fa3b3ece7ad7b398c7b31bf17467f17c304cbec86afa910a  csv/cbpp.csv
e69580cc3c18070692b6bf2f52e890803a313507c23283b15f06dbbae86451cf  csv/weather.csv
a1c28881a82a652fba1d3afc6254761fa95fd7f16f2ccab1fc7a7075dc8a8a0e  csv/schools.csv
```
