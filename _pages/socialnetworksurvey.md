---
title: "Social Network Survey page"
permalink: /socialnetworksurvey/
layout: splash
---
# Social Network Survey 

The **Social Network Survey** is a method I developed to get information about a child's social network. Through parent interview, parents will describe their child's "typical week". The parent interview detrimines the boundaries of the network - which people should be included. The Social Network Survey then collects demographic information to assess various aspects of children's network;the Linguistic Diversity, Racial Diversity, Age Diversity, Proportion of Kin relationshps, and how relationships cluster together. These metrics can be used to characterize children's early social experience. 

If you are interested in using the Social Network Survey, please feel free to contact me at [nicoleburke@uchicago.edu](mailto:nicoleburke@uchicago.edu). Below is a description of the R package I created to extract the Social Network Survey from the Qualtrics survey.  

## SocialNetworkSurvey - R package. 

SocialNetworkSurvey is a R package I developed available on my [Github](https://github.com/nicoleburke/Social-Network-Survey). This package contains the functions neccessary to extract the Social Network data from the Qualtrics output. 

## How to install 
devtools::install_github("nicoleburke/Social-Network-Survey")

library(SocialNetworkSurvey)

## How to use package to extract data 

I wrote these functions to take the raw Qualtrics output as it is. The idea is that a person can hit "Export" on Qualtrics, run the .csv file through these functions, and end up with the dataframe they need. With this in mind, before we can extract the Social Network Data, we need to clean the Qualtrics output and prepare a dataframe that has each relationship or "node" on a separate line. Follow the steps below to get the Social Network Data! 

### Step 1: Clean Qualtrics output and create a dataframe with each node per line. 

- Export the data as a .csv file. Make sure the SubjectIDs are *numeric* values. I highly recommend using numbers as opposed to calling your subjects something like "Subject01". 
    
- Import the .csv file into R. Run the .csv file in the *clean_qualtrics* function. This will do 3 things; change NAs into 9999, rename the SubjectID column, and re-order the SubjectID column. This is neccessary in order to run the other functions. 

Testing a theory
```
help("functionname")

```





