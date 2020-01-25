
<!-- README.md is generated from README.Rmd. Please edit that file -->
makeproject
===========

<!-- badges: start -->
[![Travis build status](https://travis-ci.org/nibortolum/makeproject.svg?branch=master)](https://travis-ci.org/nibortolum/makeproject) <!-- badges: end -->

The goal of makeproject is to quickly deploy new project folders, with a consistent architecture.

Installation
------------

You can install the released version of makeproject from [Github](https://github.com/nibortolum/makeproject) with:

``` r
library(devtools)
install_github("https://github.com/nibortolum/makeproject")
```

More advanced versions will be pushed to CRAN in the future.

Example
-------

This is a basic example which shows you how to crete a project folder:

``` r
library(makeproject)

## Once in the proper folder :

make_project("kickassProject")
```

Do not pur white spaces in your poject name. It will be ugly and may mess up with path handling, depending on which OS youre working on.

This function will create the following structure :

    ├── KickassProject
    │   ├── Data
    │   ├── Docs
    │   │   └── KickassProject_docs.Rmd
    │   ├── Figures
    │   ├── Gist
    │   ├── KickassProject_MainScript.R
    │   └── Sources

-   Data is the folder where you need to put the data (csv, .Rdata files, etc)
-   Docs is a folder in which you store documentation related to the ongoing project. It comes with a pretemplated Rmd file
-   Figures is the folder where to save the figures
-   Gist a folder where to store small useful pieces of codes
-   Sources is a folder where to place some functionnal R scripts containing ready-to-use functions you would like to import
-   KickassProject\_MainScript.R is the pretemplated main project Script.
