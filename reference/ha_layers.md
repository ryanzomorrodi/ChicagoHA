# List Geographic Layers

List all geographic layers available.

## Usage

``` r
ha_layers()
```

## Value

Layer information tibble.

## Examples

``` r
# \donttest{
ha_set("chicagohealthatlas.org")

ha_layers()
#> # A tibble: 7 × 3
#>   layer_name      layer_key    layer_url                                        
#>   <chr>           <chr>        <chr>                                            
#> 1 Community areas neighborhood https://media.metop.io/shapes/ancestries/communi…
#> 2 ZIP Codes       zip          https://media.metop.io/shapes/teams/chicago-heal…
#> 3 Census Tracts   tract-2020   https://media.metop.io/shapes/teams/chicago-heal…
#> 4 Chicago         place        https://media.metop.io/shapes/teams/chicago-heal…
#> 5 United States   us           https://media.metop.io/shapes/us.topo.json       
#> 6 States          state        https://media.metop.io/shapes/teams/chicago-heal…
#> 7 Counties        county       https://media.metop.io/shapes/teams/chicago-heal…
# }
```
