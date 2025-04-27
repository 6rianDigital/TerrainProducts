# Halifax Regional Municipality - Terrain Products for Fire Hazard Mapping

### Overview
This project performs terrain analysis on a given dataset to compute slope, aspect, and elevation models, specifically focusing on fire hazard mapping for the Halifax Regional Municipality (HRM). It uses Google Earth Engine (GEE) to process Sentinel-2 satellite imagery and DEM (Digital Elevation Models) data to generate fire hazard layers.

### Purpose
The purpose of this project is to assess the fire hazard levels across various regions within HRM by analyzing terrain factors such as slope, aspect, and elevation. This will help to identify high-risk areas for wildfires, aiding in resource allocation and planning for fire prevention strategies.

### Requirements
- Python 3.13.1
- Google Earth Engine API
- geemap library for visualization
- Access to Sentinel-2 satellite imagery and DEM data

### Setup and Installation
1. Install the required libraries:
    ```bash
    pip install geemap
    pip install earthengine-api
    ```

2. Authenticate Google Earth Engine:
    ```python
    import ee
    ee.Authenticate()
    ```

3. Initialize Google Earth Engine:
    ```python
    ee.Initialize(project='your_project_id')
    ```

### Functionality
- **Terrain Analysis**: Computes slope, aspect, and elevation models.
- **Fire Hazard Mapping**: Classifies terrain based on slope and aspect to create fire hazard levels.
- **Satellite Imagery**: Processes and visualizes cloud-free Sentinel-2 imagery for HRM regions.
- **Interactive Map**: Displays results in an interactive map using the geemap library.

### Features
- Terrain splitting into 4 sections for more granular analysis.
- Cloud masking for satellite images.
- Dynamic visualization of terrain features and fire hazard zones.
