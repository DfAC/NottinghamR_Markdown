---
title: Take it easy with markdown
author:
- LKB
fontsize: 11pt
output: ioslides_presentation
# output: html_document
<!-- output:
  beamer_presentation:
    theme: metropolis
    slide_level: 2
    includes:
      in_header: head.tex
      before_body: body.tex
      after_body: tail.tex -->

---


# Introduction

## Latex vs Word

![](http://i.stack.imgur.com/6bRxX.png "Word or Latex")


<div class="notes">

Let's start by discussing apparent conflict


Microsoft Office is the most widely used office suite for a number of years now, mostly due to relative easy learning curve and  initial flexibility.

Today I am going to discuss tools that you can use to carry out some of Microsoft Office tasks. The aim behind this talk is to address the balance between two statements:

* Change for the sake of change is rarely a sensible use of time.
* Tools have to fit the purpose.

Before I venture any further I would like to discuss topic that seems a bit unrelated, that is Word vs Latex discusion.

</div>

## Word perception

ADD FIGURE

[An Efficiency Comparison of Document Preparation Systems Used in Academic Research and Development](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0115069)

<div class="notes">
A common conception is that Latex is predominantly of academic use, due to a steep learning curve, and while it handles complex equation and big documents well, it fares poorly when comparing the writing efficiency, especially when the grammar is considered.
Latex users argument can be presented in  a simple graph as


Microsoft Office user argument would be the first sentence and highligh of how easy it is to start
Academic use paragim, a steep learning curve and compex syntax even lead to [a academic paper](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0115069). Discussion of any other tools, has to address those comments as well.
</div>

## Latex perception

![](http://www.pinteric.com/pic/miktex.gif)

# Re-framing the question

## Change

* Change for the sake of change is rarely a sensible use of time.
* Tools have to fit the purpose.

<div class="notes">

The aim behind this talk is to address the balance between two statements:

* Change for the sake of change is rarely a sensible use of time.
* Tools have to fit the purpose.

</div>

## What do I mean?

* Does content matters? Or the visuals?
* what is the most productive use of my time?
* How can I maintain the contribution from others? How do we archive documents?
* What about data fidelity?


<div class="notes">

So before I progress any further in this discussion I would like to bring attention to my second sentence. Let's ask some questions:

</div>

## Does content matters?

![Content is king](https://pixabay.com/static/uploads/photo/2013/07/18/10/56/graph-163509_960_720.jpg)

## Who send what?

![Entropy build up](./pics/disaster.jpg)

## Which is my latest copy?

* report_01.doc
* report_02.doc
* report_03_revByJim.doc
* report_04_changes.doc
* report_05_final.doc
* report_05_finalFinal.doc
* report_05_finalFinal_FINAL.doc
* report_05_finalFinal_FINAL_send.doc

## Deep Work

![<http://calnewport.com/books/deep-work/>](http://www.evidenceinmotion.com/wp-content/uploads/2016/04/Deep-Work.jpg)


## Social aspect

![https://rpubs.com/ykashou92/eq_wmap](http://i0.wp.com/david-lallemant.com/wp-content/uploads/2014/10/EQ_Website.jpeg)

* [Hawkers in Singapore](https://rpubs.com/JoshMah/168498)
* [interactive plots](https://plot.ly/r/)


## Big guys open source

![http://pandoc.org/](pics/Tensorflow.png)


# Tools

## Markdown - Keep it simple

![https://daringfireball.net/projects/markdown/](http://i.imgur.com/Pghp2CU.png){ width=100% }


## Markdown - its flexible

![Spoil for choice?](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c5/Gelato_in_Las_Vegas_in_2007.jpg/1280px-Gelato_in_Las_Vegas_in_2007.jpg ""){ width=50% }


<div class="notes">

 Markdown was created to simplify HTML, but with the right tools, your Markdown files can easily be converted to many different formats!

</div>


## One to rule them all

![http://pandoc.org/](https://sachsmc.github.io/knit-git-markr-guide/knitr/img/knitr-workflow.png)


## Control the time

![How good is your version control](d:\tmp\Dropbox\Edu\Presentations\R_meetup\pics\Git_flow.png){ height=50% }


## Let's talk about this

* Which tools are missing?
* WHich are important?
* How easy it is to implement?

## Goying b


# Demo

## inspiration

<>

## report

```
pandoc 01Markdown.md --output=01Markdown.html
pandoc 02_Rmd+references.rmd --output=02_Rmd+references.html
pandoc 02_Rmd+references.rmd --output=02_Rmd+references.docx
pandoc 03_FinalReport.rmd --output= 03_FinalReport.docx
```

## presentation

```
pandoc -t beamer presentation.md -o simple.pdf
pandoc --slide-level 2 -H head.tex -B body.tex -t beamer presentation.md -V theme:metropolis -o output.pdf
```

## future work

* running code inside presentation
* [converting back from MSc Office](http://pandoc.org/demos.html)
* animations + interactive content


#summary

* simple tool allow to focus on content
* simple does not mean not flexible


## useful links

* R
  * [RMarkdown](http://rmarkdown.rstudio.com/)
  * [ioslides](http://rmarkdown.rstudio.com/ioslides_presentation_format.html)
  * [knit](https://sachsmc.github.io/knit-git-markr-guide/knitr/knit.html)
  *
* Pandoc
  * [try online](http://pandoc.org/try/)
  * [check demos](http://pandoc.org/demos.html)
* git
  * [guide](http://rogerdudler.github.io/git-guide/)
  * [try yourself](https://try.github.io/levels/1/challenges/10)