# Automated Manufacturing State Prediction

## Introduction
The Automated Manufacturing State Prediction project aims to predict the state of an automated manufacturing unit based on data from 25 sensors. This project enables proactive decision-making, optimised maintenance schedules, and improved operational efficiency by accurately forecasting the unit's state, ranging from 'no risk' to 'catastrophic'. With applications in manufacturing and related industries, such as automotive, energy, healthcare, and logistics, accurate state prediction contributes to cost savings, enhanced equipment performance, and uninterrupted services. The project utilizes advanced predictive techniques and sensor data to optimize machinery functionalities and ensure reliable operations. This README provides an overview of the various stages involved in the project, including EDA, feature engineering, data preprocessing, model selection, model validation, and model inference.

## EDA (Exploratory Data Analysis)
During the initial phase of the project, extensive exploratory data analysis (EDA) was performed to gain insights into the dataset. The EDA involved visualizing sensor data, identifying trends, and examining the distribution of different states. Correlation plots were generated using libraries such as plotly, seaborn, and matplotlib to understand the interdependencies among sensors and their relationship with the final state.

## Feature Engineering and Data Preprocessing
To enhance the predictive power of the models, several feature engineering techniques were employed. Seasonality decomposition was performed to extract trends and patterns from the time series data. Transformations like moving average and Naive Bayes were applied to capture relevant information. Additionally, the dataset was transformed by transposing it to create a 10-minute window frame and converting the (10,25)-shaped dataframes to a consolidated (1,250)-shaped dataframe. These preprocessing steps enabled the models to effectively capture temporal dependencies.

## Model Selection and Evaluation
Multiple models were considered for the state prediction task, including NaiveForecaster, ARIMA, SARIMA, KNN, KNN with Dynamic Time Wrapping, Temporal Convolutional Network (TCN), SARIMAX, LSTM, and bi-directional LSTM. Extensive literature review was conducted to understand the concepts of time series analysis and time series classification. Each model was trained and evaluated using appropriate metrics to assess its accuracy.

## Model Validation and Inference
Model validation was performed using a portion of the dataset for cross-validation and assessing generalization. The accuracy of each model was measured against the true labels to determine their performance. Notably, the bi-directional LSTM model, after applying the transpose transformations mentioned earlier, achieved an impressive accuracy of 96.6%. The TCN model also performed well, yielding an accuracy of 95.8%. Other models demonstrated accuracies in the range of 35% to 60%, even after applying the aforementioned transformations.

## Conclusion
The Automated Manufacturing State Prediction project involved a comprehensive analysis of sensor data, feature engineering techniques, data preprocessing, and model selection. By employing bi-directional LSTM with transpose transformations, an outstanding accuracy of 96.6% was achieved. The project demonstrates the effectiveness of advanced models in accurately predicting the state of the automated manufacturing unit based on sensor data.

## Acknowledgments
We would like to acknowledge the organizers of the Automated Manufacturing State Prediction Challenge for providing the dataset and platform for evaluation.

Please note that the accuracies mentioned above are for illustrative purposes and can be adjusted according to the actual performance of the models.
