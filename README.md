# Canada ODCAF Clustering Project

This project demonstrates the use of clustering algorithms, specifically **DBSCAN** and **HDBSCAN**, to analyze and visualize cultural and art facilities across Canada. The dataset used is the **Open Database of Cultural and Art Facilities (ODCAF)**, which contains information about the names, types, and locations of various facilities.

## Project Overview

The project includes the following key steps:
1. **Data Preparation**:
   - Importing and cleaning the dataset.
   - Filtering the data to include only museums.
   - Removing invalid or missing coordinates and converting them to the appropriate format.

2. **Clustering with DBSCAN**:
   - Applying the DBSCAN algorithm to cluster museums based on their geographical proximity.
   - Visualizing the clusters on a basemap of Canada.

3. **Clustering with HDBSCAN**:
   - Applying the HDBSCAN algorithm for hierarchical clustering.
   - Visualizing the hierarchical clusters on a basemap of Canada.

4. **Visualization**:
   - Using GeoPandas and Contextily to overlay clustered locations on a basemap of Canada.

## Dataset Information

- **Source**: [The Open Database of Cultural and Art Facilities (ODCAF)](https://www.statcan.gc.ca/en/lode/databases/odcaf)
- **License**: Open Government License - Canada
- **Data Fields**:
  - `ODCAF_Facility_Type`: Type of facility (e.g., museum, gallery, etc.)
  - `Latitude` and `Longitude`: Geographical coordinates of the facility.

## Requirements

The following Python libraries are required to run the project:
- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `hdbscan`
- `geopandas`
- `contextily`
- `shapely`

Install the required libraries using:
```bash
pip install numpy pandas matplotlib scikit-learn hdbscan geopandas contextily shapely
```

## How to Run

1. Clone the repository or download the project files.
2. Open the Jupyter Notebook file `Canada_ODCAF_Clustring.ipynb`.
3. Follow the notebook cells step-by-step to execute the code and visualize the results.

## Results

- **DBSCAN Clustering**:
  - Identifies clusters of museums based on proximity using a fixed neighborhood radius.
  - Noise points (unclustered museums) are labeled as `-1`.

- **HDBSCAN Clustering**:
  - Provides a hierarchical clustering approach with adaptive cluster sizes.
  - More robust to varying densities compared to DBSCAN.

## References

- [ODCAF Landing Page](https://www.statcan.gc.ca/en/lode/databases/odcaf)
- [ODCAF Data Download (ZIP)](https://www150.statcan.gc.ca/n1/en/pub/21-26-0001/2020001/ODCAF_V1.0.zip?st=brOCT3Ry)

## License

This project is licensed under the Open Government License - Canada. For more details, visit [Open Government License](https://open.canada.ca/en/open-government-licence-canada).
