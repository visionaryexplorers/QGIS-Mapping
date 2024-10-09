**Landslide Clustering and Safe Evacuation Zones using GIS and K-Means**

**Project Overview**
This project aims to identify landslide-prone areas in India using a dataset of past landslides and visualize the clusters based on the size of the landslide. The project also identifies safe evacuation zones near these areas by applying the K-Means clustering algorithm. The analysis is done through Python, and the results are visualized on a map using QGIS. The project utilizes geospatial techniques to inform disaster management efforts, providing a valuable tool for identifying high-risk areas and planning evacuations.

**Technologies Used**
- **Jupyter Notebook:** For developing the Python code and running data analysis.
- **QGIS:** A powerful open-source GIS tool for mapping and visualization.
- **Python Libraries:**
- **pandas:** For data manipulation and analysis.
- **geopandas:** For working with geospatial data.
- **matplotlib:** For plotting data.
- **shapely:** For creating and manipulating geometries.
- **scikit-learn:** For applying the K-Means clustering algorithm.
- **Shapefiles:**
- India shapefile for geographical boundaries.
- Landslide data from the provided dataset (with points representing landslides).

**Project Features**
- **Landslide Clustering:** Clusters landslide events based on location and severity (small, medium, large, unknown, catastrophic) using K-Means.
- **Safe Zone Identification:** Identifies safe evacuation zones by analyzing the proximity of these landslide clusters to low-risk areas.
- **Visualizations:** Displays the results on an interactive map using QGIS, with different colors representing the severity of landslides and the corresponding evacuation zones.

**How It Works**

Input Data:
- **India shapefile:** Geographical boundary of India.
- **Landslide dataset:** CSV file containing landslide data with latitude, longitude, and severity classification.

**Steps:**
- Preprocess the data using pandas and geopandas to convert the landslide data into a geospatial format.
- Apply the K-Means clustering algorithm to group landslide events into clusters based on proximity.
- Generate safe evacuation zones around the clusters using buffer geometries.
- Export and visualize the results in QGIS, color-coding the clusters and safe zones for clarity.

**Visualization:**
Different colors represent landslide severity:
- Small: Green
- Medium: Yellow
- Large: Orange
- Unknown: Blue
- Catastrophic: Red
_Safe evacuation zones are highlighted around the clusters._

**How to Run the Project**
- Prerequisites:
-Python 3.x
-QGIS (for visualization)
-Required Python libraries (pandas, geopandas, matplotlib, shapely, scikit-learn)

**Steps to Run:**
- Clone the repository:
  git clone https://github.com/username/project-name.git
- Install the necessary Python packages:
  pip install -r requirements.txt
- Run the Jupyter Notebook to perform the clustering and safe zone analysis.
- Open the QGIS project file (.qgz) and load the shapefiles to visualize the clusters and safe zones on the map.

**Results**
- The results of the analysis include a QGIS map where:
- Landslide locations are marked and color-coded based on severity.
- Safe evacuation zones are displayed around the clusters.
- This project provides an insightful approach to landslide risk analysis using GIS tools and clustering techniques. It can be a crucial aid for disaster management and evacuation planning.

