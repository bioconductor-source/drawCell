
<!-- README.md is generated from README.Rmd. Please edit that file -->

# drawCell

<!-- badges: start -->
<!-- badges: end -->

The goal of drawCell is to easily obtain nice cell pictures in R!

## Installation

drawCell needs the package
[webshot2](https://github.com/rstudio/webshot2), which needs to be
installed.

draCell connects to the [SwissBioPics
API](https://www.swissbiopics.org/) to generate the images.

``` r
# install.packages("devtools")
devtools::install_github("svalvaro/MQmetrics")
```

## Example

This is a basic example which shows you how to solve a common problem:

It requires the [taxonomy id](https://www.ncbi.nlm.nih.gov/taxonomy/) of
your species of interest, and one or multiple SL codes for subcellular
locations that will be colored. [This
dataset](http://current.geneontology.org/ontology/external2go/uniprotkb_sl2go)
contains the SL codes for each subcellular location.

The taxonomy id for *Quercus ilex* a common tree in the south of Spain
is `58334` and as an example I will use the SL code of the chloroplast:
`0049`.

``` r
library(drawCell)

drawCell(taxonomy_id = '58334', sl_ids = '0049')
```

<img src="man/figures/README-example-1.png" width="100%" />
