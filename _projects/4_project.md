---
layout: page
title: OSRS Data Tracker
description: Project was developed for storing player data from the Old School Runescape API into a PostgreSQL Database. The data can be used to check the player's progression over time.
img: assets/img/osrs_tableau.png
importance: 3
category: fun
---

#### Data Extraction
Each player Hiscores Data is obtained hourly from the available OSRS API: 
E.g. <a href="https://secure.runescape.com/m=hiscore_oldschool/index_lite.ws?player=zezima">https://secure.runescape.com/m=hiscore_oldschool/index_lite.ws?player=zezima</a>

Data is paired with the respective names for each skill and boss kill count.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/osrs_data.png" title="data output" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Structured data obtained from the API after transformation..
</div>

#### Database Insertion and Validation

Data is validated from each user's last record in the database to check data format and if insertion is necessary.

#### Retrieving Data and Visualization

Each player's data can be retrieved directly from the PostgreSQL database and sent to Tableau or any other visualization tool for creating charts to follow character development and other insights.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/osrs_tableau.png" title="tableau" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Dashboard example for evaluating player's data.
</div>

