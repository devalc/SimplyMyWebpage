---
author: Chinmay Deval
categories:
- R
- Shiny
date: "2021-11-15"
draft: false
excerpt: A Shiny Web app implementation to assist in targeted management using WEPPcloud simulated outputs. Synthesize multi-scenario, multi-watershed outputs from process-based geospatial model WEPP (WEPPcloud) using this post-processing, interactive visualization, and analysis tool. 
featured: false
layout: single
links:
- icon: door-open
  icon_pack: fas
  name: application website
  url: https://cdeval.shinyapps.io/Viz-WEPPCloud/
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/devalc/Viz-WEPPCloud
subtitle: ""
tags:
- hugo-site
title: Viz-WEPPcloud
---
***
[![](https://img.shields.io/badge/Shiny-shinyapps.io-blue?style=flat&labelColor=white&logo=RStudio&logoColor=blue)](https://cdeval.shinyapps.io/Viz-WEPPCloud/)
<p align="center">
  <img src="vizweppcloud_hex_featured.png" width=60%/>
</p>

A Shiny web application that is a post-processing, interactive tool based on the simulations from the WEPPcloud interface and can be used to identify erosion hotspots and hillslopes that are suitable for targeted management.

At present it has the capability to get WEPPCloud generated hillslope, channel and watershed summary output files and post-processes them in the back end and perform visualizations both (spatial and non spatial plots) based on the user selected variables.

