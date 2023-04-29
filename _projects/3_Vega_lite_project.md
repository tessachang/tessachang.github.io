---
name: HW10 Vega Lite plots, multiple ways
tools: [Python, HTML, vega-lite, altair]
image: assets/pngs/building.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# HW10 Python+altair+vegalite

#### Group 7:

Rhuta Patki (rhutap2@illinois.edu)
Tessa Chang (chingc4@illinois.edu)

#### Visualization 1

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_of_building.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_of_building.json" style="width: 100%"></vegachart>

The histogram plot displays the distribution of the year constructed variable, using an ordinal encoding scheme and the count of records represented by each bar. To avoid overcrowding the plot, I have chosen to filter the years and only visualize the most recent 50 years. This allows the user to focus on the more recent data and gain a better understanding of the distribution over time.

The heatmap plot displays two categorical variables, Bldg Status and County, using an ordinal encoding scheme. The color gradient is based on the count of records, with more counts represented by intense colors and fewer counts represented by lighter colors.

To enhance interactivity, the histogram and heatmap plots are connected. By selecting a window in the histogram, the user can filter the count of records within a specific year constructed. The heatmap plot will also filter by building status and county based on the selected year.within the year constructed and also on the building status by county the plot will also filter whose years.

#### Visualization 2

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard.json" style="width: 100%"></vegachart>

Dashboard 2:<br>
The second dashboard focuses on conveying insights regarding the total number of buildings abandoned, in use, and in progress and their resulting total square footage under a given agency. This dashboard is interactive and selecting a bar in the first upload updated the second plot to show data for the selected agency only.<br>
<br>
Data Preprocessing: <br>
The data used in this dashboard was preprocessed by dropping any rows with the "Year Acquired" or "Year Constructed" equal to 0 since it does not make sense for a building to exist but not have these years associated with it.<br>
<br>
Plot1:<br>
This plot presents the total square footage of the area associated with the various agencies. The total square footage has been calculated as the sum of the square footage of individual buildings under a given Agency. For this visualization, we used the bar chart since it was more intuitive for our use case. The x-axis and y-axis represent the Agency Names and the Square Footage respectively, and these variables have been encoded as ‘Nominal’ and ‘Quantitative’ data types respectively. The color of the bar is governed by a condition. A bar in this plot can be selected by clicking on it. On doing this, the rest of the bars in the plot turn grey to highlight the Agency of interest in blue. Other than the data cleaning, no other transformations we implemented on this data prior to creating this visualization. The sum of the individual square footage was calculated using the function ‘sum()’ within the Altair chart construct. This chart was previously implemented in homework #9 using vegalite in Starboard. <br>
<br>
Plot2:<br>
The second plot in our second dashboard presents the number of buildings that are currently abandoned, in progress or in use. We used the bar chart to represent our insights. The x-axis and y-axis represent the Building Status and the Building count respectively, and these variables have been encoded as ‘Nominal’ and ‘Quantitative’ data types respectively. To match the theme of the previous plot, we used the same blue color for this one. Other than the data cleaning, no other transformations we implemented on this data prior to creating this visualization. The building count was calculated using the function ‘count()’ within Altair’s chart construct. This chart was not implemented as a part of homework #9.

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tessachang/tessachang.github.io/blob/main/python_notebooks/chang-tessa-patki-rhuta-homework10.ipynb" text="The Analysis" %}
</div>
