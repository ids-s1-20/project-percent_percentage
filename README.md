[![Check allowed files](https://github.com/ids-s1-20/project-percent_percentage/workflows/Check%20allowed%20files/badge.svg)](https://github.com/ids-s1-20/project-percent_percentage/actions?query=workflow:%22Check%20allowed%20files%22) [![Check presentation renders](https://github.com/ids-s1-20/project-percent_percentage/workflows/Check%20presentation%20renders/badge.svg)](https://github.com/ids-s1-20/project-percent_percentage/actions?query=workflow:%22Check%20presentation%20renders%22) [![Check README renders](https://github.com/ids-s1-20/project-percent_percentage/workflows/Check%20README%20renders/badge.svg)](https://github.com/ids-s1-20/project-percent_percentage/actions?query=workflow:%22Check%20README%20renders%22)


Coffee Ratings
================
percentage-%

## Summary

As we all know, nowadays people are more and more getting used to having
a cup of coffee in the morning to start the day. Therefore, an
increasing amount of coffee lovers are trying to research the quality of
coffees so that higher quality of coffee can be provided to the world.
In order to find out how the quality of coffee can be related to other
factors such as farms or companies, we are employing the database from
TidyTuesday with the source James LeDoux & Coffee Quality Database.

# Coffee Ratings

The data this week comes from James LeDoux & Coffee Quality Database
(<https://github.com/jldbc/coffee-quality-database>). This Yorgos
Askalidis - TWD
(<https://towardsdatascience.com/the-data-speak-ethiopia-has-the-best-coffee-91f88ed37e84>)
talks about Coffee Ratings in greater detail. Credit: %(Percentage)

    ## 
    ## ── Column specification ────────────────────────────────────────────────────────
    ## cols(
    ##   .default = col_character(),
    ##   total_cup_points = col_double(),
    ##   number_of_bags = col_double(),
    ##   aroma = col_double(),
    ##   flavor = col_double(),
    ##   aftertaste = col_double(),
    ##   acidity = col_double(),
    ##   body = col_double(),
    ##   balance = col_double(),
    ##   uniformity = col_double(),
    ##   clean_cup = col_double(),
    ##   sweetness = col_double(),
    ##   cupper_points = col_double(),
    ##   moisture = col_double(),
    ##   category_one_defects = col_double(),
    ##   quakers = col_double(),
    ##   category_two_defects = col_double(),
    ##   altitude_low_meters = col_double(),
    ##   altitude_high_meters = col_double(),
    ##   altitude_mean_meters = col_double()
    ## )
    ## ℹ Use `spec()` for the full column specifications.

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──

    ## ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
    ## ✓ tibble  3.0.4     ✓ dplyr   1.0.2
    ## ✓ tidyr   1.1.2     ✓ stringr 1.4.0
    ## ✓ readr   1.4.0     ✓ forcats 0.5.0

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

    ## Warning: Missing column names filled in: 'X1' [1]

    ## 
    ## ── Column specification ────────────────────────────────────────────────────────
    ## cols(
    ##   .default = col_character(),
    ##   X1 = col_double(),
    ##   Number.of.Bags = col_double(),
    ##   Aroma = col_double(),
    ##   Flavor = col_double(),
    ##   Aftertaste = col_double(),
    ##   Acidity = col_double(),
    ##   Body = col_double(),
    ##   Balance = col_double(),
    ##   Uniformity = col_double(),
    ##   Clean.Cup = col_double(),
    ##   Sweetness = col_double(),
    ##   Cupper.Points = col_double(),
    ##   Total.Cup.Points = col_double(),
    ##   Moisture = col_double(),
    ##   Category.One.Defects = col_double(),
    ##   Quakers = col_double(),
    ##   Category.Two.Defects = col_double(),
    ##   altitude_low_meters = col_double(),
    ##   altitude_high_meters = col_double(),
    ##   altitude_mean_meters = col_double()
    ## )
    ## ℹ Use `spec()` for the full column specifications.

    ## Warning: Missing column names filled in: 'X1' [1]

|                                                  |            |
| :----------------------------------------------- | :--------- |
| Name                                             | Piped data |
| Number of rows                                   | 1339       |
| Number of columns                                | 43         |
| \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_   |            |
| Column type frequency:                           |            |
| character                                        | 24         |
| numeric                                          | 19         |
| \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |            |
| Group variables                                  | None       |

Data summary

**Variable type: character**

| skim\_variable         | n\_missing | complete\_rate | min | max | empty | n\_unique | whitespace |
| :--------------------- | ---------: | -------------: | --: | --: | ----: | --------: | ---------: |
| species                |          0 |           1.00 |   7 |   7 |     0 |         2 |          0 |
| owner                  |          7 |           0.99 |   3 |  50 |     0 |       315 |          0 |
| country\_of\_origin    |          1 |           1.00 |   4 |  28 |     0 |        36 |          0 |
| farm\_name             |        359 |           0.73 |   1 |  73 |     0 |       571 |          0 |
| lot\_number            |       1063 |           0.21 |   1 |  71 |     0 |       227 |          0 |
| mill                   |        315 |           0.76 |   1 |  77 |     0 |       460 |          0 |
| ico\_number            |        151 |           0.89 |   1 |  40 |     0 |       847 |          0 |
| company                |        209 |           0.84 |   3 |  73 |     0 |       281 |          0 |
| altitude               |        226 |           0.83 |   1 |  41 |     0 |       396 |          0 |
| region                 |         59 |           0.96 |   2 |  76 |     0 |       356 |          0 |
| producer               |        231 |           0.83 |   1 | 100 |     0 |       691 |          0 |
| bag\_weight            |          0 |           1.00 |   1 |   8 |     0 |        56 |          0 |
| in\_country\_partner   |          0 |           1.00 |   7 |  85 |     0 |        27 |          0 |
| harvest\_year          |         47 |           0.96 |   3 |  24 |     0 |        46 |          0 |
| grading\_date          |          0 |           1.00 |  13 |  20 |     0 |       567 |          0 |
| owner\_1               |          7 |           0.99 |   3 |  50 |     0 |       319 |          0 |
| variety                |        226 |           0.83 |   4 |  21 |     0 |        29 |          0 |
| processing\_method     |        170 |           0.87 |   5 |  25 |     0 |         5 |          0 |
| color                  |        218 |           0.84 |   4 |  12 |     0 |         4 |          0 |
| expiration             |          0 |           1.00 |  13 |  20 |     0 |       566 |          0 |
| certification\_body    |          0 |           1.00 |   7 |  85 |     0 |        26 |          0 |
| certification\_address |          0 |           1.00 |  40 |  40 |     0 |        32 |          0 |
| certification\_contact |          0 |           1.00 |  40 |  40 |     0 |        29 |          0 |
| unit\_of\_measurement  |          0 |           1.00 |   1 |   2 |     0 |         2 |          0 |

**Variable type: numeric**

| skim\_variable         | n\_missing | complete\_rate |    mean |      sd | p0 |     p25 |     p50 |     p75 |      p100 | hist  |
| :--------------------- | ---------: | -------------: | ------: | ------: | -: | ------: | ------: | ------: | --------: | :---- |
| total\_cup\_points     |          0 |           1.00 |   82.09 |    3.50 |  0 |   81.08 |   82.50 |   83.67 |     90.58 | ▁▁▁▁▇ |
| number\_of\_bags       |          0 |           1.00 |  154.18 |  129.99 |  0 |   14.00 |  175.00 |  275.00 |   1062.00 | ▇▇▁▁▁ |
| aroma                  |          0 |           1.00 |    7.57 |    0.38 |  0 |    7.42 |    7.58 |    7.75 |      8.75 | ▁▁▁▁▇ |
| flavor                 |          0 |           1.00 |    7.52 |    0.40 |  0 |    7.33 |    7.58 |    7.75 |      8.83 | ▁▁▁▁▇ |
| aftertaste             |          0 |           1.00 |    7.40 |    0.40 |  0 |    7.25 |    7.42 |    7.58 |      8.67 | ▁▁▁▁▇ |
| acidity                |          0 |           1.00 |    7.54 |    0.38 |  0 |    7.33 |    7.58 |    7.75 |      8.75 | ▁▁▁▁▇ |
| body                   |          0 |           1.00 |    7.52 |    0.37 |  0 |    7.33 |    7.50 |    7.67 |      8.58 | ▁▁▁▁▇ |
| balance                |          0 |           1.00 |    7.52 |    0.41 |  0 |    7.33 |    7.50 |    7.75 |      8.75 | ▁▁▁▁▇ |
| uniformity             |          0 |           1.00 |    9.83 |    0.55 |  0 |   10.00 |   10.00 |   10.00 |     10.00 | ▁▁▁▁▇ |
| clean\_cup             |          0 |           1.00 |    9.84 |    0.76 |  0 |   10.00 |   10.00 |   10.00 |     10.00 | ▁▁▁▁▇ |
| sweetness              |          0 |           1.00 |    9.86 |    0.62 |  0 |   10.00 |   10.00 |   10.00 |     10.00 | ▁▁▁▁▇ |
| cupper\_points         |          0 |           1.00 |    7.50 |    0.47 |  0 |    7.25 |    7.50 |    7.75 |     10.00 | ▁▁▁▇▁ |
| moisture               |          0 |           1.00 |    0.09 |    0.05 |  0 |    0.09 |    0.11 |    0.12 |      0.28 | ▃▇▅▁▁ |
| category\_one\_defects |          0 |           1.00 |    0.48 |    2.55 |  0 |    0.00 |    0.00 |    0.00 |     63.00 | ▇▁▁▁▁ |
| quakers                |          1 |           1.00 |    0.17 |    0.83 |  0 |    0.00 |    0.00 |    0.00 |     11.00 | ▇▁▁▁▁ |
| category\_two\_defects |          0 |           1.00 |    3.56 |    5.31 |  0 |    0.00 |    2.00 |    4.00 |     55.00 | ▇▁▁▁▁ |
| altitude\_low\_meters  |        230 |           0.83 | 1750.71 | 8669.44 |  1 | 1100.00 | 1310.64 | 1600.00 | 190164.00 | ▇▁▁▁▁ |
| altitude\_high\_meters |        230 |           0.83 | 1799.35 | 8668.81 |  1 | 1100.00 | 1350.00 | 1650.00 | 190164.00 | ▇▁▁▁▁ |
| altitude\_mean\_meters |        230 |           0.83 | 1775.03 | 8668.63 |  1 | 1100.00 | 1310.64 | 1600.00 | 190164.00 | ▇▁▁▁▁ |

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

Askalidis, Y. (2019, March 26). The data is in: Ethiopia has the best
coffee. Retrieved October 23, 2020, from
<https://towardsdatascience.com/the-data-speak-ethiopia-has-the-best-coffee-91f88ed37e84>

LeDoux, J. (2018, June 17). Jldbc/coffee-quality-database. Retrieved
October 23, 2020, from
<https://github.com/jldbc/coffee-quality-database>

## References

James LeDoux & Coffee Quality Database
(<https://github.com/jldbc/coffee-quality-database>). Yorgos Askalidis -
TWD
(<https://towardsdatascience.com/the-data-speak-ethiopia-has-the-best-coffee-91f88ed37e84>)
