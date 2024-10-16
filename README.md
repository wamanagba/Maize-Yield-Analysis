# Maize-Yield-Analysis


- This project involves predicting maize yield in Togo and Benin using MODIS vegetation indices (NDVI and EVI). The workflow includes geospatial data wrangling, feature extraction, and machine learning model building to assess yield predictions based on vegetation data.



-	Data Wrangling: Import and merge administrative boundaries for Togo and Benin, and extract vegetation features from MODIS VI data, including NDVI and EVI. Missing data values were masked based on metadata.

-	Feature Extraction: Extract mean, minimum, and maximum values for NDVI and EVI for each administrative polygon at levels 1 and 2. Data reshaped into a wide format for model input.

-	Modeling: Implemented ridge regression models using vegetation indices to predict maize yield. Cross-validation was performed to optimize the model, and feature encoding was used to account for regional differences.

-	Evaluation: Compared performance between models at different administrative levels, with better results found at level 1 aggregation due to reduced variability.

-	Visualization: Created scatter plots to evaluate model predictions against observed yield, highlighting the accuracy of the models.

## Key Files

- modis_vi.nc: MODIS vegetation index data file.

- Scripts: Python scripts for data extraction, transformation, modeling, and evaluation.

- Outputs: Plots and CSV files summarizing the features and model results.

## Results
The model predictions at level 1 showed an R² of 0.64, demonstrating reasonable predictive power. 