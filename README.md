# Irvine Package Theft
This repository contains all files used in analyzing petty theft (package, vehicle, garage) in Irivne, CA (2011-2019). The result is an **[interactive map](https://hassenmorad.github.io/irvine.html)** that allows users to look for general patterns and correlations between these different categories of theft.

*The first iteration of this project (Irvine Theft Mapping.ipynb) was a [time-lapse video](https://youtu.be/a6sYRXIeFhY). It was created from images of monthly package theft incidents plotted via matplotlib.

## Workflow Summary:
1. Collection
    - Requested theft data from the Irvine Police Dept. and the US Postal Service via [FOIA](https://en.wikipedia.org/wiki/Freedom_of_Information_Act_(United_States)) requests
    - Extracted the lat/lon coordinates of each theft record via Google Maps API 
2. Cleaning
    - Manually corrected a few lat/lon coordinates returned from google maps API
3. Visualization
    - Converted data from csv to geojson
    - Uploaded to Mapbox template
    - Added interactive map elements via Mapbox GL JS (irvine_theft.html)
