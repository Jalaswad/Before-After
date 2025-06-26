<!-- README.md is generated from README.Rmd. -->

# Interaction of severe climate change and extinctions result in ecosystem simplification across time and space

<!-- badges: start -->
<!-- badges: end -->

This GitHub repository contains the code used to analyse all
datasets presented in **Interaction of severe climate change and extinctions result in ecosystem simplification across time and space**

by Jood Al Aswad, Mohamad Bazzi, Justin Penn, Pedro Monarrez, Curtis Deutsch and Jonathan L. Payne

Code written and maintained by Jood Al Aswad and Mohamad Bazzi
<br/>
Contact:
<jalaswad@stanford.edu> and <bazzi@stanford.edu>

**All codes and data used in this paper are provided here for reproducibility.**

There are two ways to access the Paleobiology Database data used in this study. You may either open the pbdb.csv file for the interval of your choice in the Pbdb-files folder to access the processed dataset utilized here, or if you wish to download straight from the database, you may use R and start with 01_download_pbdb_new.R to download the raw dataset used in this study with instructions on how to process and clean that data in 02_AllCalcs.html.

The fossil occurrence analyes can be found and reproduced by opening 02_AllCalcs.html, which is accompanied by the source code 02_AllCalcs.qmd. The script for creating figures 2 and 3 are in 03_Differences-Figure3.html and 04_Stripes-Figure2.html and their accompanying .qmd files.

The recommended order to go through the code is:
*  01_download_pbdb_new.R
*  02_AllCalcs.html (or .qmd)
*  03_Differences-Figure3.html (or .qmd)
*  04_Stripes-Figure2.html (or .qmd)

 The .qmd files are Quarto markdown files for R and RStudio.

## Access .Rdata

Larger assets can be accessed from within a report using
[`piggyback`](https://github.com/ropensci/piggyback)!

``` r
# Install and load R package
require(piggyback)

# Create temporary directory and load .Rdata into R environment,
pb_download(file = "default.RData",dest = tempdir(),repo = "mohabazzi/AptianShark",tag = "v.01")
load(file = file.path(tempdir(),"default.RData"))
```