---
layout: page
name: Bigfoot Sightings HW5
tools: [Python, Altair, Vega-lite]
image: assets/pngs/chart1.png
description: A project that explores Bigfoot sightings using interactive vega-lite visualizations.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
permalink: /projects/hw5/index.html
---

## HW5 - Interactive Visualizations with Vega-Lite

## Visualization 1: Bigfoot Reports by State

<iframe src="/assets/chart1.html" width="100%" height="600" style="border:none;"></iframe>

This bar chart displays the number of Bigfoot sightings reported in each U.S. state. The x-axis represents state names, while the y-axis shows the count of reports. I used a bar chart to clearly compare different states, with nominal encoding for state and quantitative encoding for count. Each state is represented by a different color to visually distinguish between them.  
Data was grouped by state using pandas, and the counts were sorted in descending order to highlight the states with the most reports (e.g., Washington, California). No other major transformations were needed for this chart.

---

## Visualization 2: Monthly Trends in Bigfoot Sightings

<iframe src="/assets/chart2.html" width="100%" height="600" style="border:none;"></iframe>


This line chart visualizes the number of Bigfoot sightings by month across all years in the dataset. I extracted the month component from the `date` column using `pd.to_datetime(df['date']).dt.month` and then grouped the data by month. The result is a clear trend that shows sighting peaks during summer months.  
The chart includes interactivity in the form of tooltips that appear when hovering over each point. This helps the viewer get exact values for each month, making the chart more informative and user-friendly.

---

## The Data & The Analysis

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

