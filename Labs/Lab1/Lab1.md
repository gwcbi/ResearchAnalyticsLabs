# Lab 1: Introduction to R

## Introduction

R is a free software environment for statistics. 

In this lab, you will install R and practice loading a basic dataset.

## Setup

### Installing R

The latest version of R is available for download on Linux, OS X and Windows on the Comprehensive R Archive Network (CRAN): [https://cran.r-project.org/](https://cran.r-project.org/).

### Installing RStudio (optional)

RStudio is a (free) intergrated developement environment for R. You can think of R Studio as a companion program for basic R that helps you by keeping track of your things and organizing your various windows. Some people prefer to use R within in RStudio, but you do **not** need RStudio for this course.

Install R before installing RStudio (if install RStudio).

RStudio is available for download on [www.rstudio.com](https://www.rstudio.com/products/rstudio/download/). You do **not** need to pay money for RStudio. You can use RStudio Desktop under the Open Source License.

### R Packages

#### Installing R Packages

In addition to hosting the actual R software, CRAN also hosts a variety of packages of R code. These packages are neatly bundled pieces of R code that add functionality to your basic R environment.

One package that is very handy for data science is Tidyverse (actually a collection of packages). Install Tidyverse by running the following command:

```r
install.packages("tidyverse")
```

#### Loading R Packages

Once installed, packages need to be loaded into your environment before you can use them. You can load the core packages of Tidyverse by running the following command.

```r
library("tidyverse")
```

## Help! How do I use this?

To quickly open the documentation for package or function using the `help()` function. This can be shortened to just a question mark. In RStudio, this will open a help window on your chosen function.

```r
# An example
help(tidyverse)
?tidyverse #this does the same thing
```

You can find more information on getting help with R on the [R Project website.](https://www.r-project.org/help.html)


## Reading Data into R

R comes with a variety of functions built-in to help you load data. When we load Tidyverse, a package called `readr` is also loaded which contains additional functions to help you load data.

There are two basic ways to load comma-separated value files into R, now that we've loaded the Tidyverse package. We can use the `read.csv` function from base R or the `read_csv` function from the `readr` package which got loaded as part of the Tidyverse core. One notable difference between `read.csv` and `read_csv` is that `read.csv` will return a standard R dataframe whereas `read_csv` will return a tibble, which like a standard R dataframe but with certain changes to improve their behavior. 

Look up the details on how to use one of these two functions using the help documentation.

In addition to `read.csv` or `read_csv`, both base R and the `readr` package contain functions to read many other formats. Explore these on your own.

If they don't contain code that will read in your preferred format, there may be another package in existence that does. For example, if you want to load in data directly from a Microsoft Excel spreadsheet, you could do this by using the [readxl package](http://readxl.tidyverse.org/).

## Your Turn: Loading a Dataset

You can choose between a publicly available health dataset or you can use your own data if you have any! Here are some suggestions.

* [Inpatient Prospective Payment System (IPPS) Provider Summary for the Top 100 Diagnosis-Related Groups (DRG) - FY2011](https://data.cms.gov/Medicare-Inpatient/Inpatient-Prospective-Payment-System-IPPS-Provider/97k6-zzx3)
* [U.S. Chronic Disease Indicators (CDI)](https://catalog.data.gov/dataset/u-s-chronic-disease-indicators-cdi-e50c9)

Start a new R script file to save your work (showing each of the following steps)
Load your preferred dataset into R. Print the first 5 rows and 5 columns. Submit your work as an R script (somefilename.R).

## The report

For this first lab, save your code as an R script file and submit it through the course 2GW site. Clean up your code first if necessary, but ensure that it works as submitted.

## Due date

Day 7, Week 2
