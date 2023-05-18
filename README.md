# Cement Strength Prediction with PySpark's MLlib

[![Language Badge](https://img.shields.io/badge/Language-Python-blue.svg)](https://www.python.org/)
[![PySpark Badge](https://img.shields.io/badge/PySpark-3.1.2-e25a1c.svg)](https://spark.apache.org/docs/latest/api/python/index.html)
[![Library Badge](https://img.shields.io/badge/Library-Pandas-yellow.svg)](https://pandas.pydata.org/)
[![Library Badge](https://img.shields.io/badge/Library-Scikit--learn-orange.svg)](https://scikit-learn.org/)
[![License Badge](https://img.shields.io/badge/License-CC%20BY--NC%204.0-0a2c46.svg)](https://creativecommons.org/licenses/by-nc/4.0/legalcode)

This project involves building a regression model using PySpark's MLlib to predict the compressive strength of cement based on its ingredients. The dataset consists of 1030 instances of concrete samples, containing 9 attributes (8 continuous and 1 discrete), and 1 continuous quantitative output variable.

Our goal is to identify the features that are the strongest predictors of cement strength and provide recommendations for optimal values of cement ingredients. We will also create an application where users can input their own values for age and get a predicted value for cement strength.

## Prerequisites

Before running the code, you will need to have the following installed:

- PySpark: the Python API for Apache Spark
- Jupyter Notebook: an interactive development environment for Python


## Dataset

The dataset used in this project is the [Concrete Compressive Strength Data Set](https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength) from the UCI Machine Learning Repository. It contains 1030 instances of concrete samples, with 9 attributes (8 continuous and 1 discrete) and 1 continuous quantitative output variable (compressive strength).

| Column Name       | Data Type | Measurement Unit | Description                                      |
|-------------------|----------|------------------|---------------------------------------------------|
| cement            | double   | kg/m3            | Input variable                                    |
| slag              | double   | kg/m3            | Input variable                                    |
| flyash            | double   | kg/m3            | Input variable                                    |
| water             | double   | kg/m3            | Input variable                                    |
| superplasticizer  | double   | kg/m3            | Input variable                                    |
| coarseaggregate   | double   | kg/m3            | Input variable                                    |
| fineaggregate     | double   | kg/m3            | Input variable                                    |
| age               | integer  | days             | Input variable                                    |
| csMPa (compressive strength)| double | MPa | Output variable                               | 


## Usage

To run the code, open the `Cement_Strength_Prediction.ipynb` file in Jupyter Notebook and execute the cells in order. The notebook contains detailed explanations of each step in the code and the results obtained.

To use the application for predicting cement strength based on user input, run the `predict_cement_strength` function in the notebook after it has been defined. This function takes a single argument `age` (in days) and returns the predicted cement strength (in MPa).
