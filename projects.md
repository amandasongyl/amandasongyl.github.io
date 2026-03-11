---
layout: page
title: Projects
permalink: /projects/
---

## Project All Access Livable Housing
*[Placeholder for link to public GitHub repository]*
This project examines the relationship between unsheltered homelessness and housing prices in San Francisco between 2020 and 2024 at the census tract level. Our objective was to integrate multiple public datasets (including housing price indicators, homelessness-related counts and reports, and census demographic data) in order to better understand spatial and temporal patterns in unsheltered homelessness across the city. We also aimed to develop interactive visualizations that allow users to explore how key indicators change across neighborhoods and over time. 

### Key Contributions
- **Data ingestion and preprocessing**: I developed Python scripts to clean and filter relevant datasets from the U.S. Census and American Community Survey (ACS). These scripts consolidated key metrics into standardized CSV files and generated tract-level shapefiles that could be used for spatial analysis. I also developed an automated web-scraping tool to download publicly available shelter waitlist datasets, although this pipeline was later archived due to limitations in upstream data availability.
- **Geospatial data integration**: To combine multiple spatial datasets, I wrote scripts to match point-based geographic data to census tracts. This involved implementing spatial indexing techniques such as quadtrees to improve the efficiency of spatial joins when processing large volumes of data.
- **Data aggregation and transformation**: I aggregated encampment reports and 311 service call data at the monthly and census tract levels, creating a structured dataset that allowed for temporal and geographic comparisons across neighborhoods.
- **Interactive data visualization**: I developed an interactive choropleth map using Altair that allows users to explore multiple metrics and observe how they change across census tracts and over different time periods. The visualization was designed to make complex spatial data more accessible and interpretable for users interested in housing and homelessness trends.
- **Command-line interface development**: I built a command-line interface (CLI) to streamline execution of the data processing and analysis pipeline, enabling users to run workflows and manage inputs directly from the terminal.
- **Data validation and pipeline reliability**: To ensure the robustness of the data processing workflow, I implemented a suite of pytest tests to validate datasets and relevant transformations. These tests helped ensure the accuracy and reliability of the project's data pipelines and analysis.
