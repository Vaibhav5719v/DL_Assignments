# LSTM Time Series Forecasting

A Deep Learning workflow using an **LSTM (Long Short-Term Memory)** neural network in TensorFlow/Keras to perform time-series forecasting. The project uses daily minimum temperature data (modeled as sales/values), incorporates cyclical feature engineering for seasonal trends, and handles preprocessing strictly to prevent data leakage.

---

## 📌 Features & Highlights

- **Cyclical Encoding**: Captures monthly seasonality using sine and cosine transformations ($Sin\_Month$, $Cos\_Month$).
- **Data Leakage Prevention**: Fits feature and target scalers (`MinMaxScaler`) **only** on the training data.
- **Sequence Generation**: Converts time series data into overlapping sliding windows (lookback period = 12 steps).
- **Test Tail Alignment**: Overlaps the training tail into the testing set so no initial time steps are lost during test evaluation.
- **Early Stopping**: Prevents overfitting by monitoring validation loss (`patience=15`) and restoring the best model weights.

---

## 📁 Repository Structure

```text
.
├── Assignment_4.ipynb    # Main Jupyter Notebook containing data loading, training, & evaluation
└── README.md             # Project documentation
