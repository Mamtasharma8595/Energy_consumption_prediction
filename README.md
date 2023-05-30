# Energy Consumption Prediction using LSTM#
This code performs energy consumption prediction using an LSTM (Long Short-Term Memory) model. It analyzes historical energy consumption data and predicts future energy consumption values based on the learned patterns.
## Dependencies
•	pandas
•	numpy
•	matplotlib
•	seaborn
## Dataset
The energy consumption data is stored in a CSV file (AEP_hourly.csv). The code loads the data into a pandas DataFrame and performs initial exploratory analysis.
## Data Preprocessing
•	The code extracts additional features from the datetime column, such as month, year, date, time, week, and day of the week.
•	The dataset is resampled to daily frequency for modeling purposes.
•	The dataset is split into a training set and a test set.
## LSTM Model
•	The LSTM model is constructed using the Keras Sequential API.
•	The model consists of multiple LSTM layers with dropout regularization to prevent overfitting.
•	The output layer is a dense layer with a single unit.
•	The model is compiled with the Adam optimizer and mean squared error loss function.
## Training and Prediction
•	The training set is prepared by reshaping the data and applying feature scaling.
•	The LSTM model is trained on the training set.
•	The test set is prepared and passed to the trained model for predicting future energy consumption values.
•	The predicted values are inverse transformed to obtain the original scale.
## Results Visualization
•	The true and predicted energy consumption values are stored in a DataFrame for comparison.
•	The true and predicted values are visualized over time using line plots.

