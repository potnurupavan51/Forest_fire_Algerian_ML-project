# **Algerian Forest Fires Project**

## **Overview**

This project analyzes the Algerian Forest Fires Dataset to understand the factors contributing to forest fires in two regions of Algeria: Bejaia and Sidi Bel-abbes. The dataset includes weather conditions and fire weather indices (FWI) for the period from June 2012 to September 2012\. The analysis involves data cleaning, exploratory data analysis (EDA), and building regression models to predict the Fire Weather Index (FWI).

## **Dataset Description**

The dataset contains 244 instances (122 for each region) with 14 attributes, including weather data, FWI components, and a class label indicating whether a fire occurred.

### **Attributes**

* **Date:** Day, month, and year of the observation.  
* **Temperature:** Noon temperature (Celsius).  
* **RH:** Relative Humidity (%).  
* **Ws:** Wind speed (km/h).  
* **Rain:** Total daily rainfall (mm).  
* **FFMC:** Fine Fuel Moisture Code index.  
* **DMC:** Duff Moisture Code index.  
* **DC:** Drought Code index.  
* **ISI:** Initial Spread Index.  
* **BUI:** Buildup Index.  
* **FWI:** Fire Weather Index (target variable).  
* **Classes:** 'Fire' or 'Not Fire'.  
* **Region**: 0 for "Bejaia Region Dataset", 1 for "Sidi-Bel Abbes Region Dataset"

### **Data Source**

Algerian Forest Fires Dataset

## **Data Cleaning**

The data cleaning process involves the following steps:

* Removing null values.  
* Splitting the dataset into two regions.  
* Converting columns to appropriate data types.  
* Removing irrelevant columns ('day', 'month', 'year').

## **Exploratory Data Analysis (EDA)**

EDA is performed to visualize the data and understand the relationships between different attributes. This includes:

* Plotting histograms to show the distribution of numerical features.  
* Plotting a pie chart to visualize the distribution of fire and non-fire instances.  
* Calculating and visualizing the correlation matrix using a heatmap.  
* Creating box plots.  
* Monthly fire analysis.

## **Feature Selection**

* Checking for multicollinearity and dropping the features 'BUI' and 'DC'

## **Model Training and Evaluation**

Several regression models are trained to predict FWI, including:

* Linear Regression  
* Lasso Regression  
* Ridge Regression  
* Elastic Net Regression

The performance of each model is evaluated using Mean Absolute Error (MAE) and R-squared.

## **Results**

The Linear Regression model performs the best, with the lowest Mean Absolute Error and the highest R-squared score.

## **File Structure**

* README.md: This file.  
* Algerian\_forest\_fires\_cleaned\_dataset.csv: Cleaned dataset.  
* Algerian\_forest\_fires\_dataset\_UPDATE.csv: Raw dataset.  
* notebook: Jupyter Notebook with the data processing, model training, and evaluation code.

## **Usage**

1. Clone the repository.  
2. Ensure you have the required Python libraries installed (pandas, numpy, matplotlib, seaborn, scikit-learn).  
3. Run the Jupyter Notebook to reproduce the analysis and modeling.
