# forecasting_prophet

📊 Data Retrieval and Forecasting Example
This repository demonstrates how to:

Pull time series data from a public dataset (monthly airline passengers).

Walk through a forecasting example using:

Facebook Prophet (additive model with trend & seasonality)

A simple Rolling Moving Average model for baseline comparison.

🔄 What the Code Does
Loads the airline passenger dataset from a public URL.

Prepares the data by renaming columns and parsing dates.

Splits the dataset into training and test sets (last 12 months as test).

Fits a Prophet model and generates 12 months of future forecasts.

Implements a custom rolling average forecast, using the previous 5 months recursively to predict the next 12 months.

Visualizes both forecasts alongside the actuals using an interactive Plotly chart.

📁 Files
forecast_example.py: Main script to load data, fit models, and generate the plot.

README.md: Overview and walkthrough instructions.

📦 Requirements
Make sure you have the following Python packages installed:

bash
Copy
Edit
pip install pandas prophet plotly
▶️ Running the Example
bash
Copy
Edit
python forecast_example.py
This will launch an interactive Plotly chart comparing:

Actual values (historical),

Prophet forecast (with confidence interval),

Rolling moving average forecast (baseline).

📈 Output
The output includes:

Forecast plot comparing Prophet and Rolling Average.

Visual confidence interval for Prophet forecasts.

Forecast start marker for better interpretability.
