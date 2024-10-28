Oakland CA Weather Prediction Model
This project analyzes weather data from the Oakland International Airport to predict daily maximum temperatures using historical weather patterns. The model leverages Ridge regression to forecast the next day's maximum temperature based on factors like precipitation and temperature history.

Project Structure
Data Preprocessing: Handles missing data by forward-filling and setting precipitation to 0 where applicable.
Feature Engineering: Creates additional features such as monthly temperature averages and ratios of daily max and min temperatures.
Model Training: Trains a Ridge regression model with selected predictors to minimize mean squared error.
Evaluation: Measures model accuracy and visualizes predictions versus actual temperatures.
Data Description
The dataset (WO1.csv) includes daily weather observations with columns:

DATE: Date of observation
PRCP: Daily precipitation
TMAX: Maximum temperature
TMIN: Minimum temperature
Additional columns indicate various weather conditions (e.g., WT01 for fog).
Requirements
Python 3.x
Libraries:
pandas
scikit-learn
matplotlib
Usage
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/Oakland_CA_Weather_Model.git
cd Oakland_CA_Weather_Model
Run the Notebook: Open the notebook in Jupyter or Google Colab and execute the cells to load the dataset, preprocess data, and train the model.

Customize Predictors: Adjust predictor variables in the predictors list to experiment with model accuracy.

Visualizations
Plots of temperature and precipitation trends over time.
Comparison plot of actual vs. predicted temperature values.
Results
The Ridge regression model’s coefficients and errors are displayed, providing insights into the predictive power of each feature.
