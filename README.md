# 🛰️ Geospatial Data Analysis - Satellite Imagery & Building Feature Extraction
The **Geospatial Data Analysis - Satellite Imagery & Building Feature Extraction** project focuses on processing satellite imagery and geospatial data using Python. It leverages remote sensing techniques to analyze land cover, building footprints, and environmental features using machine learning.
<br><br>

### ✨ Features
- **Geospatial Data Processing**: Extracts and processes satellite imagery and vector data.
- **Building Feature Extraction**: Computes statistics on building density, height, and footprint areas.
- **Satellite Image Analysis**: Fetches and processes Landsat and Sentinel-2 imagery using cloud-based STAC API.
- **Median Composite Mosaics**: Generates clear, noise-reduced satellite images for analysis.
- **Machine Learning Models**: Implements `RandomForestRegressor` for predictive geospatial analysis.
<br>

### 🛠️ Technical Overview
- **Python**: Primary programming language.
- **geopandas & rasterio**: Geospatial data processing.
- **xarray & rioxarray**: Satellite image analysis.
- **pystac_client & planetary_computer**: Accesses cloud-based satellite imagery.
- **scikit-learn**: Machine learning for predictive modeling.
<br>

### 📁 File Structure
- **Model.ipynb**: Jupyter Notebook containing the full implementation of data processing, feature extraction, and model training.
- **output_mosaic.tiff**: Processed median composite of satellite imagery.
- **building_features.csv**: Extracted building statistics used for modeling.
<br>

### 🚀 Getting Started
1. **Set Up Environment**: Ensure Python and Jupyter Notebook are installed.
2. **Install Dependencies**: Run the following command:
   ```sh
   pip install geopandas rasterio xarray pystac_client planetary_computer rioxarray scikit-learn tqdm seaborn matplotlib fiona rtree odc-stac
   ```
3. **Run the Notebook**: Open and execute `Model.ipynb` in Jupyter Notebook to process geospatial data.
<br>

### 🛰️ Geospatial Data Sources
- **Satellite Imagery**: Landsat & Sentinel-2 (retrieved via Microsoft Planetary Computer).
- **Vector Data**: Building footprints and land-use datasets.
<br>

### 🔍 Data Processing Steps:
1. **Data Loading:**
   - Loaded geospatial data using `geopandas` and `rasterio`.
   - Accessed cloud-based satellite imagery through `pystac_client`.
2. **Feature Extraction:**
   - Computed statistics on building footprints and land cover.
   - Created median composite images from Landsat and Sentinel-2.
3. **Model Training:**
   - Used extracted features to train a `RandomForestRegressor`.
   - Evaluated model performance using `r2_score`.
4. **Exporting:**
   - Saved processed satellite imagery as `.tiff` files.
   - Stored extracted building statistics in `.csv` format.
<br>
