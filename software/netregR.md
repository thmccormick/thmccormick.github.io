+++
title = "netregR"

date = 2018-09-09T00:00:00
# lastmod = 2018-09-09T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.

# Add menu entry to sidebar.
linktitle = "netregR"
[menu.software]
  parent = "Networks"
  weight = 2

# Featured image.
# Uncomment below lines to use.
# [header]
# image = "headers/getting-started.png"
# caption = "Image credit: [**Academic**](https://github.com/gcushen/hugo-academic/)"
+++

Regress network responses (both directed and undirected) onto covariates of interest that may be actor-, relation-, or network-valued. In addition, compute principled variance estimates of the coefficients assuming that the errors are jointly exchangeable. Missing data is accommodated. Additionally implements building and inversion of covariance matrices under joint exchangeability, and generates random covariance matrices from this class. For more detail on methods, see [Marrs, Fosdick, and McCormick (2017)](https://arxiv.org/abs/1701.05530).

+ [CRAN](https://cran.r-project.org/web/packages/netregR/index.html)