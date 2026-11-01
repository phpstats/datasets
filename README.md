# PHPstats datasets

Public datasets that the PHPstats examples and comparisons read by URL, so
anyone can run them. Each file is a CSV with a header row; `rownames` holds the
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

The files are copied unchanged from the CSV exports in
[Rdatasets](https://vincentarelbundock.github.io/Rdatasets/), maintained by
Vincent Arel-Bundock. The license texts are in [`LICENSES`](LICENSES). The
data remain under their packages' licenses; this repository adds nothing to
them.

## Sources

**mtcars.** Fuel consumption and ten aspects of design and performance for 32
cars (1973–74 models), from the 1974 *Motor Trend* US magazine. Henderson, H.
V. and Velleman, P. F. (1981), Building multiple regression models
interactively, *Biometrics* 37, 391–411.

**mroz.** Labor force participation of 753 married women in 1975, from the
Panel Study of Income Dynamics. Mroz, T. A. (1987), The sensitivity of an
empirical model of married women's hours of work to economic and statistical
assumptions, *Econometrica* 55, 765–799. Distributed in `carData` by J. Fox,
S. Weisberg, and B. Price.

**sleepstudy.** Average reaction time per day for 18 subjects in a sleep
deprivation study, days 0–9. Belenky, G. et al. (2003), Patterns of
performance degradation and restoration during sleep restriction and
subsequent recovery, *Journal of Sleep Research* 12, 1–12.

**cbpp.** Serological incidence of contagious bovine pleuropneumonia in 15
herds of zebu cattle in Ethiopia, over four periods. Lesnoff, M. et al.
(2004), Within-herd spread of contagious bovine pleuropneumonia in Ethiopian
highlands, *Preventive Veterinary Medicine* 64, 27–40.

## Checksums

SHA-256:

```
4d6dfa9b029dbcc15333a6e3598803fae8ae7c4d08605040b1706e6367695058  csv/mtcars.csv
e7d618f518d247ce0ef29ff551b28d4c2d260faabad4955cf9164f2908fbd0b5  csv/mroz.csv
20922ddc87d538bf2344f73d49000eeb2d7e14934b6191a3e071fefc329942c4  csv/sleepstudy.csv
8919ad586aabfa75fa3b3ece7ad7b398c7b31bf17467f17c304cbec86afa910a  csv/cbpp.csv
```
