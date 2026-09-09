# Flight-ticket-price-estimation
Flight Ticket Price Estimation is a machine learning project that predicts flight ticket prices based on airline, source, destination, travel month, booking time, number of stops, and flight duration. It uses Linear Regression to estimate ticket prices.

# Flight Ticket Price Estimation

## Overview

Flight Ticket Price Estimation is a machine learning project that estimates the price of a flight ticket using different flight and booking details. The project analyzes factors such as airline, source, destination, travel month, days before booking, number of stops, and flight duration.

The project uses Linear Regression to predict flight ticket prices.

## Objectives

* Explore and analyze flight booking data.
* Identify factors affecting ticket prices.
* Compare ticket prices between airlines and routes.
* Prepare and preprocess the dataset.
* Train a machine learning regression model.
* Estimate the price of a new flight.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

## Dataset Features

The dataset contains:

* Flight ID
* Airline
* Source
* Destination
* Travel Month
* Days Before Booking
* Stops
* Duration in Hours
* Ticket Price

### Target Variable

`ticket_price` is the target variable that the model predicts.

## Data Preprocessing

The project performs the following steps:

1. Loads the flight dataset using Pandas.
2. Checks the dataset shape and missing values.
3. Handles missing numerical values using the median.
4. Handles missing categorical values using the most frequent value.
5. Standardizes numerical features using StandardScaler.
6. Converts categorical features into numerical form using One-Hot Encoding.
7. Splits the data into training and testing sets.

## Machine Learning Algorithm

The project uses **Linear Regression**, a supervised machine learning algorithm used for predicting continuous numerical values.

The model learns the relationship between flight details and ticket prices to estimate the price of a new flight.

## Model Evaluation

The model is evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score
* Actual vs Predicted Price Comparison

## New Flight Prediction

The project creates an example flight with details such as airline, source, destination, travel month, booking time, stops, and duration.

The trained model then estimates the ticket price for this new flight.

## Visualizations

The project generates the following charts:

* Flight Duration vs Ticket Price
* Booking Lead Time vs Ticket Price
* Average Ticket Price by Airline
* Actual vs Predicted Ticket Prices

## Project Structure

```text
Flight_Ticket_Price_Estimation/
│
├── README.md
├── requirements.txt
├── flight_data.csv
└── flight_ticket_price_estimation.py
```

## How to Run

### 1. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 2. Run the Python Program

```bash
python flight_ticket_price_estimation.py
```

## Output

The program displays:

* Dataset information
* Missing value information
* MAE
* RMSE
* R² Score
* Actual and predicted ticket prices
* Estimated price for a new flight
* Important factors affecting ticket prices

It also generates four visualization files:

```text
duration_vs_price.png
booking_days_vs_price.png
airline_vs_price.png
actual_vs_predicted.png
```

## Applications

Flight price estimation can help users and travel-related businesses:

* Understand factors affecting flight prices.
* Compare prices between airlines.
* Analyze booking patterns.
* Estimate the price of a future flight.

## Dataset Note

The included flight dataset is synthetic and intended for educational and classroom machine-learning practice.

## Conclusion

This project demonstrates how machine learning can be used to estimate flight ticket prices. It combines data preprocessing, Linear Regression, model evaluation, and data visualization to build a complete price estimation system.
