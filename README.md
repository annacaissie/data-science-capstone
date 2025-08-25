# Off the Rails: Examining Reliability and Ridership on the MBTA

#### Jake Jauregui & Anna Caissie

## Brief background

Many Boston-area commuters and residents start and end their days riding with the MBTA. Slow zones, delays, and reliability issues affect the day-to-day life of riders. We aim to explore how these issues have evolved post-COVID and their association with ridership. 

## Question

What factors best predict MBTA ridership, and how strongly do service disruptions like slow zones and alerts contribute compared to other predictors? 

## Hypothesis & Predictions

### Hypothesis

Service disruptions like delays and track speed restrictions line up with significantly reduced reliability scores and ridership.

### Predictions

We expect that disruptions will emerge as significant predictors of ridership, even when accounting for other temporal and operational factors.

### Data source

Data is sourced from the MBTA Blue Book Open Data Portal, found here: https://mbta-massdot.opendata.arcgis.com

Datasets included are:
1. [MBTA Gated Station Entries](https://mbta-massdot.opendata.arcgis.com/datasets/001c177f07594e7c99f193dde32284c9_0/explore)
2. MBTA Service Alerts ([1](https://mbta-massdot.opendata.arcgis.com/datasets/90ed9092bd7a4285b296d5ff938edf29_0/explore), [2](https://mbta-massdot.opendata.arcgis.com/datasets/f960d5089e164fb8b6c6936c70719d72/about), and [3](https://mbta-massdot.opendata.arcgis.com/datasets/ef115f7cf6684360b040b6d1d033eff0/about))
3. [MBTA Rapid Transit Speed Restrictions by Day](https://mbta-massdot.opendata.arcgis.com/datasets/d73ed67e4cc84a84b818ea2c5caef696/about)
4. [MBTA Bus, Commuter Rail, & Rapid Transit Reliability](https://mbta-massdot.opendata.arcgis.com/datasets/b3a24561c2104422a78b593e92b566d5_0/explore)

#### Thank you for riding the T!

# Guide

## What you need
Python 3.10
Jupyter Notebook

Please have installed:
sklearn
seaborn
matplotlib
pandas
numpy
scipy
statsmodels

It will be helpful to have at least 8GB RAM.

## Running code
All code is contained in Jupyter Notebook files in the jupyter_notebook_files directory.
Clone the repository and start Jupyter Notebook.
Files do not need to be run in any particular order since inputs are stored in this repository. 

However, we recommend the following order:

1. exploratory_data_analysis.ipynb
This file contains the reading in and aggregation/merging of raw data.
2. preprocessing_feature_engineering.ipynb
This file contains feature engineering and pre-processing steps.
3. linear_regression.ipynb
This is a simple linear regression model to serve as a baseline. 
4. lasso_regression.ipynb
This is a lasso regression model where we tune for the best alpha. It should run relatively quickly.
5. random_forest.ipynb
Please allow several minutes for the fit() function to run. We are tuning several parameters, and this can be somewhat resource-intensive.
