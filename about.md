---
layout: page
title: About
permalink: /about/
---

Daphne Moon is a student pursuing a B.S. in Chemistry with a minor in Environmental Studies at Cal Poly SLO. She is originally from Orange County, California and is looking for oppurtunities either in San Luis Obispo or the Orange County Area. She is an avid volunteer at city events and clean-up-the-beach initiatives as well as a tutor for chemistry and biology in the Study Sessions program at Cal Poly. Being active in the community and engaging in learning/new perspectives is one of Daphne's core principles and tries to work toward these goals regularly. Aside from purely academic pursuits, Daphne is involved in the Choral program to have an artistic outlet during every week. Balancing personal passions with academic pursuits is Daphne's main goal and she aims to find a job that can intertwine both her ideals.  

```{r}
# Library
library(streamgraph)
 
# Create data:
data <- data.frame(
  year=rep(seq(1990,2016) , each=10),
  name=rep(letters[1:10] , 27),
  value=sample( seq(0,1,0.0001) , 270)
)
 
# Stream graph with a legend
pp <- streamgraph(data, key="name", value="value", date="year", height="300px", width="1000px") %>%
  sg_legend(show=TRUE, label="names: ")
  

# save the widget
# library(htmlwidgets)
# saveWidget(pp, file=paste0( getwd(), "/HtmlWidget/streamgraphDropdown.html"))
```

#### Contact me

[dmoon06@calpoly.edu](mailto:dmoon06@calpoly.edu)
[daphnemoon33@gmail.com](mailto:daphnemoon33@gmail.com)
