# Forecasting Daily Price GBP/USA Direction

This notebook aims to forecast the daily price direction for GBP/USA using various technical indicators and simple technical trading rules. The main steps in the notebook are as follows:

1. Load Datasets
2. Exploratory Data Analysis (EDA) & Preprocessing
3. Engineering Features:
   - ***y_label*** (Buy, sell, Hold) based on α
   - ***Technical Indicators***:
     - The Weighted Moving Average (WMA)
     - The Exponential Moving Average (EMA)
     - The simple moving average (SMA)
     - The Relative Strength Index (RSI)
     - The Average Directional Index (ADX)
     - The Commodity Channel Index (CCI)
     - The Rate-of-Change (ROC)
     - The Bollinger Band (BB)
     - The Moving Average Convergence Divergence (MACD)
     - The Moving Polynomial Trending
   - ***And Simple Technical Trading Rules***
4. EDA again
5. Preprocessing
6. Implementing the base paper model (CNN-GRU)
7. Improving accuracy

## Packages, Libraries, Functions

The notebook uses various packages, libraries, and custom functions for data manipulation, visualization, and modeling. The main libraries include:
- pandas
- numpy
- scikit-learn
- tensorflow and keras
- seaborn
- plotly
- matplotlib

## Dataset

The notebook uses GBP/USA historical data from Investing.com, covering the date range from 01/01/2017 to 25/04/2023. The dataset contains OHLCV (Open, High, Low, Close, Volume) data for each trading day.

## Experiments with Alpha and Window Size

The notebook performs experiments with different alpha thresholds and sliding window sizes to create the models. The alpha threshold is used to determine the daily price direction (Buy, Sell, Hold), and the sliding window size is used for sequence generation in the models. The experiments involve two models: CNN+GRU and CNN+GRU with self-attention.

![newplot (1)](https://github.com/ozzmanmuhammad/Forecasting-Daily-Price-Direction/assets/93766242/f3138513-fa26-4459-80cd-62578e928afc)


## Note

Please note that this is an automatically generated copy of the original notebook, and any modifications or updates made to the original notebook after the generation date are not reflected here. To access the most up-to-date version of the notebook, refer to the link provided for the original notebook.
