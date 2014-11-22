# Shiny - Homework
Julia Gustavsen and Jenny Bryan  
2014-11-18  

## Big picture

We made a Shiny app that let us graph the Gapminder data. 

There is a lot you can do with Shiny. For homework we want you to:

* add the Gapminder data as a .tsv file to a directory in your gapminder app ("./data/" would be a good option for a directory). This way we the data are included as part of your app. Load in the data from this directory instead of the url given in class. 
* use another type of widget to control an aspect of the data (see [Shiny Widget Gallery](http://shiny.rstudio.com/gallery/widget-gallery.html))
* edit the dropdown menu for countries so that you can choose 2 (or more) countries
* try facetting the data based on one of your user inputs.
* please have your app organized with the strict directory structure required by Shiny so that your peer reviewer can download your scripts and run you app locally. Please also deploy your app to the shinyapps.io website or if you are really excited talk to Jenny about deploying to the shinyapps.stat.ubc.ca server.  

### Due date

Your Shiny app is due Friday 28 November 2014.

## Please just tell me what to do

Follow the tutorial up until the end. 
* Replace the slider for the years instead with the widget `dateRangeInput`. Pay careful attention to the "format" and "startview" arguments. 
* Edit the `selectInput` for countries by adding in values for the arguments "selected" and "multiple".  
* Either add facetting to your plot by country or add the use of colour to you plot to distinguish the 2 or more countries displayed. See [ggplot2 tutorial](cm005_still-data-ggplot2-rmarkdown.html)
* Commit the app to your Stat545/547 repo, push to Github.  Also deploy the app to shinyapps.io using the "Publish" button in Rstudio (or see [tutorial section on deployment](shiny02_activity.html#deployment))

## I want to aim higher! Shiny

* Use another approved data set to create an app that outputs a plot, a table and has 2 control widgets that change the output of the plot (i.e. meets all the requirements above, but using a different data set). 
* Add a widget to enable you to turn the facetting of the graphs "on" or "off" (either using your Gapminder app or another dataset.)
* Add images to your app.[R studio Shiny tutorial-see header "Images"](http://shiny.rstudio.com/tutorial/lesson2/)
* Deploy on shinyapps.stat.ubc.ca

## I want to aim way higher!  

* CSS or Html junkie? Try using another css theme or create and use your own css theme. `shinyUI(fluidPage(theme = "bootstrap.css"` [R studio Shiny Article on css style](http://shiny.rstudio.com/articles/css.html)
* Explore a new layout (e.g. `gridLayout()`, `fluidRow()`) and have different graphs laid out on different pages.
* Deploy your cool app and tweet to @STAT545 about it. We guarantee people will be stoked about what you created. 


## Rubric

Your peer reviewer will try run your app! 

Check minus: There is a problem with some aspect of `server.R` or `ui.R`. When the directory for the Gapminder app is downloaded locally (we won't be able to use the `runGitHub()` since these are private repositories) the peer reviewer cannot get the Shiny app to run. 

Check: App runs! All the required widgets, interactivity and facetting/colour are included. Good work!

Check plus: Exceeded the requirements in number of dimensions. App is deployed on shinyapps.io or on shinyapps.stat.ubc.ca. You have added a pleasant, useful dimension (widget, images, layout, css/html coding) to the app that was not required. Neat! 

Recall the [general homework rubric](http://stat545-ubc.github.io/peer-review01_marking-rubric.html).

## Authors

Written by [Julia Gustavsen][] and [Jenny Bryan][].

[Julia Gustavsen]: http://twitter.com/JuliaGustavsen
[Jenny Bryan]: http://www.stat.ubc.ca/~jenny/