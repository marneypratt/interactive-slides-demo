# Creating Interactive Slides with Quarto

**Author:** Dr. Marney Pratt, 
Senior Laboratory Instructor,
Biological Sciences Department,
Smith College, Northampton, MA

**Last updated:** May 1, 2026

It is best to get timely feedback on understanding. However, it is rarely possible to have an expert or instructor give individualized feedback right away. Thus, having tools that can give a learner immediate feedback is helpful for learning. 

You can use Quarto along with extensions to create interactive slides with multiple choice questions that give feedback right away.

This is a demonstration for how to use the Quarto presentation format (revealjs) with the Quiz for Quarto extension to create interactive slides.

## Getting Started

1) Start by creating a new Quarto file and choosing the Quarto Presentation option. (Make sure you have [installed Quarto](https://quarto.org/docs/get-started/) first and then chosen a tool such as Rstudio, Positron, VS Code, or Jupyter to run Quarto in)

2) Follow instructions to install the [quiz extension for Quarto](https://github.com/parmsam/quarto-quiz) using the terminal (see additional instructions here about [installing Quarto extensions](https://quarto.org/docs/extensions/managing.html))

3) Use the "dichotomous-key-demo.qmd" file as a template/example to base your own slides off of.


## Tips & Resources

-  See the [Quarto documentation for how to format Revealjs presentation slides](https://quarto.org/docs/presentations/revealjs/) 
-  See additional [extensions for Revealjs Quarto Slides](https://quarto.org/docs/extensions/listing-revealjs.html)
-  [Slidecrafting-Making beautiful slides with reveal.js and Quarto](https://slidecrafting-book.com/)
-  Use lightbox to make images that you can click to zoom. Add the code below into the yaml


```r
format:
  revealjs:
    lightbox: true
```

## Publishing

There are several places you can publish Quarto slides

-  [Publishing Basics](https://quarto.org/docs/publishing/) (compares different options)
-  Use instructions from [Happy Git and GitHub for the useR](https://happygitwithr.com/) to get setup with version control

-  This demo was published using GitHub Pages using the [Publish Command](https://quarto.org/docs/publishing/github-pages.html#publish-command) method using the following steps

    -  I created a GitHub repository first and then created a Quarto Project associated with it
    -  I created [my home website](https://marneypratt.github.io/) on [GitHub Pages](https://docs.github.com/en/pages/quickstart) 
    -  When ready to publish my slides, I 
        -  Tested the slides by Rendering them to make sure things worked and looked how I wanted
        - Committed and pushed to my GitHub repository
        - Typed `quarto publish gh-pages dichotomous-key-demo.qmd` in the terminal to publish the slides
