
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Building a Bioconductor package using RStudio

## Key resources

  - Docker image: [Docker
    Hub](https://hub.docker.com/repository/docker/saskiafreytag/making_bioconductor_pkg)
  - Workshop material: [pkgdown
    website](https://saskiafreytag.github.io/making_bioconductor_pkg)

## Workshop description

This workshop gives an introductory overview of how to build a
Bioconductor package.

Workshop participants will learn what makes a Bioconductor package
special, how to get started building one and how to disseminate your
final product. This workshop will feature introductory material, ‘live’
coding, and Q\&A, all of which are adapted from the content below.

### Instructor

  - [Saskia Freytag](https://twitter.com/trashystats)
    (<saskia.freytag@perkins.uwa.edu.au>)
  - [Peter Hickey](https://peterhickey.org/) (<hickey@wehi.edu.au>)

### Pre-requisites

  - Basic knowledge of R syntax.
  - Github account\!\!\!

### Workshop Participation

Students will build a small package which is ideally version controlled.
There will be a Q\&A session in the second half of the workshop.

### Workshop goals and objectives

#### Learning goals

  - Understand the purpose of a package
  - Learn about the essential building blocks of a package
  - Develop your first simple package
  - Become familiar with version control

## Installation

This workshop uses Bioconductor version 3.12. At the time of writing,
this is the current ‘devel’ version of Bioconductor, which can be
installed following [these
instructions](https://www.bioconductor.org/developers/how-to/useDevel/).

You can then install the packages necessary for this workshop using the
following:

``` r
library(BiocManager)
install(c("usethis", "roxygen2", "devtools", "goodpractice", "BiocCheck"))
```

Alternatively, you can might like to use Docker to run the workshop in a
container with R, all the necessary packages, and RStudio. This can be
done as follows:

  - Log in to RStudio at <http://localhost:8787> using username
    `rstudio` and password `welcome-to-bioc2020`. Note that on Windows
    you need to provide your localhost IP address like
    `http://191.163.92.108:8787/` - find it using `docker-machine ip
    default` in Docker’s terminal.
  - Run `browseVignettes(package = "Building a Bioconductor Package")`.
    Click on one of the links, “HTML”, “source”, “R code”.
      - In case of `The requested page was not found` error, add `help/`
        to the URL right after the hostname, e.g.,
        <http://localhost:8787/help/library/making_bioconductor_pkg/doc/Building_a_Bioconductor_Packages.html>.
        This is a [known
        bug](https://github.com/rocker-org/rocker-versioned/issues/178).
