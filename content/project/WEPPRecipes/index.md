---
author: Chinmay Deval
categories:
- R
- package
date: "2019-07-02"
draft: false
excerpt: An R package for post processing Watershed Erosion Prediction Project (WEPP) model simulations.   
featured: true
layout: single
links:
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/devalc/WEPPRecipes
subtitle: ""
tags:
- hugo-site
title: WEPPRecipes
---


An R package containing functions for post processing, analyzing and visualizing Watershed Erosion Prediction Project (WEPP) model simulations.         

### Getting Started

These instructions will get you a copy of the "WEPPRecipes" up and running on your 
local machine.

### How to Install

This package is available only via GitHub. 

First, install devtools by running following command in your R console: 

```{r}
install.packages("devtools")
```

Now you can install the WEPPRecipes package from Github using devtools as:

```{r}
devtools::install_github("devalc/WEPPRecipes")
```
Once installed the package can be loaded to the system using:
```{r}
library(WEPPRecipes)
```