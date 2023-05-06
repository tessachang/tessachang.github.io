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

<br/>

#### Introduction

The Olympic Games is one of the most exciting and highly anticipated sporting events in the world. With over 200 countries participating and more than 40 sports to compete in, it's an event that captures the attention of billions of people worldwide. As a data analyst, I was interested in exploring the rich and extensive dataset of the Olympic Games to answer some key questions. What are the most successful countries in Olympic history? How have each country's medal counts evolved over time, and what is the breakdown by gender? And, which countries dominate in each sport?

<br/>

#### Dataset

This dataset contains a wealth of information on the modern Olympic Games, covering all the Games from Athens 1896 to Rio 2016. The data was scraped from www.sports-reference.com in May 2018, and is available for download at https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results.

<br/>

#### Visualization 1

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_combined.json" style="width: 100%"></vegachart>

<br/>

The two charts that have a joint filter of choosing the country provide a more detailed view of the Olympic medal data. The first plot displays the count of every sport that the chosen country has won medals in, providing an overview of the sports in which that country has been successful in the Olympics. This plot can help us identify the strengths and weaknesses of each country in terms of sports, and it can also give us an idea of the sports that are most popular and competitive in the Olympics.

The second plot shows the change of medal over time for the selected country, and the bars are separated by sex using color. This plot helps us understand the trends in the number of medals won by the chosen country over the years, as well as the gender distribution of the medals. By looking at the color of the bars, we can easily see the breakdown of medals by gender, which can help us understand the level of representation of men and women in the Olympics.

Both charts have a joint filter, which means that when we select a country in one chart, the other chart will update to show the data for that country only. This feature enables us to easily compare the count of every sport for that country with the change of medal over time, and to analyze the data in a more focused way.

<br/>

#### Visualization 2

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/medals_won_by_country.json" style="width: 100%"></vegachart>

<br/>

I created a bar chart that shows the number of medals won by each country in the history of the Olympic Games. Each bar in the chart represents a country, and the height of the bar shows the total number of medals won by that country. Additionally, the color of the bar represents the distribution of medals won by that country - gold, silver, and bronze. This allows us to easily see which countries have the most medals, as well as which countries have the highest number of gold medals, which is often considered the most prestigious.

Furthermore, I added a filter to the chart, which allows the user to choose which sport to see the distribution of medals for each country. This feature allows us to see which countries excel in a particular sport, and which sports are dominated by specific countries. For example, we can see that the United States dominates in swimming and athletics, while China excels in badminton.

Overall, this chart provides a comprehensive overview of the Olympic Games' history and allows us to visualize the success of each country in the competition. It also allows us to explore the different sports and see which countries are dominant in each.

<br/>

#### Contextual visualization 1

source: https://www.kaggle.com/code/joshuaswords/does-hosting-the-olympics-improve-performance

![alt text](https://www.kaggleusercontent.com/kf/71354869/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..iDOdbMVEjt22WUXycfMfQA.IC3u9SspY4qw0OOjXVWUzL1ZucD-yxUIDynAv_08l0gv75vQmJwzrfQWUsOPAwZO-4dQ7M7RdT4y8eaEL9ivk8HAQ9ls647zPSd7kc45qXrepBQRajJrvu58cG86gLo74R3BeB5UFVk4xkFNTpZLmb_fFrQgDB0foNlRPfk36VN68Asq5BD6ocRMFDNquSympx78BqYzoWY0mdWA1TsJbZEUyW5qsek7Fa3yKqgh-uChg7bojx2TFUdk5uoc11ECaVTx2i6YZh9RaTiSkgo5K66cK6r7rnTCqGo7P3F_649uLLSab1bu9r0pnc6CH-YnEX6LliRVTlKFDVLl27aUGe6QbI6qBSz0XVdvXgLhETGMC72vg7Y8Z8P2kV4oSLD_R_fz7-1nr9qe3rZ138xEMXYGg3PGw89B-22NWsBhG0uh3pSI3Yl9YNN4cRW9O4NNPTsXMLMXNWV-O-g25X8q9jtAP2fwb3PBtiXfQeKu1dy6l2d53jFTKCt0YKlTr1aoh9jEbDs9AD20cjCIWAJrZBzdCNk6RsVpwSLDmrmBTmXNszJv0KAusoBA640kXF_UEJv3sIfpJyLu-3M4lsCRz5-fpYN9MgCso7t6gQeZ35uzYw5SVPbEhhXQEyXkuuHdNTkUkxQ4b24v29JmAJliA3f8J59lOkLhQ0tmEab4zM9GAadCoty7TBp2UueWcdMvruhnOKF76BdO1BiNw-yiRA.TK_Lfob3JQItUfmnZm5CeQ/__results___files/__results___33_0.png)

The plot shows that when a country hosts an Olympic Games, their average total medal tally tends to increase significantly compared to their performance in previous games. This suggests that the host country often has a home advantage, perhaps due to factors such as familiarity with the venue, support from the local crowd, and reduced travel and logistical stress. Additionally, host countries may invest more resources and prioritize their athletes' training and development in preparation for the Games, leading to a stronger overall performance.

However, it is worth noting that hosting an Olympic Games is a massive undertaking that requires significant financial and infrastructural investment. Therefore, it is not always feasible or desirable for countries to host the Games, especially if the potential benefits are outweighed by the costs and risks involved. Nevertheless, for those countries that do host, this plot provides an interesting insight into the potential benefits of hosting the Olympics beyond simply showcasing their national pride and culture.

<br/>

#### Contextual visualization 2

source: https://www.bloomberg.com/graphics/tokyo-2020-summer-olympics-medal-count/

![alt text](https://www.datasketch.co/uploads/2-bloomberg.png)

The results of all events and medals won by each country or delegation during the Tokyo 2020 Olympic Games were tracked by Bloomberg and presented in a map-like graph. The United States came out on top for gold medals with a count of 39, closely followed by China with 38. The graph offers an event-by-event breakdown of all the winners and how the medals were distributed across different delegations.

<!-- these are written in a combo of html and liquid -->

<br/>

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/tessachang/tessachang.github.io/main/_data/athlete_winner.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tessachang/tessachang.github.io/blob/main/python_notebooks/chang-tessa-project_part3.ipynb" text="The Analysis" %}
</div>
