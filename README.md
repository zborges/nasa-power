## Quick demo introduction to become more familiar with ArcGIS and .zarr files.

- index.html uses arcGIS JavaScript API to render an interactive map.
- power_connection.py used to retrieve a slice of POWER data from AWS as a CSV.
- region.csv contains the slice of POWER output.


### Resources:
- https://power.larc.nasa.gov/docs/tutorials/service-data-request/aws/
- https://developers.arcgis.com/javascript/latest/sample-code/layers-csv/index.html


## Setup
  
    pip install fsspec pandas xarray
  
   ## Run
  
   1. **Fetch data:**
      ```bash
      python power_connection.py
      ```
      Outputs `region.nc` and `region.csv`.
  
   2. **Visualize:**
      ```bash
      python -m http.server 8000
      ```
      Open http://localhost:8000 in browser.
