# SmartGridXAI: Explainable AI for Electricity Consumption Prediction

Overview:-
SmartGridXAI is a machine learning project that predicts electricity consumption using smart meter and environmental data. The system integrates predictive modelling with explainable AI techniques to understand the factors influencing energy demand.
The project demonstrates an end-to-end data analytics workflow using Python and RapidMiner, along with explainability techniques such as SHAP and LIME.

Problem Statement:-
Electricity consumption fluctuates due to environmental conditions and historical usage patterns. Accurate forecasting of electricity demand is essential for efficient energy management, smart grid planning, and sustainability.
This project builds a predictive model to estimate electricity consumption while providing interpretable insights into the factors driving the predictions.

Dataset:-
The dataset contains 5000 records of smart meter data with the following features:
Temperature
Humidity
Wind Speed
Average Past Consumption
Hour of the Day
Day of the Week
Target variable:
Electricity_Consumed

Methodology:-
1. Data Preprocessing
Timestamp converted into Hour and DayOfWeek
Removal of irrelevant features
Encoding of categorical variables
Train-test split of the dataset
2. Machine Learning Model
A Random Forest Regressor is used to predict electricity consumption because it can capture nonlinear relationships between variables.
3. Model Evaluation
The model is evaluated using:
Mean Squared Error (MSE)
Mean Absolute Error (MAE)
R² Score

Explainable AI:-
To improve the interpretability of predictions, the project uses:
SHAP (SHapley Additive Explanations)
Identifies the global importance of the features that affect electricity demand.
LIME (Local Interpretable Model-Agnostic Explanations)
Explains individual predictions made by the model.
These techniques help understand which factors most strongly influence electricity consumption.

Results:-
Key insights from the model:
Average Past Consumption is the strongest predictor of electricity usage.
Weather variables, such as temperature and humidity, also affect electricity demand.
Temporal features such as hour and day of the week influence consumption patterns.

Project Architecture:-
Dataset
↓
Data Preprocessing
↓
Random Forest Model
↓
Energy Demand Prediction
↓
Explainable AI (SHAP + LIME)

Technologies Used:-
Python
Scikit-learn
SHAP
LIME
Pandas
Matplotlib
Seaborn
RapidMiner
