---
layout: page
title: Sales Data Analytics and forecasting
description: Dashboards for evaluating sale's data and predicting seasonal sale's for different products.
img: assets/img/ecommerce_dashboard.png
importance: 1
category: work
---

This project was developed by getting sales and ecommerce data from the U.S. and Brazil.

## Dashboard

PowerBI was used to develop a dynamic dashboard to analyze all payments made within the timeline present in the database. The dashboard gives an overall view of the regions and type of products that are mostly sold.

It's possible to filter by date and product, changing the other charts as well to check how those payments were made (number of installments and payment type) and in which regions. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ecommerce_dashboard.png" title="dashboard example" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The developed PowerBI dashboard contains value information to surf the historical ecommerce data.
</div>

It's important to note that this type of dashboard is dynamic and interactive, allowing the user to actually see the results of any filter or selection into the other charts.
<br>

## Forecasting

It's also possible to do some forecasting with the available data. For demonstration purposed, a more complete historical dataset, containing U.S. Sales from 1970 to 2018 was used to predict sales for 2019. 

Below we can see some analysis done before applying the ARIMA (Autoregressive integrated moving average) model.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/forecast_1.png" title="timeseries decomposition" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/forecast_2.png" title="1st order diff" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/forecast_3.png" title="2nd order diff" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, a series decomposition of the whole timeseries. On the middle, the 1st order differentiation with it's respective autocorrelation. On the right, the 2nd order differentiation and autocorrelation.
</div>

After training and evaluating different ARIMA models, the RMSE (Root Mean Square Error) was reduced from the first training method by more than 5000, obtaining a more satisfying result. A cross-validation for another years or with a time delay could be used for even better results and validation.

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/true_pred_1.png" title="true values vs predicted" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/true_pred_2.png" title="true values for predicted" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    On the left, the first model results for prediction values for 2019. On the right, the results for best model obtained.
</div>

The same type of forecast can be done by using different categories, or by filtering by product or department. Dashboards can also be made to evaluate different models, allowing a huge range of possible combinations to achieve good results and improve decision making with machine learning algorithms.