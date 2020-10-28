---
layout: default
---

# Project

In order to gain hands-on experience, you will engage in a semester-long project in which you will build a competitive end-to-end machine translation system. Using this system, you will conduct experiments using [data from the 2020 Conference on Machine Translation shared tasks (WMT20)](http://statmt.org/wmt20/index.html). As you progress through the semester, you will document your progress as you write sections of what will ultimately become your end-of-semester final project report.

Following the completion of the Fall 2020 semester, students who wish to continue their projects may participate in continuing research with Professor Schwartz, leading to potential co-authorship on a University of Illinois shared task paper submitted to the 2021 Conference on Machine Translation.


## Proposal

You will begin by researching the [WMT20 news shared task](http://statmt.org/wmt20/translation-task.html) and the [results of the WMT19 news shared task](https://www.aclweb.org/anthology/W19-5301.pdf), selecting a language pair from the WMT20 news shared task, and writing a proposal describing the MT techniques you plan to use as you build a working end-to-end machine translation system for this language pair over the course of the semester.

* Begin by going to [Github Classroom](https://classroom.github.com/a/8agbh932) and cloning the **project-report** repository. For each of the five project components, there is a corresponding [tex](https://en.wikipedia.org/wiki/XeTeX) file (01-proposal.tex, 02-litreview.tex, etc).

* You will work locally in the *proposal* branch of your cloned **project-report** repo.

* Perform background research to identify a language pair and MT approaches known to work well for this language pair:
  * Read the description of the [Shared Task: Machine Translation of News](http://statmt.org/wmt20/translation-task.html) at WMT20
  * Look at the [findings of the WMT19 news shared task](https://www.aclweb.org/anthology/W19-5301.pdf)
  * Browse the [proceedings of WMT19](https://www.aclweb.org/anthology/volumes/W19-53/), with a focus on papers describing submissions to the news shared task. The [proceedings of previous WMTs](https://www.aclweb.org/anthology/venues/wmt/) may also be useful.

* Decide on one language pair from those in the WMT20 news shared task.

* Using [XeLaTeX](https://en.wikipedia.org/wiki/XeTeX), write a project proposal:
  * Begin by compiling 01-proposal.pdf by running `make 01-proposal.pdf`
    * You may use the cl server, [Overleaf](https://www.overleaf.com), or your own machine. 
       * The cl machine is preconfigured with all requisite dependencies.
       * On [Overleaf](https://www.overleaf.com), you will need to configure your project to use XeLaTeX and you will need to include a copy of the Times New Roman font from your local machine in your Overleaf project.
       * On Ubuntu, the following dependencies should suffice: `apt install texlive-xetex latexmk ttf-mscorefonts-installer`
    * Look at the resulting *01-proposal.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *01-proposal.tex*. The content of your proposal should describe the language pair and the techniques you plan to employ.
  * Your *01-proposal.tex* must successfully compile into *01-proposal.pdf* without errors on the cl server by running `make 01-proposal.pdf`
  
* Ensure that all changes to *01-proposal.tex* and *project.bib* are committed, and push your *proposal* branch and all its changes to Github.


## Literature review

You will continue your project development by conducting a thorough literature review describing the current state-of-the-art in machine translation for your selected language pair. Your literature review must, at a minimum, cover all shared task submissions for your language pair from WMT19, and should also cover other relevant sources (ACL 2020, etc).

* Create a new branch called *litreview* in your local **project-report** repo:
  * `git checkout -b litreview`
  
* Write your literature review in *02-litreview.tex*
  * Copy any relevant text from *01-proposal.tex* into *02-litreview.tex*
  * Begin by compiling 02-litreview.pdf by running `make 02-litreview.pdf`
    * Look at the resulting *02-litreview.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *02-litreview.tex*. The content of your literature review should thoroughly describe the current state-of-the-art in machine translation for your selected language pair.
  * Look at the resulting *02-litreview.pdf*. The content of your work should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Your *02-litreview.tex* must successfully compile into *02-litreview.pdf* without errors on the cl server by running `make 02-litreview.pdf`

* Ensure that all changes to *02-litreview.tex* and *litreview.bib* are committed, and push your *litreview* branch and all its changes to Github.



## Checkpoint 1

* Go to [Github Classroom](https://classroom.github.com/a/8agbh932) and clone the **project-scripts** repository.
* In your **project-scripts** repository:
  * Work in the *checkpoint1* branch
  * Edit *run.tape*, writing [ducttape](https://github.com/ExperimentWith/ducttape/releases/tag/v0.4) *task*s and a *plan* to run your scripts. Every task must be thoroughly documented.
  * Your scripts must successfully execute a complete experiment on a very scaled down data set when `ducttape run.tape -y` is executed
  * Ensure that all changes to *run.tape* are committed, and push your changes to Github.

  
* Continue your writing in *03-checkpoint1.tex*
  * Copy any relevant text from *02-litreview.tex* into *03-checkpoint1.tex*
  * Begin by compiling 03-checkpoint1.pdf by running `make 03-checkpoint1.pdf`
    * Look at the resulting *03-checkpoint1.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *03-checkpoint1.tex*. You will now add an Approach section, with Data and Methods subsections.
  * Look at the resulting *03-checkpoint1.pdf*. The content of your work should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Your *03-checkpoint1.tex* must successfully compile into *03-checkpoint1.pdf* without errors on the cl server by running `make 03-checkpoint1.pdf`

* Ensure that all changes to *03-checkpoint1.tex* and *checkpoint1.bib* are committed, and push your *checkpoint1* branch and all its changes to Github.


## Checkpoint 2

* In your **project-scripts** repository:
  * Create a new branch called *checkpoint2* in your local **project-scripts** repo:
    * `git checkout -b checkpoint2`
    * Work in the *checkpoint2* branch
  * Continue work on run.tape, making any necessary changes to run on a complete data set
  * Your scripts must successfully execute your plan when `ducttape run.tape -y` is executed
  * Ensure that all changes to *run.tape* are committed, and push your *checkpoint2* branch and its changes to Github.
  
* Continue your writing in *04-checkpoint2.tex*
  * Create a new branch called *checkpoint2* in your local **project-report** repo:
    * `git checkout -b checkpoint2`
    * Work in the *checkpoint2* branch
  * Copy any relevant text from *03-checkpoint1.tex* into *04-checkpoint2.tex*
  * Begin by compiling 04-checkpoint2.pdf by running `make 04-checkpoint2.pdf`
    * Look at the resulting *04-checkpoint2.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *04-checkpoint2.tex*. You will now add a Preliminary Results section.
  * Look at the resulting *04-checkpoint2.pdf*. The content of your work should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Your *04-checkpoint2.tex* must successfully compile into *04-checkpoint2.pdf* without errors on the cl server by running `make 04-checkpoint2.pdf`

* Ensure that all changes to *04-checkpoint2.tex* and *checkpoint2.bib* are committed, and push your *checkpoint2* branch and all its changes to Github.


## Final report

* In your **project-scripts** repository:
  * Create a new branch called *dec2020* in your local **project-scripts** repo:
    * `git checkout -b dec2020`
    * Work in the *dec2020* branch
  * Continue work on run.tape, making any necessary changes to run all baselines and experimental variants on a complete data set
  * Your scripts must successfully execute your entire end-to-end experiment when `ducttape run.tape -y` is executed
  * Ensure that all changes to *run.tape* are committed, and push your *dec2020* branch and its changes to Github.
  
* Continue your writing in *05-report.tex*
    * Create a new branch called *dec2020* in your local **project-report** repo:
    * `git checkout -b dec2020`
    * Work in the *dec2020* branch
  * Copy any relevant text from *04-checkpoint2.tex* into *05-report.tex*
  * Begin by compiling 05-report.pdf by running `make 05-report.pdf`
    * Look at the resulting *05-report.pdf*. The content of your proposal should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Edit *05-report.tex*. The content of your literature review should thoroughly describe the current state-of-the-art in machine translation for your selected language pair.
  * Look at the resulting *05-report.pdf*. The content of your work should be at least as long as the [lorem ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) dummy text provided therein.
  * Your *05-report.tex* must successfully compile into *05-report.pdf* without errors on the cl server by running `make 05-report.pdf`

* Ensure that all changes to *05-report.tex* and *checkpoint2.bib* are committed, and push your *dec2020* branch and all its changes to Github.
