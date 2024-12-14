# Stock-Market-Trend-Prediction-Using-Time-Series-Analysis

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Features](#features)
- [Models Implemented](#models-implemented)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Data](#data)
- [Usage](#usage)
- [Results](#results)
- [Evaluation Metrics](#evaluation-metrics)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview
This project focuses on building a stock price prediction model using multiple time series forecasting techniques. The models included are:

1. Long Short-Term Memory (LSTM)
2. ARIMA (AutoRegressive Integrated Moving Average)
3. GARCH (Generalized Autoregressive Conditional Heteroskedasticity)
4. ETS (Exponential Smoothing)
5. XGBoost (Extreme Gradient Boosting)

The goal is to compare the performance of each model in predicting stock closing prices. The dataset used for this project includes historical stock price data from `BAJFINANCE.NS`.

---

## Project Structure
```plaintext
.
├── data/
│   └── Bajaj Stock Dataset.csv  # Stock price data
├── models/
│   ├── lstm.py             # LSTM model implementation
│   ├── arima.py            # ARIMA model implementation
│   ├── garch.py            # GARCH model implementation
│   ├── ets.py              # ETS model implementation
│   └── xgboost.py          # XGBoost model implementation
├── notebooks/
│   └── stock_prediction.ipynb  # Jupyter notebook for model training and evaluation
├── requirements.txt        # Dependencies required to run the project
├── README.md               # Project README file
└── LICENSE                 # Project License

```

## Features

	•	Multiple Models: Implementation of LSTM, ARIMA, GARCH, ETS, and XGBoost for stock price prediction.
	•	Data Preprocessing: MinMax scaling for data normalization and handling missing values.
	•	Model Comparison: Evaluation of model performance using mean squared error (MSE) and mean absolute error (MAE).
	•	Visualization: Comparison plots showing actual vs predicted stock prices for each model.
	•	Early Stopping: LSTM model uses early stopping to avoid overfitting.

## Models Implemented

1. LSTM:

	•	Deep learning model capable of capturing long-term dependencies in time series data.
	•	Used multiple features: ‘Close’, ‘Open’, ‘High’, ‘Low’, and ‘Volume’.

2. ARIMA:

	•	Statistical model designed for univariate time series data, capturing linear trends and patterns.

3. GARCH:

	•	Model specialized in predicting volatility in financial time series.

4. ETS:

	•	Captures trend and seasonality in time series using exponential smoothing.

5. XGBoost:

	•	Powerful machine learning algorithm known for its high predictive performance on structured data.

## Technologies Used

	•	Python: Core programming language.
	•	TensorFlow / Keras: Deep learning library used for LSTM implementation.
	•	Statsmodels: Used for ARIMA and ETS model implementations.
	•	ARCH: Used for GARCH model implementation.
	•	XGBoost: For implementing the XGBoost algorithm.
	•	Matplotlib: For visualizing predictions vs actual prices.

## Installation

To run this project locally, follow these steps:

1.	Clone the repository:
git clone https://github.com/mohit0825/Stock-Market-Trend-Prediction-Using-Time-Series-Analysis-With-Python.git

2.	Navigate into the project directory:
cd Stock-Market-Trend-Prediction-Using-Time-Series-Analysis

3.	Install the required dependencies:
pip install -r requirements.txt

Make sure to have the Bajaj Stock Dataset.csv dataset in the data/ folder.

## Data

The dataset used is Bajaj Stock Dataset.csv, which contains the following columns:

	•	Date: Date of stock trading.
	•	Open: Opening price of the stock.
	•	High: Highest price of the stock for the day.
	•	Low: Lowest price of the stock for the day.
	•	Close: Closing price of the stock.
	•	Volume: Number of stocks traded.

Ensure that the dataset is placed in the data/ directory.

## Usage

To run the model training and evaluation, follow these steps:

	1.	Open the notebooks/stock_prediction.ipynb Jupyter notebook.
	2.	Execute the cells to train the models and generate predictions.
	3.	Visualize the results using the plots generated by the notebook.

Alternatively, you can run individual model scripts from the models/ directory.

## Results

The models were evaluated using the following metrics:

	•	Mean Squared Error (MSE)
	•	Mean Absolute Error (MAE)

The LSTM model generally performed better at capturing the complex patterns in stock prices compared to the other models, especially for long-term trends.

## Evaluation Metrics

The following evaluation metrics were used to compare the models:

	•	Mean Squared Error (MSE): Measures the average squared difference between predicted and actual values.
	•	Mean Absolute Error (MAE): Measures the average absolute difference between predicted and actual values.

Results for each model can be found in the output of the Jupyter notebook.

## Contributing

Contributions are welcome! If you’d like to contribute, please follow these steps:

	1.	Fork the repository.
	2.	Create a new feature branch (git checkout -b feature-branch).
	3.	Commit your changes (git commit -m 'Add new feature').
	4.	Push to the branch (git push origin feature-branch).
	5.	Create a new Pull Request.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact

For any questions or suggestions, please contact:

	•	Mohit Kumar
	•	Email: mk1695@srmist.edu.in
	•	GitHub: mohit0825
