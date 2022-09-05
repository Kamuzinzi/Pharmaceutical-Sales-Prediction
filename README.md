# Pharmaceutical-Sales-Prediction

Rossmann Store Sales

Forecast sales using store, promotion, and competitor data

# Overview

# Business Need

You work at Rossmann Pharmaceuticals as a Machine Learning Engineer. The finance team wants to forecast sales in all their stores across several cities six weeks ahead of time. Managers in individual stores rely on their years of experience as well as their personal judgment to forecast sales.

The data team identified factors such as promotions, competition, school and state holidays, seasonality, and locality as necessary for predicting the sales across the various stores.

Your job is to build and serve an end-to-end product that delivers this prediction to analysts in the finance team.

# Data and Features

The data for this challenge can be found [here](https://drive.google.com/file/d/1sGLyrytv6xYBrCPdjZkE1ZDSwngDij4W/view?usp=sharing) . Or you can find it also [here](https://www.kaggle.com/competitions/rossmann-store-sales/data): Rossmann Store Sales | Kaggle

## Data fields

-   Most of the fields are self-explanatory. The following are descriptions for those that aren't.
-   Id - an Id that represents a (Store, Date) duple within the test set
-   Store - a unique Id for each store
-   Sales - the turnover for any given day (this is what you are predicting)
-   Customers - the number of customers on a given day
-   Open - an indicator for whether the store was open: 0 = closed, 1 = open
-   StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
-   SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools
-   StoreType - differentiates between 4 different store models: a, b, c, d
-   Assortment - describes an assortment level: a = basic, b = extra, c = extended. Read more about assortment here
-   CompetitionDistance - distance in meters to the nearest competitor store
