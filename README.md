# Exploratory Data Analysis Final Project | Fall 2021


## Description
Data Analysis of Life expectancy with multiple WHO data-sets uisng R.


## Languages/Technologies used:
R, Rmd, R-Studio. 


## Data Collection
* Scraped data from the WHO website to obtain life expectancy data-set along with adjacent factors affecting life expectancy (from other sources).
* Time period for analysis 2000-2018
* Data-sets for other factors included GDP, % GDP growth, population, health-care (% spent on health-care, % of populataion with AIDS, Polio, Hep-A, Hep-B and more)
* Data-set included (almost) all countries in the world.


## Data Cleaning, Missing value imputation, Data Transformation and joining
* Data-sets were joined and transformed into one master file using R.
* Few missing features, which were identified to be crucial for analysis were imputed using R. These features included: Continent, Developing/Developed. 
* Many incorrect and erronous data-points were present, especially for the under-developed nations. These were identified and fixed using R and Excel. 
* There were also a lot of missing values, again more missing values were identified for the under-developed nations. Upon identification these were manually filled in, if found. Otherwise they were filled by using nearest-neighbour analysis by filtering on Continents/Countries. 


## Data Analysis with R
* Extensive data analysis was performed on various factors that could potentially affect life-expectancy. Uni-variate and multi-variate analyses were performed. 
* The data analysis techniques utilized, with target variable as life-expectancy: Multi-variate Linear Regression, Local Polynomial Regression / LOESS (locally estimated scatterplot smoothing). 
* Using these models with weighted and un-weighted variants, the models were trained and observed for data as a whole as well as with seperation-analysis for Continents, 4-year periods and developed-status, as well as economic state.
* The results from regression analysis were then visualized using gg-plot library. 


## Results 
* In general, Life-expectancies grew as years passed. 
* As expected the life expectancy was were higher for developed nations rather than developing nations, higher for nations with larger health-care budgets and/or lesser factors/diseases affecting health. 
* Although the Afcrican continent was observed to be an outlier with all the major factors. Several countries in Africa had higher health-care funds allocated but did not have higher life expectancies. Life-expectanices saw a sharp turn in the recent years. The hypothesis for this was the due to healtcare emergenices and disease outbreaks in these countries, the budgets to counter them was also higher. But due to ever-rising cases of disease-outbreaks, the life expectancies in these countries remained low for a long time. 
* More observed results are present in the final report. 
