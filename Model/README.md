## Structure Overview

```

Model/
├── Statistical/              # Classical statistical models
│   ├── LinearRegression/     # Basic LR, LR with CalendarFourier & DeterministicProcess
│   ├── ARIMA/                # AutoRegressive Integrated Moving Average
│   └── FFT/                  # Fast Fourier Transform for frequency analysis
│
├── MachineLearning/          # Gradient boosting and feature-based models
│   └── LightGBM/             # Light Gradient Boosting Machine
│
├── DeepLearning/             # Neural network-based forecasting
│   ├── RNN/                  # Recurrent Neural Network
│   ├── GRU/                  # Gated Recurrent Unit
│   └── LSTM/                 # Long Short-Term Memory
│
├── utils/                    # Helper functions (preprocessing, evaluation, visualization)
└── saved\_models/             # Serialized model weights/checkpoints

```

---

## Model Descriptions

### 🔹 Statistical Models
- **Linear Regression (LR):** Baseline model to capture linear relationships between time and stock price.  
- **LR-CF-DP:** Extended linear regression with Calendar Fourier terms (seasonality) and Deterministic Process (trend).  
- **ARIMA:** Captures autoregressive and moving average components in time series data.  
- **FFT:** Identifies cyclical patterns and dominant frequencies in stock price movements.  

### 🔹 Machine Learning
- **LightGBM:** Gradient boosting decision tree model, efficient for handling non-linear relationships and feature interactions.  

### 🔹 Deep Learning
- **RNN:** Sequential model capturing short-term dependencies in time series.  
- **GRU:** Variant of RNN with gating mechanisms, more efficient for long sequences.  
- **LSTM:** Advanced recurrent architecture addressing vanishing gradients, proven effective for 30-, 60-, and 90-day forecasts.  

---

## Utilities
The `utils/` folder contains reusable scripts:
- **data_preprocessing.py** – Cleaning, normalization, and train-test split functions.  
- **evaluation.py** – Metrics including RMSE, MAPE, and MSLE.  
- **visualization.py** – Functions to plot predicted vs. actual stock prices.  

---

## Training & Evaluation Workflow
1. **Preprocess data** using utilities (normalization, feature engineering).  
2. **Train models** with scripts inside each subfolder.  
3. **Evaluate performance** using RMSE, MAPE, and MSLE across multiple horizons (30, 60, 90 days).  
4. **Save models** into `saved_models/` for reproducibility and deployment.  

---

## Example Results

- **LSTM** achieved **MAPE < 3.5%**, outperforming ARIMA (≥30%) and FFT (≥60%).  
- **LightGBM** provided competitive accuracy with fast training times.  
- Statistical models (LR, ARIMA) served as interpretable baselines for comparison.  

---

## Learning Outcomes
- Hands-on experience implementing **statistical, ML, and DL forecasting models**.  
- Ability to compare performance across different modeling families.  
- Exposure to **model saving/loading workflows** for reproducibility.  
- Demonstrated improvements in accuracy for **Vietnamese stock market forecasting**.  
