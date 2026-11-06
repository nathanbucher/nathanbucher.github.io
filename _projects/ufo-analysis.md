---
layout: project
title: "UFO Sightings Analysis"
---

# UFO Sightings Analysis

## Data and Analysis

### The Data

[The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv)

### The Analysis

[The Analysis](https://github.com/nathanbucher/nathanbucher.github.io/blob/main/Workbook.ipynb)

## Visualization 1: UFO Sightings by State and Shape

<iframe src="/ufo_shape_state.html"
        width="100%"
        height="700"
        frameborder="0">
</iframe>

This visualization shows the number of UFO sightings reported in each state for a selected UFO shape. The x-axis encodes the number of sightings as a quantitative variable while the y-axis encodes state as a nominal variable. A horizontal bar chart was selected because it makes comparisons across states easy to interpret. Color is also used to encode the count of sightings using a sequential blue color scale, where darker shades indicate larger numbers of sightings. To prepare the data, the original UFO dataset was grouped by state and shape and the total number of sightings was calculated for each combination. This aggregation reduced the size of the dataset while keeping the important information needed for the visualization.

## Visualization 2: UFO Sightings Over Time

<iframe src="/ufo_year_trend.html"
        width="100%"
        height="500"
        frameborder="0">
</iframe>

This visualization displays how UFO sightings have changed over time. The x-axis encodes year as a quantitative variable and the y-axis encodes the total number of sightings as a quantitative variable. A line chart was chosen because it clearly communicates trends and changes across time. During preprocessing, the datetime column was converted into a pandas datetime object and a new year variable was extracted from each observation. The data was then grouped by year and the total number of sightings was calculated. This transformation made it possible to display long-term patterns in UFO reports.

## Interactivity

The first visualization includes a dropdown menu that allows users to filter sightings by UFO shape. Selecting a shape updates the chart and displays only sightings that match that category. This interaction makes the visualization more useful because users can focus on one type of sighting at a time and compare how differentdistributed across states. The filter reduces visual clutter and makes geographic patterns easier to identify.
