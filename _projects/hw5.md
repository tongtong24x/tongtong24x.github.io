---
name: Bigfoot Sightings Project
tools: Python, Altair, Vega-lite
image: assets/pngs/chart1.png
description: A visualization project using Altair and Vega-Lite to explore Bigfoot sightings data.
custom_js: none
---

## HW5

### Visualization 1: Bigfoot Reports by State

<img src="{{ '/assets/pngs/chart1.png' | relative_url }}" width="100%">

This bar chart displays the number of Bigfoot sightings reported in each U.S. state. The x-axis represents the state names, while the y-axis shows the count of reports. I used a bar chart because it’s effective for comparing categorical variables. The chart uses nominal encoding for the `state` variable on the x-axis and quantitative encoding for the count on the y-axis. I applied color encoding based on state names to give each bar a distinct color, making the chart visually engaging and helping distinguish states quickly.

The data transformation was minimal — I grouped the raw dataset by the `state` column and counted the number of records per state. I sorted the bars in descending order by count so viewers can easily see which states have the most reports. Washington, California, and Florida had the highest counts, suggesting possible regional trends or cultural reporting differences.

---

### Visualization 2: Monthly Bigfoot Report Frequency

<img src="{{ '/assets/pngs/chart2.png' | relative_url }}" width="100%">

This line chart shows the frequency of Bigfoot sightings by month. The x-axis represents the month of the year (1 to 12), and the y-axis shows the count of sightings. I chose a line chart with dots to emphasize the trend across months while still showing the individual data points. The color scheme is uniform since the focus is on time trends rather than category distinction.

For data transformation, I extracted the month from the `date` column using `pd.to_datetime()` and `.dt.month`. I then aggregated the counts by month. The interactive feature I added was tooltip functionality using Altair's `tooltip` encoding. This allows viewers to hover over any point to view the exact number of reports for that month, making it easier to analyze specific data points in context. This interactivity adds clarity and makes the data more engaging.

---

## The Data & The Analysis

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/hw5:2.ipynb" text="The Analysis" %}
</div>
