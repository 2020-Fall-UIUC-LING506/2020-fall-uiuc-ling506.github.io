---
layout: default
---

# Project

In order to gain hands-on experience, you will engage in a semester-long project in which you will build a competitive end-to-end machine translation system. Using this system, you will conduct experiments using [data from the 2020 Conference on Machine Translation shared tasks (WMT20)](http://statmt.org/wmt20/index.html). As you progress through the semester, you will document your progress as you write sections of what will ultimately become your end-of-semester final project report.

Following the completion of the Fall 2020 semester, students who wish to continue their projects may participate in continuing research with Professor Schwartz, leading to potential co-authorship on a University of Illinois shared task paper submitted to the 2021 Conference on Machine Translation.


## Proposal

You will begin by researching the [WMT20 news shared task](http://statmt.org/wmt20/translation-task.html) and the [results of the WMT19 news shared task](https://www.aclweb.org/anthology/W19-5301.pdf), selecting a language pair from the WMT20 news shared task, and writing a proposal describing the MT techniques you plan to use as you build a working end-to-end machine translation system for this language pair over the course of the semester.

* Begin by going to [Github Classroom](https://classroom.github.com/a/8agbh932) and cloning the **project** repository. For each of the five project components, there is a corresponding [tex](https://en.wikipedia.org/wiki/XeTeX) file (proposal.tex, litreview.tex, etc).

* You will work locally in the *proposal* branch of your cloned repo.

* Perform background research to identify a language pair and MT approaches known to work well for this language pair:
  * Read the description of the [Shared Task: Machine Translation of News](http://statmt.org/wmt20/translation-task.html) at WMT20
  * Look at the [findings of the WMT19 news shared task](https://www.aclweb.org/anthology/W19-5301.pdf)
  * Browse the [proceedings of WMT19](https://www.aclweb.org/anthology/volumes/W19-53/), with a focus on papers describing submissions to the news shared task. The [proceedings of previous WMTs](https://www.aclweb.org/anthology/venues/wmt/) may also be useful.

* Decide on one language pair from those in the WMT20 news shared task.

* Using [XeLaTeX](https://en.wikipedia.org/wiki/XeTeX), write a project proposal:
  * Begin by compiling proposal.pdf by running `make proposal.pdf`
    * You may use the cl server, [Overleaf](https://www.overleaf.com), or your own machine. 
       * The cl machine is preconfigured with all requisite dependencies.
       * On [Overleaf](https://www.overleaf.com), you will need to configure your project to use XeLaTeX and you will need to include a copy of the Times New Roman font from your local machine in your Overleaf project.
       * On Ubuntu, the following dependencies should suffice: `apt install texlive-xetex latexmk ttf-mscorefonts-installer`
    * Look at the resulting *proposal.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *proposal.tex*. The content of your proposal should describe the language pair and the techniques you plan to employ.
  * Your *proposal.tex* must successfully compile into *proposal.pdf* without errors on the cl server by running `make proposal.pdf`
  
* Ensure that all changes to *proposal.tex* and *project.bib* are committed, and push your *proposal* branch and all its changes to Github.


## Literature review

You will continue your project development by conducting a thorough literature review describing the current state-of-the-art in machine translation for your selected language pair. Your literature review must, at a minimum, cover all shared task submissions for your language pair from WMT19, and should also cover other relevant sources (ACL 2020, etc).

* Create a new branch called *litreview* in your local repo:
  * `git checkout -b litreview`
  
* Write your literature review in *litreview.tex*
  * Copy any relevant text from *proposal.tex* into *litreview.tex*
  * Begin by compiling proposal.pdf by running `make litreview.pdf`
    * Look at the resulting *proposal.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *proposal.tex*. The content of your literature review should thoroughly describe the current state-of-the-art in machine translation for your selected language pair.
  * Look at the resulting *litreview.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Your *litreview.tex* must successfully compile into *litreview.pdf* without errors on the cl server by running `make litreview.pdf`



