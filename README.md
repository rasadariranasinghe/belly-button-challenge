# Belly Button Biodiversity Dashboard

## Overview

This project is an interactive dashboard that allows users to explore the Belly Button Biodiversity dataset, which catalogs the microbes that inhabit human navels. The dashboard visualizes data on microbial species, known as operational taxonomic units (OTUs), and provides insights into their prevalence across different individuals.

## Features

- **Dropdown Menu**: Select an individual to view their specific microbial data.
- **Horizontal Bar Chart**: Displays the top 10 OTUs found in the selected individual, using:
  - `sample_values` as values for the bar chart.
  - `otu_ids` as labels for the chart.
  - `otu_labels` as hover text for additional information.
  
- **Bubble Chart**: Displays each sample's data using:
  - `otu_ids` for the x values.
  - `sample_values` for the y values.
  - `sample_values` for the marker size.
  - `otu_ids` for marker colors.
  - `otu_labels` for text values on hover.

- **Metadata Display**: Shows the individual's demographic information by looping through each key-value pair from the metadata JSON object and appending it to the `#sample-metadata` panel.

## Coding Overview

In this project, I utilized JavaScript along with the D3.js library to manipulate the DOM and handle data visualization tasks. Key coding aspects include:

- **Data Loading**: Used D3 to load the `samples.json` dataset from a remote URL, which contains the necessary data for the dashboard.
  
- **Dynamic Charts**: Implemented functions to build a horizontal bar chart and a bubble chart based on user selections from a dropdown menu. The charts update dynamically to reflect the selected individual's data.

- **Metadata Panel**: Created a metadata panel that displays an individual's demographic information by extracting and formatting the relevant data from the dataset.

- **User Interaction**: Designed an interactive experience where the dashboard updates all visualizations when a new individual is selected from the dropdown menu.

## Technologies Used

- HTML
- CSS
- JavaScript
- D3.js
- Plotly.js

## Usage

1. Select an individual from the dropdown menu.
2. View the horizontal bar chart to see the top 10 OTUs for the selected individual.
3. Analyze the bubble chart to explore the relationship between OTUs and sample values.
4. Read the individual's demographic information displayed in the metadata panel.


