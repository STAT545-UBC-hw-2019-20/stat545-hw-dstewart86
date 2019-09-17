Assignment 1: Exercise 2
================
Daniel Stewart
16 September 2019

Loading Libraries
-----------------

``` r
library(rmarkdown)
```

    ## Warning: package 'rmarkdown' was built under R version 3.5.3

``` r
library(gapminder)
```

    ## Warning: package 'gapminder' was built under R version 3.5.3

Determining the number of columns in the dataset
------------------------------------------------

``` r
ncol(gapminder)
```

    ## [1] 6

Listing the column names of the dataset
---------------------------------------

``` r
names(gapminder)
```

    ## [1] "country"   "continent" "year"      "lifeExp"   "pop"       "gdpPercap"

Investigating the mean life expectancy of all countries across all years
------------------------------------------------------------------------

``` r
LifeExp <- gapminder$lifeExp
mean(LifeExp)
```

    ## [1] 59.47444

Looking at the countries included in the dataset (ordered alphabetically)
-------------------------------------------------------------------------

``` r
Countries <-gapminder$country
MasterList <-unique(Countries)
MasterList[1:10]
```

    ##  [1] Afghanistan Albania     Algeria     Angola      Argentina  
    ##  [6] Australia   Austria     Bahrain     Bangladesh  Belgium    
    ## 142 Levels: Afghanistan Albania Algeria Angola Argentina ... Zimbabwe
