# Tongtong Gu 
##IS 445

Body of sub

###lat thing
add in a link:[This is alink to IS 445](https://uiuc-ischool-dataviz.github.io/is445_obuobg_spring2025/)



---
name: Bigfoot Sightings Project
tools: Python, Altair, Vega-lite
description: An interactive visualization project exploring Bigfoot reports using Altair and Vega-lite
custom_js: vega.min, vega-lite.min, vega-embed.min, justcharts
---


### HW5
## Visualization 1: Bigfoot Classifications by Location

<div id="vis1"></div>
<div id="vis2"></div>

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

<script>
  vegaEmbed('#vis1', '{{ "/assets/json/chart1.json" | relative_url }}');
  vegaEmbed('#vis2', '{{ "/assets/json/chart2.json" | relative_url }}');
</script>

## Visualization 2: Monthly Trends in Bigfoot Sightings


---

## The Data & Analysis

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/hw5:2.ipynb" text="The Analysis" %}
</div>
