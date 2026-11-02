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
| [`csv/penguins.csv`](csv/penguins.csv) | 344 | R `palmerpenguins` package (`penguins`) | CC0 |
| [`csv/airports.csv`](csv/airports.csv) | 1,458 | R `nycflights13` package (`airports`) | CC0 |
| [`csv/warpbreaks.csv`](csv/warpbreaks.csv) | 54 | R `datasets` package (`warpbreaks`) | GPL-2 or GPL-3, as part of R |
| [`csv/gapminder.csv`](csv/gapminder.csv) | 1,704 | R `gapminder` package 1.0.1 (`gapminder`) | CC0 |

Except `schools.csv`, which is written from its published table, the files are copied unchanged from the CSV exports in
[Rdatasets](https://vincentarelbundock.github.io/Rdatasets/), maintained by
Vincent Arel-Bundock. The GPL texts are in [`LICENSES`](LICENSES); `weather`, `penguins`, `airports`, and `gapminder` are in the public domain under CC0. The
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

### penguins

Size measurements, sex, and study year for 344 adult penguins of three species
(Adélie, Chinstrap, and Gentoo) on three islands near Palmer Station,
Antarctica, 2007–2009, with missing measurements left empty. Gorman, K. B.,
Williams, T. D., and Fraser, W. R. (2014), Ecological sexual dimorphism and
environmental variability within a community of Antarctic penguins (genus
*Pygoscelis*), *PLoS ONE* 9(3), e90081. Distributed in `palmerpenguins` by
A. M. Horst, A. P. Hill, and K. B. Gorman.

### airports

Name, location, altitude, and time zone of 1,458 US airports, keyed by FAA
code (`faa`). From the FAA, as distributed in `nycflights13` by H. Wickham.

### warpbreaks

Number of warp breaks per loom for 54 looms, by wool type (A or B) and tension
(L, M, or H). Tippett, L. H. C. (1950), *Technological Applications of
Statistics*, Wiley, p. 106.

### gapminder

Life expectancy, population, and GDP per capita for 142 countries in five continents, every five years from 1952 to
2007, from the Gapminder Foundation (https://www.gapminder.org/data/). Bryan, J. (2023), gapminder: Data from
Gapminder, R package version 1.0.1.

## Checksums

SHA-256:

```
4d6dfa9b029dbcc15333a6e3598803fae8ae7c4d08605040b1706e6367695058  csv/mtcars.csv
e7d618f518d247ce0ef29ff551b28d4c2d260faabad4955cf9164f2908fbd0b5  csv/mroz.csv
20922ddc87d538bf2344f73d49000eeb2d7e14934b6191a3e071fefc329942c4  csv/sleepstudy.csv
8919ad586aabfa75fa3b3ece7ad7b398c7b31bf17467f17c304cbec86afa910a  csv/cbpp.csv
e69580cc3c18070692b6bf2f52e890803a313507c23283b15f06dbbae86451cf  csv/weather.csv
a1c28881a82a652fba1d3afc6254761fa95fd7f16f2ccab1fc7a7075dc8a8a0e  csv/schools.csv
c4c14fd9d1b3466dff2e046627cc32814ab6226c0e228c55f24e896a93a89b1  csv/penguins.csv
f1c5dba736fa36ecffa93cd0556b9b920a4b1a5e27bbc3ed417f05fa42edf3d6  csv/airports.csv
82c0482e94a5652b733f38c8fe6fbd18a062d761c4d71137fda63501a934a73f  csv/warpbreaks.csv
787a909f89c853d2b6ea02106c4e0d8f3f7f0f992ba36149af41c6b31817e425  csv/gapminder.csv
```
