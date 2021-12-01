SDS 192 2021 Fall PS07
================

# Section 01

## GitHub Documents

This is an R Markdown format used for publishing markdown documents to
GitHub. When you click the **Knit** button all R code chunks are run and
a markdown file (.md) suitable for publishing to GitHub is generated.

## Including Code

You can include R code in the document as follows:

``` r
# Load all packages here
library(ggplot2)
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
library(babynames)
```

``` r
# Set up the dataframe for visualization
babynames_riley_casey <- babynames %>% 
  filter((name == "Riley" | name == "Casey")) %>% 
           group_by(year)
View(babynames_riley_casey)
```

## Including Plots

You can also embed plots, for example:

![](README_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
