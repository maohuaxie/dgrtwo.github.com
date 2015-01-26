---
layout: page
title: "Intermediate Data Science Using R (WS1015)"
description: "Intermediate Data Science Using R Course Website"
category: r
tags: [r, lesson]
---

Welcome to Wintersession 1015, **Intermediate Data Science Using R**. The course takes place from **1/26-30, 11AM-12PM, in McCosh 4**.

Please make sure to complete the following *before* coming to lecture:

* Bring a **fully charged laptop**,
* **Install the latest version of R** (3.1.2), which can be done [here](http://lib.stat.cmu.edu/R/CRAN/). If you already have R installed, make sure your version is **at least 3.1.2**.
* **Install RStudio**, which can be found [here](http://www.rstudio.com/). *Make sure you can open the application,* and have it ready at the start of the session.

R Live Feed
---------------
Ended up a few lines behind? Want to check that your spelling of the last line was correct? No problem: these pages contain the live contents of the file that's being written and executed on the screen. They are synced by Dropbox and may take a few seconds to get up to date. They'll be left up after the class as a record of the code used.

* [Lesson 1: Tidy Data Manipulation I (Monday)](https://www.dropbox.com/s/gjz5j61jpldktpy/WS1015_Lesson1.R?dl=1)

Syllabus
---------------

While you're encouraged to attend every session, you may be able to skip a session that you're particularly familiar with. Similarly, if you have friends that are interested in one topic, but not others, they should feel free to visit just that one session (I won't tell if you don't).

* **Monday: Tidy Data Manipulation I**: In this class we'll teach the [dplyr](http://cran.rstudio.com/web/packages/dplyr/vignettes/introduction.html) package for filtering, merging, and manipulating data with concise syntax. This serves as an introduction to the powerful and popular ["tidy data" framework](http://vita.had.co.nz/papers/tidy-data.pdf).
* **Tuesday: Tidy Data Manipulation II**: How do you turn messy data tidy, and how do you keep it that way? We'll learn to use the [tidyr](https://github.com/hadley/tidyr) package to manipulate the structure of data so it can be analyzed using dplyr and plotted using ggplot2. We'll also learn to use the [broom](https://github.com/dgrtwo/broom) package, which takes many kinds of statistical model objects and turns them into tidy data frames that can be manipulated within this framework.
* **Wednesday: Reproducible Research**: Suppose you've just finished your manuscript, presentation, or homework assignment based on an R analysis. But then you change your R code in a way that **slightly** changes your results- and now you have to go back and replace all of your text, your tables, and your figures- what a hassle! The [knitr](http://yihui.name/knitr/) package solves this, by integrating your code into the same document as your report. [R Markdown](http://rmarkdown.rstudio.com/), meanwhile, lets you format these reports into HTML, PDFs, Word documents, or presentations. You'll have the option of displaying your R code in the document right next to the results (useful for assignments and tutorials) or hiding it (useful for manuscripts and presentations).
* **Thursday: Package Development**: Once you've developed some statistical methods in R, you might want to share your code with the larger community. The most powerful way you can share it is as an R package (just like the ones we've learned this week). We'll go over the steps of creating an R package from scratch. You'll start with a basic skeleton using the [devtools](https://github.com/hadley/devtools) package, document your code with [Roxygen2](http://cran.r-project.org/web/packages/roxygen2/index.html), and write unit tests with [testthat](http://journal.r-project.org/archive/2011-1/RJournal_2011-1_Wickham.pdf). We'll then show how to publish your code on GitHub, and go over how one would submit it to CRAN (the official R package network).
* **Friday: Wild Card**: There are two choices for what will be introduced in Friday's session. You'll choose which in an in-class vote on Monday!
  * **Web Scraping**: Not all data that you want to analyze and visualize comes in neat tab-delimited files- some might be on web pages, in the form of tables and text. We'll learn how to use the [rvest](https://github.com/hadley/rvest) package to download and parse ("scrape") this content so it can be analyzed in R, using examples like the [Internet Movie Database](http://www.imdb.com/) (IMDb).
  * **Interactive Web Visualizations**: Some data visualizations deserve to be interactive. The [Shiny](http://shiny.rstudio.com/) web application framework lets you create and publish interactive data visualizations, including charts, maps, and timelines, using just R code (no knowledge of HTML or Javascript required). Shiny is great for class presentations, research projects, and analytics dashboards: see [here](http://shiny.rstudio.com/gallery/) and [here](http://www.showmeshiny.com/) for some great galleries.

Other Links
----------------

* [R Error Message Cheat Sheet](errors/): contains some common R error messages. If you get an error while running a line that you expect to work (perhaps because you saw it on the screen), check these examples before you go to the Google docs. (In particular, check your spelling and capitalization carefully).
* [Resources for future learning](/RData/resources/) A page of additional resources for learning R

Relevant Code
---------------

**Lesson 1**: We'll be studying a set of United Nations voting data that can be found here:

* Anton Strezhnev; Erik Voeten, 2013, "United Nations General Assembly Voting Data", <a href="http://hdl.handle.net/1902.1/12379">hdl:1902.1/12379</a> UNF:5:s7mORKL1ZZ6/P3AR5Fokkw== Erik Voeten [Distributor] V7 [Version]

You can download it using the following line of code:

    load(url("http://dgrtwo.github.io/files/undata-213.RData"))

And load the descriptions dataset with:

    load(url("http://dgrtwo.github.io/files/descriptions-213.RData"))