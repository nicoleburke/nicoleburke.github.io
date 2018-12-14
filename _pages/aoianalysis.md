---
title: "aoianalysis package page"
permalink: /aoianalysis/
layout: single
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

Although Tobii has some other lovely features, the most frustrating (to me personally) is that every time you draw a new AOI, it creates a new column in the raw data that contains -1, 0, or 1 to indicate if there was a hit to that AOI (1), no hit to the AOI (0), or if the AOI was not activated (-1). While this sounds clean and simple to have each AOI have a different column, it creats A LOT of columns to sort through in the raw data. For example, within one list let's say you have 8 trials and 2 AOIs per trial. For that list alone, that creates 16 columns that have different names to sort through and that's just one list! Godforbid you are counterbalancing across different lists, this creates a MANY columns to go through.

With this in mind, these functions are set-up such that they work for each **unique trial**. This means, you should have a separate dataframe for each trial type you want to analysis with all subjects in each dataframe. Check out this datasheet and the tabs to see what I am talking about (https://github.com/nicoleburke/aoianalysis/blob/master/sampledatastructure.xlsx). You would run these functions twice - once for Trial1 and then again for Trial2. 

Why are they set-up this way? Part of this is to compensate for mistakes in how I set-up my initial eyetracking experiments. In Tobii, it matters what the actual stimuli are called - not just what you call the elements in the timeline of Tobii Studio. Because of this, if you use the same exact simuli on different trials, those trials are indistingustable if you just look at the "MediaName" column. I am working on functions that will take into account these different trials so that eventually, you will just need one large dataframe and can process everything in that one dataframe. Until that point, make sure you have a separate dataframe for each trial type. 

Other important note: make sure your SubjectID column is read in as a **factor** not a numeric or integer. The functions need SubjecID to be a factor to work properly. Use as.factor() to change that column. 

If you are an expert in any coding language, you might not find this package particularly helpful. I wrote this for the person that I was when I came to eyetracking - minimal coding experience and minimal understanding of what the structure of eyetracking data looks like. My hope is that these functions will help save people time and aggravation! 

## The functions! 

The descriptions are the same as in the documentation in the package. Use help("functionname") to pull up the description in Rstudio. 

### firstlook 

This function specifies which AOI participants look to first for a given trial. This function only deals with 2 AOIs - typically used in infant/child studies where you want to know which AOI - the left or right AOI - did infants/children first look? This data should deal with raw eyetracking data.

### firstlook_gp

This function specifies which AOI participants look to first for a given trial AFTER they have looked to the hand AOI. This function should be used for the goal prediction paradgim.

Here, I specify "handAOI" as the neccessary AOI to look at, but that could be whatever AOI you want if you are using a different paradigm. 

### switchestotal

Given two AOIs, how many contingent switches were made by the participant? It gives the total number of switches as well as the break down of when it was aoi1 to aoi2 AND aoi2 to aoi1.

### getridofNA

This function is neccessary for 'firstlook' and 'switchestotal' functions to run properly. This gets rid of NA values in the desired AOI colunms so that the firstlook function runs smoothly. This function requires the package 'tidyverse'. 'firstlook' and 'switchestotal' do not like NAs for the boolean evaluations (see the source script). 

### getridofNA_gp 

This function is neccessary for 'firstlook_gp' function to run properly. For the same reason as 'getridofNA', this function is specifically for the 'firstlook_gp' function. 





