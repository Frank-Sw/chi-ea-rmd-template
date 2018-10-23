# ACM CHI Extended Abstracts R Markdown Template
This R package provides a template for writing ACM CHI Extended Abstract papers in R Markdown, and compiling to PDF via the LaTeX templates from the 2017 ACM Master Article Template (v. 1.55).

## Overview
Using a tool like [R Markdown](https://rmarkdown.rstudio.com) to write scientific papers makes your work more transparent and reproducible, and reduces the risk of introducing errors by manually transfering results from statistical software to manuscript.

However, getting R Markdown to [play nicely with the latest ACM LaTeX templates can be tricky](https://ulriklyngs.com/blog/acm-articles-with-r-markdown).

This R package makes it easy, by providing a ready-made .Rmd template with YAML metadata and body text illustrations of what you need to know, which compiles to the latest CHI Proceedings (used for CHI'19 submissions) format via the [official 2017 ACM Master Article LaTeX template](https://www.acm.org/publications/proceedings-template).

## Installation
``` r
# The package isn't on CRAN yet - install the development version from GitHub:
# install.packages("devtools")
devtools::install_github("ulyngs/chi-ea-rmd-template")
```

## Usage
The easiest way to use the template is with RStudio, via File -> New File -> R Markdown...
In the dialog box, click 'From Template', then find the new 'ACM CHI Extended Abstracts 2018 {CHIEA2018}' option, choose a name for what you'd like to make (e.g. 'Test'), then click OK:
![R Markdown template dialog](man/1_template.png "R Markdown template dialog")

A new folder named *Test* is created, and you see an open **Test.Rmd** file:
![Test.Rmd with illustration content](man/2_rmd.png "Test.Rmd with illustration content")

If you click 'Knit', it compiles to the example PDF output with the illustration content from **Test.Rmd**:
![Compiled result - PDF output in CHI Extended Abstracts format](man/3_pdf.png "Compiled result - PDF output in CHI Extended Abstracts format")

It also keeps the intermediary generated **Test.tex** file from which the PDF output was created:
![Intermediary Test.tex from which the PDF output was created](man/4_tex.png "Intermediary Test.tex from which the PDF output was created")

Now go ahead and replace the content of **Test.Rmd** with your own fantastic work!
