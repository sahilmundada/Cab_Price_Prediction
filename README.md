# Cab_Price_Prediction

🚕 Cab Price Prediction

This project focuses on building a machine learning model that accurately predicts cab fare prices based on input features such as pickup/dropoff locations, distance, passenger count, and time of travel.


📌 Table of Contents
About the Project

Tech Stack

Dataset Description

Features Used

Modeling Approach

Installation

How to Use

Results

Future Work


🧠 About the Project

Cab fare prices can be affected by various factors like location, distance, and time. This project applies machine learning techniques to develop a model that can predict the fare amount based on these features.


🛠 Tech Stack

🐍 Python 3.x

📊 Pandas, NumPy, Matplotlib, Seaborn

📈 Scikit-learn, XGBoost, LightGBM

📍 Folium / Geopy (for location-based distance calculations)


📂 Dataset Description

Dataset: NYC Taxi Fare Prediction

pickup_datetime: Date and time of the ride

pickup_longitude, pickup_latitude: GPS location of pickup

dropoff_longitude, dropoff_latitude: GPS location of dropoff

passenger_count: Number of passengers

fare_amount: Target variable to predict


🧾 Features Used

Haversine Distance (calculated using coordinates)

Day of week, hour of day from datetime

Passenger count

Optional: Weather info, traffic info, etc.


🔍 Modeling Approach

Data Cleaning – Removing outliers, handling missing values

Feature Engineering – Creating new features like distance, time-of-day

Model Selection – Linear Regression, Decision Trees, Random Forest, XGBoost

Evaluation Metrics – RMSE, MAE, R² Score

Hyperparameter Tuning – GridSearchCV / RandomizedSearchCV


⚙️ Installation

bash

git clone https://github.com/sahilmundada/Cab_Price_Prediction.git
cd cab-price-prediction
pip install -r requirements.txt

▶️ How to Use

bash

python main.py
Or use the notebook:

bash

jupyter notebook Cab_Price_Prediction.ipynb


📊 Results

Model	RMSE	R² Score

Linear Regression	5.27	0.65

Random Forest	3.90	0.82

XGBoost	3.75	0.84


🚀 Future Work

Add weather and traffic data

Deploy as a web app using Streamlit or Flask

Integrate with a live map API
