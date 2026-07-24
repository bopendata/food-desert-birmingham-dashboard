# Food Desert Dashboard with Network Dataset Overlay

**Location:** Birmingham City, Jefferson County, Alabama  
**Version:** 1.0

## Overview

This interactive dashboard was developed using **QGIS2Web** to visualize food accessibility across Birmingham City, Alabama.

The dashboard integrates residential parcel data, healthy food outlet locations, transportation networks, and administrative boundaries to support food accessibility assessment, urban planning, and spatial equity analyses.

The package includes the interactive dashboard, downloadable processed datasets, and supporting spatial layers used in the analysis.


## Project Attribution

This dashboard and associated datasets were developed as part of the **B-Open Project**, a research initiative at the School of Engineering, University of Alabama at Birmingham (UAB). The work was developed by the research teams of Dr. Avinash Unnikrishnan and Dr. Moiz Usmani.


## Contents

```
index.html              Main interactive dashboard
data/                   Spatial data files used by the dashboard
dataset/                Processed datasets and downloadable data products
css/                    Stylesheets
js/                     JavaScript files
legend/                 Map legend resources
webfonts/               Font resources used by the dashboard
documentation/          Detailed methodology, workflow, and dataset documentation
README.md               This file
```


## Opening the Dashboard

Open the file:

```
index.html
```

using a modern web browser such as:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox

If the dashboard does not display correctly due to browser security restrictions, serve the project folder using a local web server (for example, VS Code Live Server).


## Dashboard Layers

The dashboard includes the following datasets and map layers:

- Residential Parcel Dataset
- Healthy Food Outlet Locations
- Road Network Dataset
- Functional Road Classification
- Census Blocks
- Census Block Groups
- Neighborhood Boundaries
- Community Areas
- City Council Districts
- Birmingham City Boundary
- County Boundaries


## Data Sources

The dashboard was prepared using publicly available datasets from the following sources:

- Birmingham Land Parcel Ownership and Land Use Dataset
- Birmingham Open Data Portal
- FHWA and ALDOT GIS Data
- OpenStreetMap (Overpass Turbo)
- TIGER/Line Census Geography
- Google Maps (for reference store information where applicable)

Complete source information, metadata, methodology, and supporting documentation are available in the accompanying `documentation/` folder.

## Processed Datasets

The processed datasets include:

- Residential parcel polygons
- Residential parcel centroids
- Healthy food outlet locations
- Parcel-to-nearest grocery store network distances
- Multi-scale aggregated accessibility datasets:
  - Census Blocks
  - Census Block Groups
  - Neighborhoods
  - Community Areas
  - City Council Districts

The processed datasets are provided in GIS-compatible and tabular formats for mapping and further analysis.


## Analysis Summary

Healthy food outlets were identified using OpenStreetMap Points of Interest based on selected retail categories representing grocery stores, supermarkets, specialty fresh food retailers, and public food markets.

Residential parcels were converted to centroid points and matched to the nearest food outlet using a transportation network. Network-based shortest path distances were calculated using **OSMnx** and **NetworkX**, allowing each parcel to be assigned its nearest grocery store and corresponding travel distance.

Parcel-level accessibility results were subsequently aggregated to multiple geographic levels, including:

- Census Blocks
- Census Block Groups
- Neighborhoods
- Community Areas
- City Council Districts

These aggregated datasets support broader spatial analysis and planning applications.


## Documentation

For detailed information regarding:

- Data sources
- Data processing workflow
- Network analysis methodology
- Multi-scale aggregation methodology
- Data dictionary
- Analytical summaries

please refer to:

`documentation/` folder


## Notes

This dashboard is intended for visualization and analytical purposes.

Food accessibility classifications are based on network travel distance to the nearest healthy food outlet using the methodology described in the project documentation.

Users requiring updated datasets should consult the original data providers.


## Citation

If you use this dataset, dashboard, or any derived products, please cite:

> Author(s). (Year). *Title of the manuscript*. SSRN / arXiv.  
> DOI/Identifier: `<DOI or arXiv ID>`  
> Available at: `<Preprint URL>`

Please use the journal citation instead if a peer-reviewed version becomes available.


## Contact

For questions regarding this dataset or dashboard, please contact:

**Name:**  
**Affiliation:**  
**Email:**  