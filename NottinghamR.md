---
#title: Take it easy with markdown
#author:
#- LKB
fontsize: 11pt
#output: ioslides_presentation
output: html_document
<!-- output:
  beamer_presentation:
    theme: metropolis
    slide_level: 2
    includes:
      in_header: head.tex
      before_body: body.tex
      after_body: tail.tex
      keep_tex: true -->

---


# Introduction

<div class="notes">

[NottinghamR talk](http://www.meetup.com/NottinghamR-Nottingham-R-Users-Group/events/232383634/)

Welcome. My name is. A bit of personal story:

* I started with Word for MSc
* Latex for PhD, found it amazing and extremely frustrating
* at similar time discovered interactive RStudio, python
* looked into simplifying my presentations

* 'f' enable fullscreen mode
* 'w' toggle widescreen mode
* 'o' enable overview mode
* 'h' enable code highlight mode
* 'p' show presenter notes


</div>

## Questionnaire results

![<http://bit.ly/RMeetupNottingham>](./pics/questionnaire.jpg){ width=80% }

* Most interest in:
	* general understanding
	* making presentation + report
* more RStudio users than Microsoft Office
	* git and Markdown more popular than Latex or Beamer
	* More RMarkdown users than Markdown !


## Latex vs Word

![Word or Latex](http://i.stack.imgur.com/6bRxX.png)


<div class="notes">

A common perception is that:

* Microsoft Office is the most widely used office suite for a number of years now, mostly due to relative easy learning curve and  initial flexibility.
* Latex is predominantly of academic use, due to a steep learning curve, and while it handles complex equation and big documents well, it fares poorly when comparing the writing efficiency, especially when the grammar is considered.

</div>

## Latex perception

![Complex but worth it](http://www.pinteric.com/pic/miktex.gif)

<div class="notes">

* <http://www.schuetzler.net/blog/latex-vs-word-again/>
 	* Latex separates the formatting of the document and the content of the document in a decent, logical way.
* [another](http://serialmentor.com/blog/2014/12/27/post-publication-review-of-the-plos-one-paper-comparing-ms-word-and-latex-how-not-to-compare-document-preparation)
	* Even though cumbersome and has its quirks, LaTeX is highly predictable

</div>

## Microsoft Office perception


![[An Efficiency Comparison of Document Preparation Systems Used in Academic Research and Development](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0115069)](http://journals.plos.org/plosone/article/figure/image?size=large&id=info:doi/10.1371/journal.pone.0115069.g004)


<div class="notes">

Microsoft Office user argue:

* easy it is to start
* flexible and comprehensive
* Latex with steep learning curve and complex syntax and poor visuals is just not good for industry

</div>



# Re-framing the question

## Change

* Change for the sake of change is rarely a sensible use of time.
* Tools have to fit the purpose.

<div class="notes">

The aim behind this talk is to address the balance between those two statements.


## What do I mean?

* Does content matters? Or the visuals?
* what is the most productive use of my time?
* How can I maintain the contribution from others? How do we archive documents?
* What about data fidelity?

</div>

## Does content matters?

![Content is king](https://pixabay.com/static/uploads/photo/2013/07/18/10/56/graph-163509_960_720.jpg)


## Sum of all parts

![Complexity vs time spend](http://www.intmath.com/blog/wp-content/images/2015/03/exponential-curve.png)

## Who send what?

![Entropy builds up](./pics/disaster.jpg)

## Which is my latest copy?

* report_01.doc
* report_02.doc
* report_03_revByJim.doc
* report_04_changes.doc
* report_05_final.doc
* report_05_finalFinal.doc
* report_05_finalFinal_FINAL.doc
* report_05_finalFinal_FINAL_send.doc

## Social aspect

![https://rpubs.com/ykashou92/eq_wmap](http://i0.wp.com/david-lallemant.com/wp-content/uploads/2014/10/EQ_Website.jpeg){ width=70% }

* [Hawkers in Singapore](https://rpubs.com/JoshMah/168498)
* [interactive plots](https://plot.ly/r/)

## Deep Work

![<http://calnewport.com/books/deep-work/>](http://www.evidenceinmotion.com/wp-content/uploads/2016/04/Deep-Work.jpg)


## Big guys open source

![](pics/Tensorflow.png)


# Tools

## RStudio

![](https://teespring-storecontent.s3.amazonaws.com/FW6s2ljYB6HuZgDe15SiOQ_store_header_image)


## Markdown - Keep it simple

![https://daringfireball.net/projects/markdown/](http://i.imgur.com/Pghp2CU.png){ width=120% }


<div class="notes">

 Markdown was created to simplify HTML, but with the right tools, your Markdown files can easily be converted to many different formats!

</div>


## One to rule them all

![<http://pandoc.org/>](https://sachsmc.github.io/knit-git-markr-guide/knitr/img/knitr-workflow.png)


## Control the time

![How good is your version control](d:\tmp\Dropbox\Edu\Presentations\R_meetup\pics\Git_flow.png)


# Some downsides

## Change

* Change for the sake of change is rarely a sensible use of time.
	* How are we going to interact with others?
* Tools have to fit the purpose.
	+ How many tools do I need to learn?
	+ Who maintain those tools?

<div class="notes">

The aim behind this talk is to address the balance between those two statements.

</div>

## How many tools are we using?

![complexity vs effort](http://www.intmath.com/blog/wp-content/images/2015/03/exponential-curve.png)


## Markdown - its too flexible

![Spoil for choice?](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c5/Gelato_in_Las_Vegas_in_2007.jpg/1280px-Gelato_in_Las_Vegas_in_2007.jpg "")

<div class="notes">

There are too many ways of doing things and too many flavours of markdown.

</div>

# Let's talk about this

<div class="notes">

* Which tools are missing?
* WHich are important?
* How easy it is to implement?

## notes from the audience

</div>

# Demo time


## Report example

```
pandoc 01Markdown.md --output=01Markdown.html
pandoc 02_Rmd+references.rmd --output=02_Rmd+ref.html
pandoc 02_Rmd+references.rmd --output=02_Rmd+ref.docx
pandoc 03_FinalReport.rmd --output= 03_FinalRep.docx
```

## Presentation example

```
pandoc -t beamer presentation.md -o simple.pdf
pandoc --slide-level 2 -H head.tex -B body.tex -t beamer
 presentation.md -V theme:metropolis -o Rpresentation.pdf
```

## Future work

* running R code inside presentation
* [converting back from MSc Office](http://pandoc.org/demos.html) - seamless integration
* animations + interactive content
* [Adding Excel](https://beckmw.wordpress.com/2014/06/05/a-simple-workflow-for-using-r-with-microsoft-office-products/)
* Markdown to PowerPoint


# Summary

## Take away notes

* Markdown is one of 20-80 tools - it will cover most of problems with small effort
* content beats visuals
* set of small dedicated tools allow better flexibility and low entropy

## useful links

* R
	+ [RMarkdown](http://rmarkdown.rstudio.com/)
	+ [ioslides](http://rmarkdown.rstudio.com/ioslides_presentation_format.html)
	+ [knit](https://sachsmc.github.io/knit-git-markr-guide/knitr/knit.html)
* [Online markdown](http://dillinger.io/)
* Pandoc
	+ [try online](http://pandoc.org/try/)
	+ [check demos](http://pandoc.org/demos.html)
* git
	+ [guide](http://rogerdudler.github.io/git-guide/)
	+ [try yourself](https://try.github.io/levels/1/challenges/10)

\setbeamercolor{background canvas}{bg=blueBgd!60}

## Thank you

Can you fill in the feedback at <http://bit.ly/LKBFeedback>?



lkbonenberg@gmail.com

@LKBLab


<div class="notes">
http://www.slideshare.net/LukaszKosmaBonenberg
</div>