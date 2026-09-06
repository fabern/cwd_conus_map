# CWDmax map

A single-page map of the maximum cumulative water deficit (`cwd_max`) across the contiguous United States, 2020–2022, at 30 m resolution. The page is built with Quarto from the [GECO leaflet map template](https://github.com/geco-bern/geco-leaflet-map) and published with GitHub Pages.

Live map: https://dafaeh.github.io/ba-cwd-map/

## How the map works

The CWDmax raster is stored as an Earth Engine image asset and served by an Earth Engine App, which renders map tiles on demand at every zoom level. `index.qmd` embeds that app in an iframe and draws the GECO information panel on top of it.

Because the app carries the data, this repository contains no raster files.
The full raster can be accessed on Zenodo: 10.5281/zenodo.22281094

## Data sources

- ET: OpenET DisALEXI monthly at 30 m: https://developers.google.com/earth-engine/datasets/catalog/projects_openet_assets_disalexi_conus_gridmet_monthly_v2_1?hl=de 
- Precipitation and Temperature: DAYMET V4 https://developers.google.com/earth-engine/datasets/catalog/NASA_ORNL_DAYMET_V4?hl=de
- Processing pipeline: https://github.com/dafaeh/ba_faehdavid/tree/main 
