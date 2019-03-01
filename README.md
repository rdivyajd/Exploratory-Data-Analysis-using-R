# Exploratory-Data-Analysis-using-R
EDA of Historical Storm Data of North America

| Authors: Divya Rajendran, Ethan Violette, Pramod Duvvuri, Wenjuan Sang

## Pre-Requisites/Requirements
The project can be run using RStudio, and we assume the users have access to the application in their computers.
### Required Packages
```{r}
install.packages(knitr)
install.packages(ggplot2)
install.packages(broom)
install.packages(dplyr)
install.packages(ggmap)
install.packages(htmlwidgets)
install.packages(MASS)
install.packages(gridExtra)
devtools::install_github("dkahle/ggmap")
devtools::install_github("hadley/ggplot2")
```

## Goal / Aim

### Are storms in the Tropics of the Americas increasing? 

With hurricanes staying at the forefront of the news over the past couple of years, the idea of an increase in number of  dangerous storms is fairly frightening. We utilized past data of tropical and subtropical storms to answer this question and, also see the trends in storm frequency for each category of storm. 

## Data Set

For our choice of data set, we utilized the Department of Homeland Security’s Storm Tracking data ( available [here] )

## Analysis

We followed the below steps in our EDA

1. Plots of univariate, bivariate, and trivariate relationships between different attributes such as basin, category, location, frequency, over the year attribute. 

2. Univariate and Bivariate relationship plots between pressure and wind for different category of storms.

3. Residual, fitted values comparision for a poisson model

4. plot of predictions for expected frequency of storms

5. heat map of frequency of storms in differnt basins

## Conclusions and Limitations

* It appears that the number of storms is indeed increasing at a small rate (0.08%) as time goes on; this can be predicted with some degree of accuracy with features such as Basin of Origination, Category of Storm, and (of course) Year. 

* Though we had sufficient tools at our disposal to conclude this using a fitted Poisson Model, we’re limited in our predictive accuracy due to lack of additional features. 

* Given more time, we would have merged this dataset with another that contained information about weather, number of man-made influencers of climate change, and other useful predictors, over time.


[here]: https://data.world/dhs/historical-tropical-storm
