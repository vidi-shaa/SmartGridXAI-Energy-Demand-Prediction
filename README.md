# SmartGridXAI: Explainable AI for Electricity Consumption Prediction

AI and machine learning are used to build a predictive model of electricity consumption based on smart meter data and environmental factors (e.g., temperature, humidity). The model will use these inputs to predict energy consumption driven by various factors. The project uses Python and RapidMiner to implement an end-to-end workflow, including predictive modelling with machine learning and explaining model output using explainable AI (EAI) techniques (SHAP and LIME). 

Electricity consumption rates can vary widely depending on external conditions and a user's historical use of their electrical service. To provide the necessary forecasts for effective energy management, smart grid infrastructure planning, and sustainable energy use, an accurate estimate of electricity consumption is required. The goal of this project is to create a predictive model that provides interpretable insights into how it arrives at its predictions.

The data for this project consists of about 5000 rows of smart meter data with the following features: 
Temperature, Humidity, Wind Speed, Average Daily/Weekly Historical Usage, Current Hour, and Current Day. The target variable is (Electricity Consumed).

The data preprocessing steps included: 
- Timestamp converted to Hour and DayOfWeek
- Removed irrelevant features 
- Categorical features were coded for processing in a machine learning model 
- The final data was split into two datasets, one for training purposes and one for testing.

The method for predicting electricity consumption used a Random Forest Regressor. This model can capture non-linear relationships among features and the target variable, while providing interpretable insights into which features are available to explain the predictions.

The model evaluation is completed using three Key Performance Indicators (KPIs): 
MSE (Mean Squared Error), MAE (Mean Absolute Error), and R² (Coefficient of Determination).

The application interface and dashboard environment were designed using Mendix. The platform enables the creation of interactive dashboards and decision-support workflows that allow users to monitor electricity consumption patterns and interpret machine learning predictions effectively.

Explainable AI: 
To provide interpretability of the model predictions, we employed SHAP (SHapley Additive Explanations) for determining feature significance across the entire data set as well as LIME (Local Interpretable Model-Agnostic Explanations) for providing insight into individual model predictions. Therefore, we can determine which independent variables contribute most to total electricity consumption.

Findings: 
The key findings from our model were; Average prior consumption is the number one predictor of electricity consumption, and various types of weather (temperature and humidity) affect overall consumption. Also, time-dependent factors (e.g., hour and day of the week) correlate with the amount of power consumed during those periods.

Overall Project Architecture: 
Data Source → Data Preparation → Random Forest Machine Learning → Electricity Consumption Forecasting → Explainable AI Methods (SHAP and LIME)

Technologies: 
The software used in this project was Python, Scikit-learn, SHAP, LIME, Pandas, Matplotlib, Seaborn, and RapidMiner.
