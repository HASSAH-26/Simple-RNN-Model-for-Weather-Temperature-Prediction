# Simple-RNN-Model-for-Weather-Temperature-Prediction

🌦️ Weather Temperature Forecasting using SimpleRNN
📌 Overview

This project uses a Simple Recurrent Neural Network (SimpleRNN) to forecast next-day temperature based on historical weather data. The model learns temporal patterns from past observations such as temperature, humidity, wind speed, and pressure.

🎯 Objective

Build a time-series forecasting model using SimpleRNN
Predict next-day temperature using past 7-day weather patterns
Evaluate model performance using regression metrics
Forecast temperature for the next 7 days

📊 Dataset

Source: Kaggle Daily Weather Dataset
Features Used:
Temperature (C) → Target
Humidity
Wind Speed (km/h)
Pressure (millibars)

🧠 Model Architecture

Input Layer → SimpleRNN (64 units) → Dropout (0.2) → Dense (1)
Compilation:
Loss: Mean Squared Error (MSE)
Optimizer: Adam
Metric: Mean Absolute Error (MAE)

⚙️ Workflow

1️⃣ Data Preprocessing
    Handle missing values
    Normalize using MinMaxScaler
    Create 7-day sliding window sequences
    Split into Train / Validation / Test sets
2️⃣ Model Training
    Epochs: 20 (EarlyStopping applied)
    Batch Size: 32
    Validation monitoring enabled
3️⃣ Evaluation
    RMSE
    MAE
    R² Score
    Actual vs Predicted visualization
4️⃣ Forecasting
    Recursive prediction for next 7 days
    Visualization against historical trends

📈 Results

Model learns temperature trends from historical weather patterns
Provides short-term forecasting (7 days)
Performs regression-based prediction with acceptable error range

🛠️ Tech Stack

Python 🐍
TensorFlow / Keras
Pandas & NumPy
Scikit-learn
Matplotlib

📊 Sample Outputs

Training vs Validation Loss
Actual vs Predicted Temperature
7-Day Forecast Plot
