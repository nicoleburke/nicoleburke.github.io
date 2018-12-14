---
title: "aoianalysis package page"
permalink: /aoianalysis/
layout: splash
---
# aoianalysis  

aoianalysis is a R package I developed available on my github (https://github.com/nicoleburke/aoianalysis). This package contains a few simple functions to make dealing with raw eyetracking data a little easier. 

## Important disclaimer

1. These functions were written to deal with raw eyetracking data output from Tobii. These functions were written to be as flexible as possible, but they work best for data structured like the raw output from Tobii. 
2. Given the first point, this package is still a work in progress! Please read carefully below about how your data should be set-up to use each of these functions. You should also feel free to contact me (nicoleburke@uchicago.edu) if you have any questions or run into any problems. 


## How to install 
devtools::install_github("nicoleburke/aoianalysis")

library(aoianalysis)

## Data set-up

Although Tobii has some other lovely features, the most frustrating (to me personally) is that every time you draw a new AOI, it creates a new column in the raw data that contains -1, 0, or 1 to indicate if there was a hit to that AOI (1), no hit to the AOI (0), or if the AOI was not activated (-1). While this sounds clean and simple to have each AOI have a different AOI, it creats A LOT of columns to sort through in the raw data. For example, within one list let's say you have 8 trials and 2 AOIs per trial. For that list alone, that creates 16 columns that have different names to sort through and that's just one list! Godforbid you are counterbalancing across different lists, this creates a MANY columns to go through.

With this in mind, these functions are set-up such that they work for each **unique trial**. This means, you should have a separate dataframe for each trial type you want to analysis with all subjects in each dataframe. Check out this datasheet and the tabs to see what I am talking [about] ("https://github.com/nicoleburke/aoianalysis/blob/master/sampledatastructure.csv"). You would run these functions twice - once for Trial1 and then again for Trial2. 

Why are they set-up this way? Part of this is to compensate for mistakes in how I set-up my initial eyetracking experiments. In Tobii, it matters what the actual stimuli are called - not just what you call the elements in the timeline of Tobii Studio. Because of this, if you use the same exact simuli on different trials, those trials are indistingustable if you just look at the "MediaName" column. I am working on functions that will take into account these different trials so that eventually, you will just need one large dataframe and can process everything in that one dataframe. Until that point, make sure you have a separate dataframe for each trial type. 

## The functions! 

The descriptions are the same as in the documentation in the package. Use help("functionname") to pull up the description in Rstudio. 

### firstlook 

### firstlook_gp

### switchestotal

### getridofNA

### getridofNA_gp 





