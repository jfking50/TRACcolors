
<!-- README.md is generated from README.Rmd. Please edit that file -->

# TRACcolors

A simple package to display TRAC standard colors and generate those
colors in hex format for use in plotting.

## Quick Demo

Display a grid of TRAC colors and their associated color code with
`colorgrid()`.

``` r
library(TRACcolors)
colorgrid()
```

<img src="man/figures/README-unnamed-chunk-2-1.png" width="100%" />

Referring to this plot, choose the color(s) of interest in the plotting
package of your choice. Note in the example below that `tcolor("bl1")`
is a string that is the associated color in hex format.

``` r
library(ggplot2)
ggplot() + 
  geom_col(aes(x=c("foo", "bar"), y=1:2), fill = tcolor("bl1")) +
  xlab("X Axis Title") + ylab("Y Axis Title")
```

<img src="man/figures/README-unnamed-chunk-3-1.png" width="100%" />
