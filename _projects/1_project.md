---
layout: page
title: World Bank Open Data
description: This small project was created for obtaining data from the World Bank Open Data API using the wbdata python package.
img: assets/img/wbo_tableau.png
importance: 2
category: work
---

The World Bank Open Data API have many indicators from different countries that can be acquired and manipulation. The example below show some indicators that can be retrieved.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/wbo_indicators.png" title="indicators" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Indicators obtained from the API.
</div>

With the wbdata package it's possible to access those indicators and using pandas and other python libraries it can be manipulated to produce a desired file format.

Below is an example of the possible outputs obtained from the API.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/wbo_output.png" title="output" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Data after transformation.
</div>

Data can be saved in a CSV file or sent to any repository to be used for visualization or research purposes. In the example below, Tableau is used for visualization.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/wbo_tableau.png" title="tableau" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Dashboard example for evaluating data.
</div>

