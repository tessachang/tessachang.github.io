---
name: Exploring Medal Winning Trends in the Olympic Games
tools: [Python, HTML, vega-lite, altair]
image: assets/pngs/medals.png
description: Final Project for IS445 Data Visualization
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Exploring Medal Winning Trends in the Olympic Games Python+altair+vegalite

#### Group 10:

Tessa Chang (chingc4@illinois.edu)

#### Visualization 1

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 40%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 40%"></vegachart>

The histogram plot displays the distribution of the year constructed variable, using an ordinal encoding scheme and the count of records represented by each bar. To avoid overcrowding the plot, I have chosen to filter the years and only visualize the most recent 50 years. This allows the user to focus on the more recent data and gain a better understanding of the distribution over time.

The heatmap plot displays two categorical variables, Bldg Status and County, using an ordinal encoding scheme. The color gradient is based on the count of records, with more counts represented by intense colors and fewer counts represented by lighter colors.

To enhance interactivity, the histogram and heatmap plots are connected. By selecting a window in the histogram, the user can filter the count of records within a specific year constructed. The heatmap plot will also filter by building status and county based on the selected year.within the year constructed and also on the building status by county the plot will also filter whose years.

#### Visualization 2

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>

The histogram plot displays the distribution of the year constructed variable, using an ordinal encoding scheme and the count of records represented by each bar. To avoid overcrowding the plot, I have chosen to filter the years and only visualize the most recent 50 years. This allows the user to focus on the more recent data and gain a better understanding of the distribution over time.

The heatmap plot displays two categorical variables, Bldg Status and County, using an ordinal encoding scheme. The color gradient is based on the count of records, with more counts represented by intense colors and fewer counts represented by lighter colors.

To enhance interactivity, the histogram and heatmap plots are connected. By selecting a window in the histogram, the user can filter the count of records within a specific year constructed. The heatmap plot will also filter by building status and county based on the selected year.within the year constructed and also on the building status by county the plot will also filter whose years.

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/tessachang/tessachang.github.io/main/_data/athlete_winner.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tessachang/tessachang.github.io/blob/main/python_notebooks/chang-tessa-patki-rhuta-homework10.ipynb" text="The Analysis" %}
</div>
