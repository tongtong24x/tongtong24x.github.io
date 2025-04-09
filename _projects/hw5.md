---
layout: page
name: Bigfoot Sightings HW5
tools: [Python, Altair, Vega-lite]
image: assets/pngs/chart2.png
description: A project that explores Bigfoot sightings using interactive Vega-Lite visualizations.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
permalink: /projects/hw5/index.html
---

# HW5: Interactive Visualizations with Vega-Lite

## 📊 Visualization 1: Bigfoot Sightings by State (with Region Filter)

<iframe src="/assets/chart1.html" width="100%" height="600" style="border:none;"></iframe>

This interactive bar chart displays the number of Bigfoot sightings reported in each U.S. state, grouped by U.S. Census-defined regions: **West, Midwest, South**, and **Northeast**.  

When a region is selected from the dropdown menu, the chart updates dynamically to show only the states within that region and their respective sighting counts.  

- **X-axis:** State names (nominal encoding)  
- **Y-axis:** Number of sightings (quantitative encoding)  
- **Color:** Applied for visual separation, but the legend is disabled to reduce clutter  

To prepare the data, I used a Python dictionary to map each state to its region. Rows with missing or invalid `state` or `region` data were removed, and then grouped by state and region to count sightings.  

> The dropdown filter provides interactivity beyond basic pan/zoom and allows users to explore sightings more effectively by geographic area.

---

## 📈 Visualization 2: Monthly Trends in Bigfoot Sightings

<iframe src="/assets/chart2.html" width="100%" height="600" style="border:none;"></iframe>

This line chart illustrates the number of Bigfoot reports for each month of the year, aggregated across all years in the dataset.  

To create this chart, I extracted the month from the `date` field using `pd.to_datetime()` and `.dt.month`, then grouped the data to count reports per month.

- **X-axis:** Month (1 to 12, ordinal encoding)  
- **Y-axis:** Count of reports (quantitative encoding)  
- **Interactivity:** Tooltips show exact counts when hovering over each point  

> This visualization reveals a seasonal pattern, with sighting peaks occurring in the **summer and early fall** months—suggesting possible environmental or behavioral factors influencing reporting frequency.

---

## 🔗 Data & Analysis

<div class="left">
  {% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="📂 The Data" %}
</div>

<div class="right">
  {% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/Workbook.ipynb" text="📓 The Analysis" %}
</div>

