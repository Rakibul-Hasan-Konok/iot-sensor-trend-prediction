# IoT Sensor Data Trend Prediction

## Dataset
NASA C-MAPSS Turbofan Engine Degradation Dataset.

## Industrial Context
This dataset represents turbofan engine sensor readings collected over operational cycles. The objective is to predict Remaining Useful Life (RUL) for predictive maintenance.

## Target Variable
Remaining Useful Life (RUL)

## Data Cleaning
- Forward fill and backward fill for missing values
- IQR clipping for outlier spikes
- Sorting by engine ID and cycle to maintain time order

## Feature Engineering
- Lag features to capture previous sensor behavior
- Rolling mean and rolling standard deviation to capture degradation trend

## Model
Random Forest Regressor

## Evaluation Metrics
- MAE
- RMSE
- R2 Score

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook