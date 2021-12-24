---
author: Chinmay Deval
categories:
- R
- package
date: "2019-07-02"
draft: false
excerpt: An R package for predicting sorption processes using empirical models
featured: true
layout: single
links:
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/devalc/Sorption
subtitle: ""
tags:
- hugo-site
title: Sorption
---
***
An R package for predicting adsorption processes using empirical models on the laboratory adsorption experiments. Currently it contains functions for the Linear model, Langmuir model (both, linear and non linear forms), and Freundlich model (linear form).         

### Getting Started

These instructions will get you a copy of the "Sorption" up and running on your 
local machine.

### How to Install

Currently the package is hosted only via through Github. 

Install devtools by running following command in your R console: 

```{r}
install.packages("devtools")
```

Now using devtools functionality you can install the Sorption package from Github. Execute following code in your R console:

```{r}
devtools::install_github("devalc/Sorption")
```
### Usage

Once installed the package can be loaded to the system using:
```{r}
library(Sorption)
```
This will also load test data vectors which can be accessed using:

```{r}
test_Ceq , test_Qeq 
```

### Example Usage: Parameters

Parameters for the Freundlich isotherm can be predicted using:
```{r}
FreundlichParameters(test_Ceq, test_Qeq, "test.csv")
```
### Example Usage: Plots

Freundlich isotherm can be plotted using:
```{r}
FreundlichPlot(test_Ceq, test_Qeq, 0.,0.8,0.,0.9)
```