IS 445

add in a link:[This is a link to IS 445](https://uiuc-ischool-dataviz.github.io/is445_obuobg_spring2025/)




### HW5

## Visualization 1: Bigfoot Classifications by Location

<div id="vis1"></div>

## Visualization 2: Monthly Trends in Bigfoot Sightings

<div id="vis2"></div>

<!-- Vega + Vega-Lite + Vega-Embed CDN -->
<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

<!-- Embed the charts -->
<script>
  vegaEmbed('#vis1', '{{ "/assets/json/chart1.json" | relative_url }}');
  vegaEmbed('#vis2', '{{ "/assets/json/chart2.json" | relative_url }}');
</script>

---

## The Data & Coding

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/tongtong24x/tongtong24x.github.io/blob/main/python_notebooks/hw5_2.ipynb" text="The Coding" %}
</div>
