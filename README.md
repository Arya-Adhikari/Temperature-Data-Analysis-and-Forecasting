Temperature Data Analysis and Forecasting

Overview
This project demonstrates a simple approach to analyzing and forecasting daily temperature data using Python. It utilizes synthetic temperature data to perform exploratory data analysis, generate naive and moving average forecasts, and evaluate the accuracy of the forecasting models using the Mean Absolute Error (MAE).

Features
•	Synthetic Temperature Data Generation: Generates daily temperature data for one year.
•	Data Storage & Loading: Saves the generated data into a CSV file and reloads it for analysis.
•	Exploratory Data Analysis (EDA): Visualizes temperature trends over time.

•	Forecasting Models:
o	Naïve Forecast: Assumes tomorrow's temperature will be the same as today's.
o	Moving Average Forecast: Uses a 7-day rolling average to predict temperatures.

•	Error Evaluation: Calculates the MAE for both forecasting models.
•	Future Forecasting: Predicts the next 7 days' temperatures using the moving average method.

Installation

To run this project, ensure you have Python installed along with the following dependencies:
pip install numpy pandas matplotlib scikit-learn

Usage
1.	Run the Script: Execute the Python script to generate and analyze temperature data.
python temperature_forecasting.py
2.	View Data: The script prints the first few rows of the dataset.
3.	Visualizations: Graphs for temperature trends, naive forecasting, moving average forecasting, and future predictions are displayed.
4.	Error Metrics: The MAE values for both forecasting models are printed.
5.	Future Forecast: A 7-day temperature forecast is printed and visualized.

Code Explanation
1. Data Generation
•	Generates synthetic temperature data with seasonal variations and random noise.
•	Saves the dataset as temperature_data.csv.

2. Data Processing & Visualization
•	Loads the data and converts the date column into a datetime format.
•	Plots the temperature trend over the year.

3. Forecasting Models
•	Naïve Forecast: Uses today's temperature as tomorrow's prediction.
•	Moving Average Forecast: Uses a 7-day rolling average.

4. Model Evaluation
•	Computes the Mean Absolute Error (MAE) for both models.

5. Future Forecasting
•	Uses the last 7 days’ moving average to predict the next 7 days.
•	Displays and plots the forecast.

Output
•	CSV file: temperature_data.csv
•	Visualizations: Temperature trends, forecasts, and predictions.
•	Forecast metrics (MAE values) displayed in the console.
•	7-day future temperature predictions printed and plotted.

Example Output
Naïve Forecast MAE: 2.50
Moving Average Forecast MAE: 1.75

License
This project is open-source and available for educational and research purposes.

