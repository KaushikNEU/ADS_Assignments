# 📘 Crash Course in Forecasting — Feature Engineering & ML-Based Time Series Forecasting

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)

This repository contains my complete submission for the **Crash Course in Forecasting** assignment.  
The project demonstrates how to prepare time-series data for machine learning forecasting using **feature engineering**, **supervised learning transformation**, and **Random Forest regression models**.

---

# 🎞️ Project Preview (GIF)

Below are placeholder GIF previews.  
Replace these paths with actual GIF files once recorded:

```markdown
![Temperature Forecast GIF](path/to/temperature_forecast.gif)
![Airline Forecast GIF](path/to/airline_forecast.gif)
![Milk Production Forecast GIF](path/to/milk_forecast.gif)

📂 Contents
✔ 1. Main Notebook – Daily Temperature Forecasting

Lag features, rolling windows, and Random Forest forecasting using the Daily Minimum Temperatures (Melbourne) dataset.

✔ 2. Example 2 – Airline Passenger Forecasting

Log transform, lag-12 seasonal features, rolling trend, and month-of-year one-hot encoding.

✔ 3. Example 3 – Monthly Milk Production Forecasting

Lag-12 seasonal dependency, rolling mean/std, and seasonal feature engineering.

✔ 4. Supporting YouTube Videos
Example 1 — Daily Temperature

Screen Recording: https://youtu.be/nosSv-yzGv0

Story Video: https://youtu.be/GQJqhdwn0vo

Example 2 — Airline Passengers

Story Video: https://youtu.be/2qoi3dUfSow

Example 3 — Milk Production

Story Video: https://youtu.be/2qoi3dUfSow

🚀 Getting Started

Follow these steps to run the project locally:

1. Clone the repository
git clone https://github.com/your-username/forecasting-assignment.git
cd forecasting-assignment

2. Create a virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

3. Install dependencies
pip install -r requirements.txt

4. Launch Jupyter Notebook
jupyter notebook

5. Open and run the example notebooks

Example_1_Temperature.ipynb

Example_2_Airline_Passengers.ipynb

Example_3_Milk_Production.ipynb

Run all cells from top to bottom.

🎯 Learning Outcomes

By completing this project, you will learn:

📌 Core Time-Series Concepts

Autocorrelation

Trend, seasonality, and variance

Time-aware baseline models

Forecast evaluation (MAE)

📌 Feature Engineering Techniques

Lag features

Rolling windows (trend smoothing)

Rolling standard deviation (volatility)

Month-of-year encodings

Supervised learning transformation for time series

📌 Machine Learning Forecasting Pipelines

Random Forest training for forecasting

Time-aware train–test splitting

Naive baseline comparison (lag_1)

One-step-ahead forecasting

📌 Practical Forecasting Skills

Plotting predictions vs actuals

Working with non-stationary series

Handling seasonal cycles

Building scalable ML-based forecasting workflows

📝 Quiz Section

This project also includes 30 quiz questions, divided based on the examples:

10 questions for Example 1 (Daily Temperatures)

10 questions for Example 2 (Airline Passengers)

10 questions for Example 3 (Milk Production)

All questions include:

Multiple correct answers

Detailed explanations for each option

Coverage of theory + implementation concepts

These quizzes reinforce understanding of forecasting feature engineering and ML workflows.

📚 Datasets Used

Daily Minimum Temperatures (Melbourne) — Jason Brownlee Dataset

International Airline Passengers — Brownlee Dataset

Monthly Milk Production (Pounds per Cow) — Plotly Dataset

All datasets are openly available and widely used in time-series education.

🔗 References

Hyndman, R. J., & Athanasopoulos, G. Forecasting: Principles and Practice

Jason Brownlee – Time Series Forecasting with Python

pandas documentation

scikit-learn documentation

Dataset sources: Brownlee & Plotly repositories

📄 License

This project is licensed under the MIT License.
