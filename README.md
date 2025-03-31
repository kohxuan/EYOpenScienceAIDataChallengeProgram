# 🛰️ Urban Heat Island (UHI) & Geospatial Analysis
The **Urban Heat Island (UHI) & Geospatial Analysis** project focuses on analyzing satellite imagery and weather data to study urban heat patterns. The notebook utilizes geospatial datasets, machine learning, and remote sensing techniques to assess the impact of land cover and building density on temperature variations.
<br><br>

### ✨ Features
- **Geospatial Data Processing**: Reads and processes building footprints (`.kml`), weather data (`.xlsx`), and thermal imagery.
- **Urban Heat Island (UHI) Index Computation**: Analyzes temperature variations using satellite-based Land Surface Temperature (LST).
- **Building Footprint Analysis**: Extracts spatial features from `.kml` data.
- **Machine Learning Model**: Trains predictive models using `Training_data_uhi_index.csv` and generates benchmark results.
- **Weather Data Integration**: Incorporates meteorological observations (`NY_Mesonet_Weather.xlsx`) to enhance analysis.
- **Submission Template**: Provides `Submission_template.csv` for structured model predictions.
<br>

### 🏆 Results
We are proud to announce that our team, **DatAi**, achieved significant recognition in the **2025 EY Open Science AI and Data Challenge: Cooling Urban Heat Islands**. Our project was ranked:
- **79th internationally** out of 2076 participants.
- **11th in Malaysia**, showcasing our strong regional performance.

Our model achieved an accuracy of **96.78%**, demonstrating its effectiveness in predicting urban heat patterns.

This accomplishment highlights our team's dedication and expertise in utilizing AI and geospatial analysis to address urban heat challenges. We are excited to continue contributing to innovative solutions for sustainable urban environments.
- **Team Members:**
   - [Ong Yi Yan](https://github.com/ONGYIYAN) - Team Leader
   - [Tang Yan Qing](https://github.com/yan-qing09)
<br>

### 🛠️ Technical Overview
- **Python**: Primary language for geospatial and statistical analysis.
- **geopandas & rasterio**: Handles vector and raster data processing.
- **xarray & rioxarray**: Processes satellite-derived thermal imagery.
- **pandas & numpy**: Data wrangling and feature engineering.
- **scikit-learn**: Machine learning model training and evaluation.
- **matplotlib & seaborn**: Visualization of UHI patterns.
<br>

### 📁 File Structure
- **Building_Footprint.kml**: Contains spatial information of buildings.
- **Landsat_LST.ipynb**: Jupyter Notebook for processing Land Surface Temperature data.
- **NY_Mesonet_Weather.xlsx**: Weather dataset for atmospheric data integration.
- **Sentinel2_GeoTIFF.ipynb**: Notebook for processing Sentinel-2 imagery.
- **Training_data_uhi_index.csv**: Dataset used for model training and evaluation.
- **Submission_template.csv**: Format for submitting results.
- **UHI Experiment Sample Benchmark.ipynb**: Baseline notebook for UHI model evaluation.
- **Model.ipynb**: Jupyter Notebook containing the full implementation of data processing, feature extraction, and model training.
<br>

### 🚀 Getting Started
1. **Set Up Environment**: Ensure Python and Jupyter Notebook are installed.
2. **Install Dependencies**: Run the following command:
   ```sh
   pip install geopandas rasterio xarray pystac_client planetary_computer rioxarray scikit-learn pandas numpy matplotlib seaborn fiona rtree odc-stac
   ```
3. **Run the Notebooks**: Open and execute `Landsat_LST.ipynb` and `Sentinel2_GeoTIFF.ipynb` to process geospatial data.
<br>

### 🌍 Data Sources
- **Satellite Imagery**: Landsat & Sentinel-2 for analyzing land surface temperature.
- **Building Footprint Data**: Extracted from `.kml` file.
- **Weather Data**: Meteorological observations from New York Mesonet dataset.
<br>

### 🔍 Analysis Workflow:
1. **Data Loading:**
   - Imported geospatial data (`.kml`, `.tiff`, `.csv`, `.xlsx`).
   - Read weather and satellite imagery datasets.
2. **Feature Engineering:**
   - Computed UHI index using LST from Landsat.
   - Integrated building density and land cover statistics.
3. **Model Training:**
   - Built predictive models using `RandomForestRegressor` for temperature forecasting.
   - Validated model performance with benchmark comparisons.
4. **Exporting Results:**
   - Processed predictions stored in `Submission_template.csv`.
   - Results visualized using GIS and data plotting tools.
<br>
