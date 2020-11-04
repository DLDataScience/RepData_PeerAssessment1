---
title: "Reproducible Research: Peer Assessment 1"
author: "David Levy"
date: "11/3/2020"
output: 
  html_document:
    keep_md: true
---



## Loading and preprocessing the data

We'll be making use of the `tidyverse` here, so we'll just load the whole library.


```r
library(tidyverse)
```

```
## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──
```

```
## ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
## ✓ tibble  3.0.4     ✓ dplyr   1.0.2
## ✓ tidyr   1.1.2     ✓ stringr 1.4.0
## ✓ readr   1.4.0     ✓ forcats 0.5.0
```

```
## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
## x dplyr::filter() masks stats::filter()
## x dplyr::lag()    masks stats::lag()
```

Let's begin by reading in our data to get a sense for what it looks like:


```r
# `read_csv` will automatically unzip our csv
activity <- read_csv('activity.zip')
```

```
## 
## ── Column specification ────────────────────────────────────────────────────────
## cols(
##   steps = col_double(),
##   date = col_date(format = ""),
##   interval = col_double()
## )
```

```r
str(activity)
```

```
## tibble [17,568 × 3] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
##  $ steps   : num [1:17568] NA NA NA NA NA NA NA NA NA NA ...
##  $ date    : Date[1:17568], format: "2012-10-01" "2012-10-01" ...
##  $ interval: num [1:17568] 0 5 10 15 20 25 30 35 40 45 ...
##  - attr(*, "spec")=
##   .. cols(
##   ..   steps = col_double(),
##   ..   date = col_date(format = ""),
##   ..   interval = col_double()
##   .. )
```

Notice, we have the following columns, as described in the instructions:

- *steps*: Number of steps taken in a $5$-minute interval (missing values coded as `NA`).

- *date*: The date on which the measurement was taken in YYYY-MM-DD format.

- *interval*: Identifier for the 5-minute interval in which measurement was taken.

The only modification that looks necessary in terms of adjusting the variable **classes** is 


## What is mean total number of steps taken per day?



## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
