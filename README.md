# Employment Centers
## This repository is an analytical toolkit composed of jupyter notebooks written in python that identifies, describes, and analyzes the critical employment centers in the San Diego region. 

## Setup Instructions
Lodes.ipynb - This notebook pulls in LODES data to identify employment centers and create “lodes.parquet”, which is used across the other notebooks. Please run this notebook first to identify employment centers and ensure access to “lodes.parquet”.
This notebook has been set-up to rely on data acquired through GeoSNAP.
The get_lodes function is used to select for the specific locational and temporal area of study.
The notebook subsets the LODES data at an initial minimal threshold for employment centers at 4,000 total employees.
The following notebooks perform analysis on the identified employment centers and can be run in any order:
“demographics.ipynb” - spatial demonstration of various demographic groups and other societal indicators for residents and employees of employment centers 
“Transit_Accessibility.ipynb” - A spatial exploration of transit stops in and around employment centers with multiple interactive maps for visualization
“history.ipynb” - *insert description here*
“specialization.ipynb” 
Measures the amount of employees in each industry sector as well as overall diversity of industries within employment centers
Certain columns renamed or dropped for convenience and readability
WARNING: examining the industry sector specialization of highly populous employment centers may not reveal LODES areas with high specialization, but low total employees; adjust the EC threshold in the “lodes.ipynb” to suit your analysis goals.

## Important Data & Tools:

All data used in this project is open source and freely available for use, sharing, and modification.

LODES: https://lehd.ces.census.gov/data/#lodes
California Transit Stops: https://data.ca.gov/dataset/ca-transit-stops
GTFS: https://gtfs.org/
GeoSNAP: https://github.com/oturns/geosnap
Open Street Map: https://www.openstreetmap.org/relation/396482
Pandana for Network Analysis: https://udst.github.io/pandana/network.html
Usage:
This repository can be used to learn more about employment centers in San Diego, or adapted to analyze employment centers in other regions. Using this repository, information about population demographics, employment industry specialization, employment center spatial changes over time, and employment center transit accessibility are all readily available and displayed visually. To adapt this repository to analyze other regions, LODES data for that region will need to be imported, new transit data found, and isochrone networks will need to be attuned to the new region.

## Academic Sources Related to This Project:
Our primary guidance on employment center identification: Li, T., & Dodson, J. (2020). Job growth, accessibility, and changing commuting burden of employment centres in Melbourne. Journal of Transport Geography, 88, 102867. https://doi.org/10.1016/j.jtrangeo.2020.102867
Primary academic guidance on transit accessibility: Moran, M. M. (2013). Walking the walk: an assessment of the 5-minute rule in transit planning. https://repositories.lib.utexas.edu/server/api/core/bitstreams/4273837d-334d-49a3-9a9e-98629e74eb64/content
Foundational Isochrone Information: https://www.mapbox.com/insights/isochrones
Identifying public transport gaps using time-dependent accessibility levels https://doi.org/10.1016/j.jtrangeo.2015.09.008
The importance of recurring public transport delays for accessibility and mode choice https://doi.org/10.1016/j.jtrangeo.2024.103796
Towards transit equity in Detroit: An assessment of microtransit and its impact on employment accessibility https://doi.org/10.1016/j.trd.2022.103341
Passive transit accessibility: Modelling and application for transit gap analysis and station area assessment https://doi.org/10.1016/j.jtrangeo.2023.103757
Sectoral heterogeneity, accessibility and population–employment dynamics in Dutch cities https://doi.org/10.1016/j.jtrangeo.2012.06.013
Urban public transport system accessibility for different groups of residents: Case of Bratislava city https://doi.org/10.1016/j.cstp.2024.101200
# Project Proposal
## Timeline for project:
April 18: Project Proposal Due - Identify data sources and literature
April 22-26: Use LODES to identify geographic concentrations of employment and Calculate pedestrian and transit accessibility measures using Open-StreetMap and GTFS data
April 29-May 3: Measure urban agglomeration, employment specialization, and comparative advantage. Examine change in employment specialization and/or spatial footprint over time. Create Presentation
May 6-10: Present Project to class on May 7 and finalize repository



