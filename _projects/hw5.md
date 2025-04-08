---
name: Bigfoot Sightings Project
tools: Python, Altair, Vega-lite
image: assets/pngs/bigfoot.png
description: An interactive visualization project exploring Bigfoot reports using Altair and Vega-lite
custom_js: vega.min, vega-lite.min, vega-embed.min, justcharts
---

## Visualization 1: Bigfoot Classifications by Location

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>

## Visualization 2: Monthly Trends in Bigfoot Sightings

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart2.json" style="width: 100%"></vegachart>

---

## The Data & Analysis

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
