---
name: "BeeR - session 1"
date: "2023-11-02"
author: "Hugo Soubrier"
---

# How to get help on R ?

Like any other programming language R can be challenging, and it is VERY common for any R users to get stuck and requiring some help.

- Did you forget a function name ? Or maybe you forgot what a function does and what arguments it takes ?

- You are wondering if there is already an existing package doing what you are trying to do with your data ?

- You are completely confused about how to filter this dataframe ?

- You want to know if someone else struggled a very specific thing with your favorite package ?

- You need someone to explain you how the `pivot_longer()` and `pivot_wider()` functions work ?

- You finished your summer book and you are looking for something thrilling to read before bed ?

The mighty Internet is full of various resources to help you, and R has a great community of users that happily help each other !

## `?help` function and documentations

First let's start with the beginning, you can access informations about functions using the `?help` function. Just type a `?` before an empty function to get this function documentation in the Helper pane (if using Rstudio).

```
?filter()
```

This will give you information about the `filter()` function:

1. what this function does
2. The arguments it takes
3. The value it outputs
4. Use case examples

Nearly every functions in R have documentations, and these are accessible offline ! It is the starting point to look for answers !

## Vignettes & Package websites

`?help` function and documentation is useful if you actually know the name of the function. This is not always the case, or you may want to look into a package see if there are other useful functions for you. In this case it is useful to have a look at the package `vignette` (if the package has one). They are long-form guide, that describe the target problems that a package is trying to adress.

```
browseVignettes()
```

to access all vignettes for packages installed on your R. Otherwise type

```
vignette("colwise", package = "dplyr")
```
to access specific vignette inside a package.

With recent packages, vignettes are also combined into a package website, which provides all informations and further resources regarding the package. See this example of the `gtsummary` package

https://www.danieldsjoberg.com/gtsummary/index.html

## More advanced: GitHub repo & issues

For advance cases where you want to know if a package/function does a very specific thing, or if you want more information on the back-end of the functions you could directly check the code on the GitHub repository for the package. This is where all the code/files and revision history is stored. Because R is an open source language, this is open to anyone to inspect, or even copy. This is an example of a GitHub repository:

https://github.com/R4EPI/epikit

If you have the skills (and authors agree), you can contribute to a package, or copy them to add your own tweaks to them. Also, this is where you can find the associated *GitHub issues*, points/problems/suggestions that people have mentionned to the package authors.

## The internet is your friend

Keep in mind that few people program everyday completely offline. Most of us are frequently browsing internet for solutions, or because we forgot how to do some things. If you get stuck on a problem, a *quick browser search* should be your next step after checking functions and package documentation.

At the start of your R learning quest, most of your problems have already been encountered by other users. You will improve your programming skills when you will be able to efficiently search for solutions online.

When doing an internet search you need **key words** Always mention *R programming language* to force searches on it and exclude python or other languages. The more generic is the question, and the less likely you will rapidly find an answer. If you are using `tidyverse` / `dplyr` or specific functions to solve a problem then *you need to mention them in your search*. Be as specific as possible ! 

## Questions & Answers forums

You will find most of your answers on Q&A forums. You can read discussion threads if your problem was already adressed, or you can write a question yourself. Just bear in mind that this require **reproducible examples** (to be covered in a future BeeR session).

### Stack Overflow

> https://stackoverflow.com/

*Every programmer has a tab open to Stack Overflow !* This is the bible for programming questions and discussions. You will find most of your issues here. To make sure that your browser search sends you to appropriate Stack Overflow discussions make sure you mention R programming. many programming languages use similar terminologies.

### Applied Epi Community forum

> https://community.appliedepi.org/

The [Applied Epi NGO](https://appliedepi.org/) has a nice Q&A forum on which you can find all sort of discussion specifically on R for Epidemiology.

### Posit Community

> https://community.rstudio.com/

Posit (ex R-studio) also provides a Q&A forum called the Posit community. You can find a lot of useful discussions specific to R, but also Posit IDE (R-studio).

Check also the [Posit Cloud guides](https://posit.cloud/learn/guide). Nice, small introductionary exercises to R.

# Useful R resources

## Bookdowns

A lot of resources on R are free digital books called `bookdown`. There are A LOT of them out there. They range from very straightforward to very thorough and detailled resources on a specific aspect of R. 

### Big Book of R

> https://www.bigbookofr.com/

if you do not know where to start, or are unsure that a `bookdown` exist for your topic of interest, start by browsing the giant [Big Book of R](https://www.bigbookofr.com/) which aims at centralising every R-related programming book. 

### R for Data Science (R4DS)

>https://r4ds.had.co.nz/

[R for Data Science](https://r4ds.had.co.nz/) is **THE** book to read if you which to learn R for generic science. It will thorougly cover all of the bases for a great undersatnding of R, and all of it is applicable to Epidemiology.

### The Epidemiologist R handbook

The [Applied Epi NGO](https://appliedepi.org/) actually started by a great book called the [R for Epidemiologist Handbook](https://epirhandbook.com/en/). It is a bible for anyone using R applied to Epidemiology. It is also a great introduction resource for more complex topics such as `ggplot2`, `Rmarkdown` or dashboards (yey)

## Special visualisations

Here is a non-exaustive list of resources for visualisations in R 

### ggplot2 bookdown 

There are many of them ! But this one by Hadley Wickham (R4DS book) is a great start. 

> https://ggplot2-book.org/

### The R graph Gallery

This is a collection of R-made charts. You can browse through all the charts to get inspired, or you can have a look at the reproducible examples would you want to try them ! 

> https://r-graph-gallery.com/

### From data to Viz

This website is great for anyone who has data, and want to display them but is unsure how to go for it. It will help you choose the best visualisations for your data, also pointing out the pros/cons how each method.

> https://www.data-to-viz.com/

## Others fun stuff

### R weekly blog
> https://rweekly.org/about

This is a cool weekly blog that allows you to keep track of all the new stuff going around in the R community. 

### Tidy tuesday

> https://www.tidytuesday.com/

This is a weekly podcast and community challenge going on twitter. Every Tuesday a dataset is released for you to try some data manipulations and visualisations which you can share on Twitter. It is also a great way of checking what other R users do, and get inspired from them ! 
