# NottinghamR_Markdown

This is a code is for my [NottinghamR](http://www.meetup.com/NottinghamR-Nottingham-R-Users-Group/events/232383634/) presentation on 11/10/16, discussing RMarkdown.

# Prequisities

To compile presentation you need:

* [pandoc](http://pandoc.org/) (or [RStudio](https://www.rstudio.com/products/rstudio/download3/))
* [Latex compiler](https://miktex.org/)
* [Beamer Metropolis theme](https://github.com/matze/mtheme)

# How to compile

To build:

* PDF version type `pandoc --slide-level 2 -H head.tex -B body.tex -t beamer presentation.md -V theme:metropolis -o output.pdf`
* ioslides version open **presentation.md** in RStudio and click *Compile to HTML*. This option will be automatically selected based on the header settings.
* standard document, 
	* type `pandoc presentation.md -o output.html` , or
	* in file header change `output: ioslides_presentation` to `output: html_document`


