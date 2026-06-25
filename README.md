# 🚗 Chicago Traffic Crashes Data Mining & Predictive Modeling

A comprehensive data science pipeline designed to analyze, clean, and extract hidden patterns from large-scale Chicago traffic crash datasets. This project covers the entire data mining lifecycle, from spatial and temporal feature engineering to predictive machine learning models.

## 📂 Project Structure & Artifacts

The repository is structured to separate source pipelines, cleaned data artifacts, and narrative visualizations:
- **`traffic/`**: Core directory housing the data mining algorithms, spatial processing scripts, and predictive models.
- **`clean_data/`**: Sub-directory dedicated to holding processed, merged, and curated dataset outputs.
- **`temp/`**: Temporary tracking files used during the data transformation stage.
- **`*.png` (Visual Artifacts)**: Dynamic graphical plots generated from Exploratory Data Analysis (EDA), including:
  - `sunburst_plot.png` & `sunburst_plot2.png`: Hierarchical breakdowns of contributing crash factors.
  - `fig_lat.png` & `fig_lon.png`: Geospatial distribution mapping of accident coordinates.
  - `grouped.png` & `AIRBAG_DEPLOYED.png` & `SAFETY_EQUIPMENT.png`: Visual statistical relations between safety features and injury levels.

## 🚀 Key Pipeline Architecture

### 1. Data Cleaning & Geospatial Engineering
- **Missing Value Imputation**: Handled null values logically across critical columns (weather, lighting, and road conditions) by mapping them to standardized fallback values.
- **Geospatial Feature Engineering**: Integrated and mapped geographical coordinates (latitude and longitude) to precisely isolate accident hotspots.
- **Data Joins & Aggregation**: Successfully merged multi-relational datasets combining core crash incidents with separate files detailing vehicle and person profiles (drivers, passengers).

### 2. Exploratory Data Analysis (EDA) & Insights
- Evaluated temporal crash trends to uncover seasonal, weekly, and hourly traffic accident behaviors.
- Analyzed cross-features combining weather conditions, illumination factors, and vehicle types.
- Generated narrative visualization plots highlighting safety parameters like airbag deployments and driver licensing statuses.

### 3. Machine Learning & Pattern Mining
- **Classification Models**: Built predictive machine learning classifiers to determine and predict crash severity, identifying potential risk factors for severe injuries or fatalities.
- **Association Rule Mining**: Implemented the **Apriori algorithm** to extract actionable patterns and underlying causal relationships governing traffic mishaps.
- **Clustering Analysis**: Applied unsupervised clustering algorithms to isolate high-density geographic accident zones (Hotspots).

## 🛠️ Tech Stack & Tooling

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Folium/Geopandas (Geospatial)
- **Environment**: Structured Python and Jupyter Scripts

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Ensure your local environment has the required libraries installed:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Execute scripts within the `traffic/` directory to reproduce the cleaning pipeline and modeling steps.
