📌 Project Overview

This project aims to predict market crop prices using historical mandi data such as crop type, variety, location (state, district, market), and arrival quantity. The model is built using an Artificial Neural Network (ANN) implemented in TensorFlow/Keras, and trained on a clean, preprocessed dataset derived from multiple Excel files.
🧠 Problem Statement

Agricultural market prices often fluctuate due to various factors like location, crop type, and arrivals. This project helps:

    Farmers: to forecast prices for better planning

    Traders/Buyers: to identify price trends

    Policy makers: to analyze market behavior

🛠 Tech Stack

    Python

    TensorFlow / Keras

    Pandas, NumPy, Scikit-learn

    Matplotlib (for visualizations)

📊 Dataset Features

    📍 Categorical Fields: State Name, District Name, Market Name, Variety, Crop

    📦 Numerical Field: Arrivals (Tonnes)

    🎯 Target Variable: Modal Price (Rs./Quintal)

All categorical fields were one-hot encoded, and missing values were handled using median imputation.
🧪 Model Architecture

    Input Layer: Size = Number of input features (dynamic)

    Hidden Layer 1: 64 Neurons, ReLU activation

    Hidden Layer 2: 32 Neurons, ReLU activation

    Output Layer: 1 Neuron (Linear, for regression)

-Loss Function: Mean Squared Error (MSE); 
-Optimizer: Adam; 
-Metric: Mean Absolute Error (MAE)


📈 Model Performance :
Test Loss (MSE)   ->	4390.35
Test MAE	    ->      29.90 Rs.


💾 Output

    ✅ Trained model: crop_price_ann_model.h5

    ✅ Loss & MAE plots over 100+ epochs

    ✅ Predictive model ready for deployment or inference

🚀 Future Improvements

    Add time-series component (monthly trends)

    Use advanced models like LSTM or XGBoost for comparison

    Build a simple web interface using Streamlit or Flask
