# NottinghamR Markdown Presentation

This is a code is for my [NottinghamR](http://www.meetup.com/NottinghamR-Nottingham-R-Users-Group/events/232383634/) presentation from the 11/10/16, discussing RMarkdown.

# Prerequisites

To compile presentation you need:

* [pandoc](http://pandoc.org/) (or [RStudio](https://www.rstudio.com/products/rstudio/download3/))
* [Latex compiler](https://miktex.org/)
* [Beamer Metropolis theme](https://github.com/matze/mtheme)

# How to compile presentation

To build:

* for a PDF version, [available here](http://www.slideshare.net/LukaszKosmaBonenberg/nottingamr-presentation), type in terminal: `pandoc --slide-level 2 -H head.tex -B body.tex -t beamer presentation.md -V theme:metropolis -o output.pdf`
* ioslides version open **presentation.md** in RStudio and click *Compile to HTML*. This option will be automatically selected based on the header settings.
* standard document,
	* type `pandoc presentation.md -o output.html` , or
	* in file header change `output: ioslides_presentation` to `output: html_document`

# Report

More information about the presented report can be found at [my blog](http://dfac.github.io/code/2016/02/16/Writing-Articles-with-Markdown/).