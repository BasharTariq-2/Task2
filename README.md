# Task 2: Predict Future Stock Prices (Short-Term)

## Objective
The goal of this project is to predict the **next day's closing price** of a stock using historical market data. For this task, we used **Tesla Inc. (TSLA)** stock data fetched from Yahoo Finance.

## Dataset
- **Source**: Yahoo Finance (retrieved using the `yfinance` Python library)
- **Time Period**: [Specify time range you used, e.g., Last 2 Years]
- **Features Used**:
  - Open Price
  - High Price
  - Low Price
  - Volume
- **Target Variable**: Next Day's Closing Price

## Workflow Summary
1. **Data Fetching**: Used `yfinance` to download Tesla's historical stock data.
2. **Data Preprocessing**:
   - Shifted 'Close' column to create 'Next_Close' as the prediction target.
   - Handled missing values after shifting.
3. **Feature Selection**:
   - Used ['Open', 'High', 'Low', 'Volume'] as input features.
4. **Model Training**:
   - Split the dataset into Training (80%) and Testing (20%) sets.
   - Trained a **Random Forest Regressor** model.
5. **Evaluation**:
   - Evaluated model performance using **Root Mean Squared Error (RMSE)**.
   - Plotted Actual vs Predicted Closing Prices.
6. **Visualization**:
   - Time series plot of Actual vs Predicted prices to visually assess model accuracy.

## Results
- **RMSE**: [Insert RMSE result from notebook]
- The model is able to follow the trend of closing prices with reasonable accuracy, but may lag in highly volatile conditions.

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Stock-Price-Prediction-Task.git
   cd Stock-Price-Prediction-Task
