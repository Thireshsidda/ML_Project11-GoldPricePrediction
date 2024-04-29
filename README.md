# ML_Project11-GoldPricePrediction

### Gold Price Prediction with Lagged Returns - A Linear Regression Approach
This project investigates the potential of using a machine learning model to predict gold price returns using historical data. The model employed is Linear Regression, which aims to establish a linear relationship between a single independent variable (Lagged Return) and the dependent variable (Gold Price Return).

### Data Acquisition and Preprocessing:
The project utilizes a CSV file named "gold_price.csv" containing gold price data.

Pandas is used to read the data, set the 'Date' column as the index, and parse the dates into a datetime format.

Daily price data for USD (PM) is chosen for prediction purposes.

A new column named 'Return' is created to represent the daily percentage change in the USD (PM) price.

Another column named 'Lagged_Return' is created to incorporate the concept of lagged features. It holds the previous day's return value.

Data cleaning is performed by handling missing values using dropna().


### Train-Test Split:
The data is divided into training and testing sets for model development and evaluation.

The training set encompasses data from 2001 to 2018, while the testing set represents data from 2019.

Independent and dependent variables are defined within the training and testing sets:

Independent Variable (X): Lagged Return

Dependent Variable (y): Return

### Model Building and Evaluation:
A Linear Regression model is created using LinearRegression from sklearn.linear_model.

The model is trained on the training data (X_train, y_train).

Predictions are made on the testing data (X_test) using the trained model.

### Visualization of Results:
The predicted gold price returns are plotted against the actual returns for the testing set using matplotlib.

This visual comparison allows for an initial assessment of the model's performance in capturing trends.
Disclaimer:

It's crucial to acknowledge that predicting gold prices is a complex task influenced by various factors beyond historical returns. 

This model serves as a basic example and should not be solely relied upon for financial decision-making.


### Further Exploration:

Explore incorporating additional features beyond lagged returns that might influence gold prices (e.g., economic indicators, global events).

Experiment with different machine learning algorithms like Random Forest or Gradient Boosting for potentially improved prediction accuracy.

Implement model evaluation metrics like Mean Squared Error (MSE) or R-squared to quantitatively assess model performance.

Consider time series forecasting techniques like ARIMA or Prophet for a more robust approach to predicting future gold prices.
