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

# Exploring Medal Winning Trends in the Olympic Games

## Python+altair+vegalite

#### Group 10:

Tessa Chang (chingc4@illinois.edu)

#### Introduction

The Olympic Games is one of the most exciting and highly anticipated sporting events in the world. With over 200 countries participating and more than 40 sports to compete in, it's an event that captures the attention of billions of people worldwide. As a data analyst, I was interested in exploring the rich and extensive dataset of the Olympic Games to answer some key questions. What are the most successful countries in Olympic history? How have each country's medal counts evolved over time, and what is the breakdown by gender? And, which countries dominate in each sport?

#### Visualization 1

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 40%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 40%"></vegachart>

The two charts that have a joint filter of choosing the country provide a more detailed view of the Olympic medal data. The first plot displays the count of every sport that the chosen country has won medals in, providing an overview of the sports in which that country has been successful in the Olympics. This plot can help us identify the strengths and weaknesses of each country in terms of sports, and it can also give us an idea of the sports that are most popular and competitive in the Olympics.

The second plot shows the change of medal over time for the selected country, and the bars are separated by sex using color. This plot helps us understand the trends in the number of medals won by the chosen country over the years, as well as the gender distribution of the medals. By looking at the color of the bars, we can easily see the breakdown of medals by gender, which can help us understand the level of representation of men and women in the Olympics.

Both charts have a joint filter, which means that when we select a country in one chart, the other chart will update to show the data for that country only. This feature enables us to easily compare the count of every sport for that country with the change of medal over time, and to analyze the data in a more focused way.

#### Visualization 2

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>

I created a bar chart that shows the number of medals won by each country in the history of the Olympic Games. Each bar in the chart represents a country, and the height of the bar shows the total number of medals won by that country. Additionally, the color of the bar represents the distribution of medals won by that country - gold, silver, and bronze. This allows us to easily see which countries have the most medals, as well as which countries have the highest number of gold medals, which is often considered the most prestigious.

Furthermore, I added a filter to the chart, which allows the user to choose which sport to see the distribution of medals for each country. This feature allows us to see which countries excel in a particular sport, and which sports are dominated by specific countries. For example, we can see that the United States dominates in swimming and athletics, while China excels in badminton.

Overall, this chart provides a comprehensive overview of the Olympic Games' history and allows us to visualize the success of each country in the competition. It also allows us to explore the different sports and see which countries are dominant in each.

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/tessachang/tessachang.github.io/main/_data/athlete_winner.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tessachang/tessachang.github.io/blob/main/python_notebooks/chang-tessa-patki-rhuta-homework10.ipynb" text="The Analysis" %}
</div>
