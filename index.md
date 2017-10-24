---
title       : Developing Data Products - Plot using Plotly
subtitle    : Course 9 - Week 3 - Assignment Presentation
author      : Vasuprad Kanade
job         : Coursera Data Science Specialization
framework   : revealjs        # {io2012, html5slides, shower, dzslides, ...}
revealjs    : {theme: moon, transition: convex}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn
widgets     : [bootstrap, quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
<link href="https://fonts.googleapis.com/css?family=Open+Sans|Permanent+Marker" rel="stylesheet">

<!-- font-family: 'Permanent Marker', cursive; -->
<!-- font-family: 'Open Sans', sans-serif; -->

<style>
.reveal h1 {
    font-size: 2em;
    // color: #0000b3;
    padding-bottom: 10px;
    font-family: 'Permanent Marker', Impact, sans-serif;
}

.reveal h2 {
    font-size: 1.5em;
    //color: #fff7e6;
    padding-bottom: 10px;
    font-family: 'Permanent Marker', Impact, sans-serif;
}


.reveal p, .reveal em {
    padding-bottom: 10px;
    width: 960px;
    font-family: 'Open Sans', Verdana, sans-serif;
}

.reveal p {
    font-size: .75em;
}

.reveal small {
    width: 500px;
}

.reveal .slides {
    text-align: left;
}

.reveal .roll {
    vertical-align: text-bottom;
}

code {
    color: red;
}

.reveal pre code { 
     height: 250px;
}

</style>


# Developing Data Products
---------------------

## Course Project: [Plot using Plotly](https://vasupradkanade.github.io/DevelopingDataProducts_W3/UsingPlotly.html)

Coursera Data Science Specialization

<small> [Vasuprad Kanade](github.com/VasupradKanade) / [LinkedIn](https://www.linkedin.com/in/vasuprad) </small>

<center>
_"Plot IRIS flower data using Plotly"_
</center>


---
# The Assignment 

The goal of this assignment is to:

1. __Create a Web Page Presentation__ using R Markdown that features a plot created with Plotly.

2. __Host the Presentation on GitHub__ that contains few  slides in either Slidify or Rstudio Presenter that is pushed to and hosted on GitHub

---
# The Data

The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by the British statistician and biologist *Ronald Fisher* in his 1936 paper The use of multiple measurements in taxonomic problems as an example of linear discriminant analysis


The data set consists of 50 samples from each of three species of *__Iris__ (Iris setosa, Iris virginica and Iris versicolor)*. Four features were measured from each sample: the length and the width of the sepals and petals, in centimetres. Based on the combination of these four features, Fisher developed a linear discriminant model to distinguish the species from each other.

---
# Code Example
#### Plot IRIS flower data using Plotly
This segment of code selects the relevant data columns, aggregates the three speciees of Iris flower by petal and sepal length.

```r
filename <- "iris.csv"

# Load the CSV file from the local directory
dataset <- read.csv(filename, header=FALSE)

# Set the column names in the dataset
colnames(dataset) <- c("Sepal.Length","Sepal.Width","Petal.Length","Petal.Width","Species")
```

---
# Plot using Plotly
Using ColorBrewer Palette Names


<pre><iframe src="./assets/img/plot1.html" width=750px height=400px allowtransparency="true" scrolling="no" seamless="seamless" frameBorder="0"> </iframe></pre>

