
![EMMA](img/EMMA%20Logo_RE_3.jpg)

# Ecological Monitoring and Management Application (EMMA)

This is the core repository for environmental data processing in the
Ecological Monitoring and Management Application [EMMA.io](EMMA.io).

## File structure

The most important files are:

``` r
├── _targets.R (data processing workflow and dependency management)
├── R/
├──── [data_processing_functions]
├── data/
├──── manual_download (files behind firewalls that must be manually downloaded)
├──── raw_data (raw data files downloaded by the workflow)
├──── processed_data (data processed and stored by the workflow)
├──── emma_static.csv (static environmental data for the domain)
├──── emma_dymnamic.csv (dynamic environmental data for the domain)
└── Readme.Rmd (this file)
```

# Workflow structure

![](README_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

# Extras

    * Call `targets::tar_renv(extras = character(0))` to write a `_packages.R` file to expose hidden dependencies.
    * Call `renv::init()` to initialize the `renv` lockfile `renv.lock` or `renv::snapshot()` to update it.
    * Commit `renv.lock` to your Git repository.
