# PRODIGY_DS_05
# US Traffic Road Accident Risk Factors and Hotspot Analysis

## Project Overview

Traffic accidents remain a significant public safety concern across the United States. Understanding when, where, and why accidents occur is essential for improving road safety and developing better traffic management strategies.

This project analyzes a large-scale US traffic accident dataset to identify patterns related to time, weather conditions, road infrastructure, and geographic location. Using exploratory data analysis and geospatial visualizations, the study highlights accident hotspots and key factors influencing accident occurrence.

The analysis aims to uncover data-driven insights that can help policymakers, urban planners, and transportation authorities better understand traffic accident patterns.

---

## Dataset

This project uses the **US Accidents Dataset (2016–2023)** available on Kaggle.

Dataset characteristics:

- 7.7+ million accident records
- 49 US states covered
- 46+ features describing accident conditions

### Key Variables

- Accident time and duration
- Geographic coordinates (latitude & longitude)
- Weather and environmental conditions
- Road infrastructure attributes
- Accident severity levels

Dataset Source:  
https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents

---

## Project Workflow

### 1. Data Loading and Inspection

- Imported the dataset using Pandas
- Explored dataset structure using:
  - shape
  - info
  - descriptive statistics
- Identified missing values and feature distributions

---

### 2. Data Cleaning and Preprocessing

Key preprocessing steps included:

- Handling missing values
- Converting timestamp fields to datetime format
- Removing unnecessary or redundant columns
- Ensuring consistent data types

---

### 3. Data Optimization

Because the dataset contains millions of rows, memory optimization techniques were applied:

- Converted object columns to categorical data types
- Reduced numeric data types where possible
- Optimized memory usage for efficient analysis

After optimization, the dataset memory usage was significantly reduced, enabling faster analysis.

---

### 4. Feature Engineering

Additional features were created to support temporal analysis:

- Hour of the accident
- Day of the week
- Month and year
- Accident duration

These features helped analyze time-based accident trends.

---

## Exploratory Data Analysis

The analysis focused on identifying patterns in accident occurrence using multiple visualizations.

### Temporal Patterns

Accident frequency was analyzed across:

- Hour of the day
- Day of the week
- Month and seasonal variations

Key finding:  
Accidents peak during **morning and evening rush hours**, reflecting commuter traffic patterns.

---

### Weather Impact

Weather conditions were analyzed to understand their influence on accidents.

Findings show that:

- Most accidents occur during clear weather conditions, primarily due to higher traffic volume.
- Rain, fog, and snow increase accident risk because of reduced visibility and road friction.

---

### Road Infrastructure Factors

Road features such as:

- Traffic signals
- Junctions
- Crossings
- Stop signs

were analyzed to determine their relationship with accident frequency.

Results indicate that **intersections and traffic signals are high-risk locations** due to complex vehicle interactions.

---

## Geospatial Analysis

To identify accident hotspots, geospatial visualizations were created using **Folium and Plotly**.

Key visualizations include:

- State-level accident distribution
- Interactive accident hotspot maps
- Choropleth maps showing accident density by state

Major accident clusters were observed in:

- Southern California (Los Angeles region)
- San Francisco Bay Area
- Texas urban corridor (Dallas–Houston–Austin)
- Florida metropolitan areas
- Northeast corridor (Washington DC → New York → Boston)

These regions correspond to **highly urbanized areas with dense traffic networks**.

---

## Key Insights

- Urban areas exhibit the highest accident densities due to high traffic volumes and complex road networks.
- Rush-hour commuting periods significantly increase accident occurrence.
- Weather conditions and visibility influence accident risk and severity.
- Road infrastructure elements such as intersections and traffic signals are high-risk accident zones.
- Major interstate transportation corridors align with accident hotspots.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Folium
- Jupyter Notebook

---

## Data Citation

This project uses the **US Accidents Dataset** compiled and maintained by Sobhan Moosavi and collaborators.  
If you use this dataset in research or publications, please cite the following papers:

Moosavi, S., Samavatian, M. H., Parthasarathy, S., & Ramnath, R. (2019).  
*A Countrywide Traffic Accident Dataset.*

Moosavi, S., Samavatian, M. H., Parthasarathy, S., Teodorescu, R., & Ramnath, R. (2019).  
*Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights.*  
Proceedings of the **27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems (SIGSPATIAL '19)**.

Dataset Source:  
https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents

You can access the project in the below drive link:
https://drive.google.com/drive/folders/1boNyiW98fG5_vycDY2_zZip_YAx96Wo5?usp=sharing
