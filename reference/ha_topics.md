# List Topics

List all topics available with descriptions and units.

## Usage

``` r
ha_topics(subcategory_key = NULL, progress = TRUE)
```

## Arguments

- subcategory_key:

  Unique id for a topic subcategory

- progress:

  Display a progress bar?

## Value

Topics information tibble.

## Examples

``` r
# \donttest{
ha_set("chicagohealthatlas.org")

ha_topics("education", progress = FALSE)
#> # A tibble: 5 × 7
#>   topic_name              topic_key topic_description topic_units topic_keywords
#>   <chr>                   <chr>     <chr>             <chr>       <list>        
#> 1 9th grade education ra… EDA       Residents 25 or … % of resid… <chr [2]>     
#> 2 College graduation rate EDE       Residents 25 or … % of resid… <chr [2]>     
#> 3 High school graduation… EDB       Residents 25 or … % of resid… <chr [4]>     
#> 4 No high school diploma  NDP       The percentage o… % of resid… <chr [5]>     
#> 5 Preschool enrollment    EDG       Percentage of 3-… % of toddl… <chr [3]>     
#> # ℹ 2 more variables: topic_datasets <list>, topic_subcategories <list>
# }
```
