# assignment04

---
title: "Assignment04"
author: "Xiang Xiang & Weijing Zhong"
execute: 
  warning: false

format: html
---

### Data Source
[Current Population Survey](https://cps.ipums.org/cps-action/data_requests/download).

```{r}

library(tidyverse)
library(ipumsr)

ddi <- read_ipums_ddi("cps_00003.xml")
data <- read_ipums_micro(ddi)

glimpse(data)

```