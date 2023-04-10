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

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tessachang/tessachang.github.io/blob/main/python_notebooks/chang-tessa-homework10.ipynb" text="The Analysis" %}
</div>
