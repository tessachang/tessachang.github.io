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

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_of_building.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard_of_building.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

