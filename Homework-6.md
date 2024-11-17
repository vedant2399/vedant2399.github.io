---
layout: default
title: HW6 Visualizations
---

# Homework 6 - Interactive Visualizations with Altair

## Visualization 1: Total Square Footage by Agency

<p>This bar chart shows the total square footage managed by different agencies. It highlights which agencies handle the largest amount of building space, providing an easy comparison of building sizes across different departments.</p>

### Design Choices
<p>The x-axis represents the total square footage, while the y-axis lists the agencies in descending order to emphasize which agencies have the largest footprints. Color is encoded using a `viridis` color scale, with a gradient indicating the magnitude of the square footage. This choice makes it easy to identify agencies with higher square footage visually.</p>

### Data Transformations
<p>The data was grouped by the `Agency Name` column, and the total square footage was summed for each agency to provide an aggregated view of the data. This transformation was done to summarize building sizes managed by each agency.</p>

### Overlap with Homework #5
<p>In Homework #5, a similar analysis was done using a different visualization tool, but this visualization in Altair has been enhanced with sorting and a distinct color scheme for better clarity. Changes were made to the design, sorting order, and color scale compared to Homework #5.</p>

<iframe src="bar_chart.html" width="800" height="600"></iframe>

---

## Visualization 2: Interactive Filtered Scatter Plot

<p>This scatter plot illustrates the relationship between building square footage and the year of acquisition for different agencies. Users can filter the data by selecting an agency from the dropdown menu, allowing for targeted exploration and comparison.</p>

### Design Choices
<p>The x-axis represents the `Year Acquired` as an ordinal value, while the y-axis shows `Square Footage` as a quantitative value. Colors differentiate agencies, making it visually intuitive to identify the selected agency's data. Tooltips are added to show more details, such as `Agency Name`, `Square Footage`, and `Year Acquired` when hovering over a data point.</p>

### Interactivity
<p>A dropdown menu allows the user to select an agency, which dynamically filters the scatter plot data. This interactivity helps users focus on the data for a particular agency, enabling clearer insights and easier comparisons without being overwhelmed by unrelated data points.</p>

### Data Transformations
<p>Data cleaning involved removing missing or invalid values for the `Year Acquired` field. A selection object was created in Altair to link the dropdown filter with the data, enabling smooth interaction.</p>

### Overlap with Homework #5
<p>This visualization differs significantly from Homework #5, which used simpler visualizations without interactivity. Here, interactivity has been added with a dropdown selection, enhancing data exploration.</p>

<iframe src="dropdown_chart.html" width="800" height="500"></iframe>

---

<p>
  <a href="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" target="_blank" class="btn">The Data</a>
  <a href="https://github.com/vedant2399/vedant2399.github.io/blob/main/Homework%206.ipynb" target="_blank" class="btn">The Analysis</a>
</p>
