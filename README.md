This repository contains two files related to the optimization of regression and classification models for earthquake prediction. Various machine learning models, including KNN, Random Forest, and XGBoost, were used to analyze earthquake-related data.
Classification Model Optimization: Machine learning models were optimized for classifying earthquake occurrences.
Regression Model Optimization: Regression models were fine-tuned to forecast earthquake magnitudes. 

**Data Source**

The earthquake data were accessed through the USGS API (United States Geological Survey), providing real-time and historical seismic event records. from 1960 to the present. This starting point was selected due to the lack of reliable data before 1960. To compile a comprehensive dataset, earthquake data were collected within two radii—500 km and 1000 km—from the center of Almaty (approximately 76.9285°E, 43.2565°N). This dataset extends beyond Almaty, covering regions in Kyrgyzstan and China, which have historically experienced significant earthquakes affecting Almaty. Since some machine learning models require large datasets to perform well, the two different distance ranges were considered to enhance model training efficiency.
