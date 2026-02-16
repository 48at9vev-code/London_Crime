# London Crime GEO data analysis
Police data crime analysis for the city of London in 2024-2025 years including creation of a database in PostgreSQL 18.0. Plotting the GEO data on London map, analysing crime hot spots.
---
## Dataset Content
---
> The dataset contains more than 12 000 crime records of the crime happened in London.
> Each row contains data from one single crime and the data per column are described below:
- Crime record Number.
- Month when crime happened.
- Longitude and Latitude of a point of crime.
- Description of location.
- Crime type.
- LSOA code and name (Lower layer Super Output Areas).
- Last outcome data
- Context
## Jupyter Notebook structure
---
The repository contains 2 notebooks:
1. Data processing: pulling the data from https://data.police.uk website, undertaking initial analysis to identify what the data represents and how it can best be transformed to support analysis. For learning purposes a new data base was created. Its structure was rebuilt for efficiency. At the end the data was loaded and check in the database.
2. Data analysing: checking what data is represent.
## Task Requirements
---
- Preparing the data for plotting and clusterisation.
- Analysis the plotted data on the map.
- Locating the crime zones.
- Checking the crime season patterns.
## Hypotheses
---
1. The crime hot spots are located in the central of London.
2. The number of crime goes up and down depends on the time of year.
3. Different type of crime concentrated in some particular areas
## Project Plan
---
The dataset will be extracted from downloaded files, joined and loaded in PostgreSQL database for learning purposes. On completing this task any necessary data cleaning and pre-processing steps will be taking for the further analyses. A copy of the cleaned data is saved for future use.
![The Diagram of created Database](/DB_Diagram.jpg "The Diagram of created Database")
The exploratory data analyses (EDA) will check the distributions of important variables, identify outliers and perform any necessary transformations. The GEO data will then be plotted on London map. The visualisation will provide insights into the relationship among crime data records, and helps in answering the hypotheses.
## Rationale to map task requirements to data visualisations
---
The data visualisations helps to understand how the type of crime related to its locating, the season trends and the crime spots concentration.
## Analysis techniques used
---
The tasks were performed in Python (version 3.14.0) via VScode. Number of Python libraries were used. Pandas for processing the datasets. OS for mapping the the datasets files. SCLalchemy for connecting, inserting and extracting data from the PostgreSQL database. Sklearn.cluster for GEO data clusterisation. Matplotlib.pyplot for plotting and visualisation.
## The conclusion
---
1. The crime concentrated in the main central London areas. The busy is the area more crime is committed. We can see these areas on the London map well. The map can help to be caution when you walk through the dangerous zones.
![The London crime map](/crime_map.png "The London map by crime type")
2. There is no any significant change in crime number over the time. The crime is just slightly less in winter time.
![Crime numbers in London](/crime_over_time.png "Crime numbers in London by type across 2024-2025 years")
## Ethical considerations
---
All data is in the public domain and can be freely used. Ther datasets are cleaned for any private data. GDPR did not apply in this case.
## Credits
---
Datasets were provided by UK Police: https://data.police.uk
Code Institute teaching materials helped a lot throughout this project.
The popular online resources like [Stackoverflow](https://stackoverflow.com), [Geeksforgeeks](https://www.geeksforgeeks.org) and [Medium](https://medium.com) were used number of times for tips, code and suggestions.
