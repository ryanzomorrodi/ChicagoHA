# List Topic Coverage

List all combinations of population, periods, and geographic layers
available for a given topic. To search for individual topics use
[`ha_topics()`](https://ryanzomorrodi.github.io/healthatlas/reference/ha_topics.md).

## Usage

``` r
ha_coverage(topic_key, layer_key = NULL, keys_only = FALSE, progress = TRUE)
```

## Arguments

- topic_key:

  Unique ID specifying a topic.

- layer_key:

  Character string or vector of Unique IDs for geographic layers.

- keys_only:

  Return only keys?

- progress:

  Display a progress bar?

## Value

Topic coverage tibble.

## Examples

``` r
# \donttest{
ha_set("chicagohealthatlas.org")

ha_coverage("POP", progress = FALSE)
#> # A tibble: 8,243 × 7
#>    topic_key population_key population_name       population_grouping period_key
#>    <chr>     <chr>          <chr>                 <chr>               <chr>     
#>  1 POP       WY             White, Young Adults … Race/Ethnicity and… 2014-2018 
#>  2 POP       BY             Black, Young Adults … Race/Ethnicity and… 2010-2014 
#>  3 POP       S              65 and older          Age                 2005      
#>  4 POP       WY             White, Young Adults … Race/Ethnicity and… 2015-2019 
#>  5 POP       MY             Males, Young Adults … Sex and Age         2014-2018 
#>  6 POP       FY             Females, Young Adult… Sex and Age         2017-2021 
#>  7 POP       BF             Black, Females        Race/Ethnicity and… 2011      
#>  8 POP       H              Hispanic or Latino    Race/Ethnicity      2010-2014 
#>  9 POP       AY             Asian, Young Adults … Race/Ethnicity and… 2005      
#> 10 POP       AY             Asian, Young Adults … Race/Ethnicity and… 2008-2012 
#> # ℹ 8,233 more rows
#> # ℹ 2 more variables: layer_key <chr>, layer_name <chr>
# }
```
