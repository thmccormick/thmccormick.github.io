+++
title = "OpenVA"

date = 2018-09-09T00:00:00
# lastmod = 2018-09-09T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.

# Add menu entry to sidebar.
linktitle = "OpenVA"
[menu.software]
  parent = "Verbal autopsy"
  weight = 8

# Featured image.
# Uncomment below lines to use.
# [header]
# image = "headers/getting-started.png"
# caption = "Image credit: [**Academic**](https://github.com/gcushen/hugo-academic/)"
+++

Verbal autopsy (VA) is a survey-based tool widely used to infer cause of death (COD) in regions without complete-coverage civil registration and vital statistics systems. In such settings, many deaths happen outside of medical facilities and are not officially documented by a medical professional. VA surveys, consisting of signs and symptoms reported by a person close to the decedent, are used to infer the cause of death for an individual, and to estimate and monitor the cause of death distribution in the population. There are three components required for analyzing VAs: (i) VA survey data, (ii) inputs that give information about the association between symptoms and causes, and (iii) a statistical or algorithmic method for assigning a likely cause. For each of these pieces, there are several variants produced independently by research and policy organizations. Incompatibility between components means that there is no systematic way of applying and comparing different methods without laborious, idiosyncratic data conversion. The openVA package aims to simplify comparison across existing VA tools through a standardized pipeline that is compatible with all openly available methods and data structure. It provides an open-sourced, R implementation of four most widely used VA methods: InterVA-4, InSilicoVA, Naive Bayes Classifier, and Tariff. It supports different data input and output formats, and customizable in- formation about the associations between causes and symptoms. The paper discusses the relevant algorithms, the implementations in R and some additional information on advanced model fitting with InSilicoVA.

+ [CRAN](https://cran.r-project.org/web/packages/openVA/index.htm). 
+ [Website](http://openva.net/). 
+ [Slides](http://zehangli.com/talks/openVA-slides.html) from WHO VA Working Group. 
+ [Vignette](http://zehangli.com/openVA/openVA-vignette_2017.pdf).