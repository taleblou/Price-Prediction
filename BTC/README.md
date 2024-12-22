# Bitcoin Price Prediction with Artificial Intelligence

This repository contains experiments and analysis for predicting Bitcoin prices using various artificial intelligence (AI) models. The models are evaluated based on key metrics such as R-squared, Mean Squared Error (MSE), and Mean Absolute Error (MAE).

## Table of Contents

1. [Overview](#overview)
2. [Methodology](#methodology)
3. [Results](#results)
4. [Performance Tables](#performance-tables)
5. [Notable Observations](#notable-observations)
6. [Conclusion](#conclusion)
7. [Research Links](#research-links)
8. [License](#license)

## Overview

This project evaluates multiple machine learning and deep learning models to predict four types of Bitcoin prices:

- Close Price
- Open Price
- High Price
- Low Price

Each model's performance is ranked using the following criteria:

1. Primary: R-squared (higher is better)
2. Secondary: Mean Squared Error (lower is better)
3. Tertiary: Mean Absolute Error (lower is better)

The code for all models is available on my [GitHub](https://github.com/taleblou) and can be used for free. Visit the repository to explore the implementation and experiments.

## Methodology

The following models were implemented and evaluated:

- **Traditional Models**: Support Vector Regression (SVR), ARIMA, SARIMAX, Linear Regression, etc.
- **Tree-based Models**: Gradient Boosting Regressor, Random Forest, XGBoost, CatBoost, LightGBM
- **Neural Networks**: RNN (LSTM), GRU, BiLSTM, TransformerModels, WaveNet, Temporal Convolutional Networks (TCN)

Key metrics used for evaluation include:

- **R-squared**: Explains variability in the data.
- **Mean Squared Error (MSE)**: Captures average squared differences.
- **Mean Absolute Error (MAE)**: Represents average absolute error.

## Results

### Close Price Prediction

Top performers:

- **SVR**: R-squared = 0.982, MSE = 0.000416, MAE = 0.014585
- **ARIMA**: R-squared = 0.982, MSE = 0.000426, MAE = 0.014705

### Open Price Prediction

Top performers:

- **SVR**: R-squared = 0.982, MSE = 0.000411, MAE = 0.014526
- **ARIMA**: R-squared = 0.981, MSE = 0.000427, MAE = 0.014710

### High Price Prediction

Top performers:

- **SVR**: R-squared = 0.986, MSE = 0.000329, MAE = 0.012558
- **ARIMA**: R-squared = 0.986, MSE = 0.000336, MAE = 0.012666

### Low Price Prediction

Top performers:

- **SVR**: R-squared = 0.983, MSE = 0.000389, MAE = 0.014369
- **ARIMA**: R-squared = 0.982, MSE = 0.000403, MAE = 0.014740

## Performance Tables

### Open Price Performance Table:
| Rank | Model Name                | R-squared  | MSE      | MAE      |
| ---- | ------------------------- | ---------- | -------- | -------- |
| 1    | SVR                       | 0.981835   | 0.000411 | 0.014526 |
| 2    | ARIMA                     | 0.981189   | 0.000427 | 0.014710 |
| 3    | GradientBoostingRegressor | 0.965593   | 0.000779 | 0.020569 |
| 4    | LinearRegression          | 0.963184   | 0.000834 | 0.021416 |
| 5    | RandomForest              | 0.962704   | 0.000845 | 0.020602 |
| 6    | RNN (LSTM)                | 0.962581   | 0.000849 | 0.023862 |
| 7    | BiLSTM                    | 0.972269   | 0.000630 | 0.019660 |
| 8    | GRU                       | 0.970064   | 0.000680 | 0.019089 |
| 9    | kNN                       | 0.957707   | 0.000958 | 0.021439 |
| 10   | CatBoost                  | 0.956434   | 0.000987 | 0.021942 |
| 11   | DecisionTrees             | 0.950722   | 0.001116 | 0.023772 |
| 12   | XGBoost                   | 0.952521   | 0.001076 | 0.022370 |
| 13   | SARIMAX                   | 0.940447   | 0.001349 | 0.028063 |
| 14   | TCN                       | 0.960726   | 0.000890 | 0.022126 |
| 15   | LightGBM                  | 0.861705   | 0.003133 | 0.032595 |
| 16   | Prophet                   | 0.675307   | 0.007355 | 0.061558 |
| 17   | WaveNet                   | -9.404321  | 0.235697 | 0.461659 |
| 18   | TransformerModels         | -28.734728 | 0.673571 | 0.652279 |

### High Price Performance Table:
| Rank | Model Name                | R-squared  | MSE      | MAE      |
| ---- | ------------------------- | ---------- | -------- | -------- |
| 1    | SVR                       | 0.985805   | 0.000329 | 0.012558 |
| 2    | ARIMA                     | 0.985507   | 0.000336 | 0.012666 |
| 3    | GradientBoostingRegressor | 0.968907   | 0.000721 | 0.018323 |
| 4    | RandomForest              | 0.969408   | 0.000709 | 0.018019 |
| 5    | LinearRegression          | 0.969334   | 0.000711 | 0.018990 |
| 6    | GRU                       | 0.967341   | 0.000757 | 0.020970 |
| 7    | BiLSTM                    | 0.966113   | 0.000786 | 0.021961 |
| 8    | CatBoost                  | 0.964419   | 0.000824 | 0.018466 |
| 9    | kNN                       | 0.959956   | 0.000928 | 0.019694 |
| 10   | XGBoost                   | 0.959611   | 0.000936 | 0.020182 |
| 11   | DecisionTrees             | 0.954863   | 0.001046 | 0.021514 |
| 12   | RNN (LSTM)                | 0.957077   | 0.000995 | 0.025647 |
| 13   | SARIMAX                   | 0.951089   | 0.001142 | 0.024786 |
| 14   | TCN                       | 0.951728   | 0.001119 | 0.023316 |
| 15   | LightGBM                  | 0.868901   | 0.003038 | 0.030866 |
| 16   | Prophet                   | 0.690026   | 0.007183 | 0.060024 |
| 17   | WaveNet                   | -9.177553  | 0.235838 | 0.461260 |
| 18   | TransformerModels         | -26.300486 | 0.632617 | 0.639855 |

### Low Price Performance Table:
| Rank | Model Name                | R-squared  | MSE      | MAE      |
| ---- | ------------------------- | ---------- | -------- | -------- |
| 1    | SVR                       | 0.982703   | 0.000389 | 0.014369 |
| 2    | ARIMA                     | 0.981903   | 0.000403 | 0.014740 |
| 3    | GradientBoostingRegressor | 0.967999   | 0.000720 | 0.019884 |
| 4    | RandomForest              | 0.965523   | 0.000776 | 0.019954 |
| 5    | LinearRegression          | 0.959793   | 0.000905 | 0.022805 |
| 6    | CatBoost                  | 0.959445   | 0.000913 | 0.020976 |
| 7    | XGBoost                   | 0.953742   | 0.001041 | 0.022499 |
| 8    | GRU                       | 0.952503   | 0.001058 | 0.024503 |
| 9    | DecisionTrees             | 0.952946   | 0.001059 | 0.023558 |
| 10   | BiLSTM                    | 0.951211   | 0.001086 | 0.024556 |
| 11   | RNN (LSTM)                | 0.951184   | 0.001087 | 0.025655 |
| 12   | TCN                       | 0.949506   | 0.001136 | 0.026067 |
| 13   | kNN                       | 0.937486   | 0.001407 | 0.024773 |
| 14   | SARIMAX                   | 0.937705   | 0.001456 | 0.030064 |
| 15   | LightGBM                  | 0.858588   | 0.003182 | 0.032838 |
| 16   | Prophet                   | 0.663988   | 0.007561 | 0.062514 |
| 17   | WaveNet                   | -9.168884  | 0.228828 | 0.454339 |
| 18   | TransformerModels         | -28.978269 | 0.674595 | 0.678098 |

### Close Price Performance Table:

| Rank | Model Name                | R-squared  | MSE      | MAE      |
| ---- | ------------------------- | ---------- | -------- | -------- |
| 1    | SVR                       | 0.982291   | 0.000416 | 0.014585 |
| 2    | ARIMA                     | 0.981666   | 0.000426 | 0.014705 |
| 3    | GradientBoostingRegressor | 0.965622   | 0.000807 | 0.020829 |
| 4    | LinearRegression          | 0.964429   | 0.000835 | 0.021419 |
| 5    | RandomForest              | 0.964356   | 0.000837 | 0.021035 |
| 6    | BiLSTM                    | 0.960092   | 0.000933 | 0.023936 |
| 7    | kNN                       | 0.959089   | 0.000961 | 0.021578 |
| 8    | CatBoost                  | 0.957867   | 0.000990 | 0.021501 |
| 9    | GRU                       | 0.954458   | 0.001053 | 0.025146 |
| 10   | DecisionTrees             | 0.952835   | 0.001108 | 0.023467 |
| 11   | XGBoost                   | 0.953548   | 0.001091 | 0.022610 |
| 12   | RNN (LSTM)                | 0.951181   | 0.001130 | 0.026570 |
| 13   | SARIMAX                   | 0.942124   | 0.001357 | 0.028134 |
| 14   | TCN                       | 0.944087   | 0.001313 | 0.026585 |
| 15   | LightGBM                  | 0.864790   | 0.003175 | 0.032928 |
| 16   | Prophet                   | 0.683928   | 0.007423 | 0.061775 |
| 17   | WaveNet                   | -9.149181  | 0.238355 | 0.463644 |
| 18   | TransformerModels         | -29.599286 | 0.718628 | 0.681372 |

## Notable Observations

- **Traditional Models**: SVR and ARIMA showed the best performance across all metrics.
- **Deep Learning Challenges**: Models like RNN (LSTM), GRU, and BiLSTM underperformed compared to simpler algorithms. Potential reasons include overfitting or insufficient hyperparameter tuning.
- **WaveNet and TransformerModels**: These models exhibited negative R-squared values, highlighting their unsuitability for the dataset.

## Research Links

You can use the following links to access this research:

- [Predict Price](https://predict-price.com/): This platform provides price and trend prediction using AI models. It offers detailed insights into the behavior of Bitcoin and other assets through advanced modeling techniques.

- [Magical Prediction](https://magicalprediction.com/): This site specializes in daily signals generated from multiple AI models. It focuses on providing actionable predictions and recommendations for traders.

- [Magical Analysis](https://magicalanalysis.com/): This platform delivers technical analysis-based signals and is tailored for users looking for data-driven insights for trading decisions.

## Conclusion

The experiments reveal that traditional machine learning models are highly effective for Bitcoin price prediction. Neural networks may require larger datasets or additional preprocessing to achieve competitive performance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
## Contact

For questions or contributions, please contact my.

---

Feel free to explore and contribute to this project!
