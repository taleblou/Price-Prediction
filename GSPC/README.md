
# GSPC (S&P 500 Index) Prediction with Artificial Intelligence

## Overview

This project compares various machine learning and statistical models for predicting the S&P 500 index (GSPC). Performance is evaluated across key price metrics: Close, Open, High, and Low.

## Objectives

- Identify the most effective models for GSPC price prediction.
- Evaluate model performance using well-defined metrics.

## Metrics

The models are ranked based on:

1. **R-squared**: Higher values indicate a better fit.
2. **Mean Squared Error (MSE)**: Lower values indicate better accuracy.
3. **Mean Absolute Error (MAE)**: Lower values indicate better performance.

## Ranking Criteria

The ranking prioritizes:

- Primary: R-squared (higher is better)
- Secondary: MSE (lower is better)
- Tertiary: MAE (lower is better)

## Model Performance Tables

### Close Price Predictions

| Rank | Model Name                | R-squared | MSE      | MAE    | MedAE  |
| ---- | ------------------------- | --------- | -------- | ------ | ------ |
| 1    | SVR                       | 0.9790    | 0.000292 | 0.0126 | 0.0092 |
| 2    | ARIMA                     | 0.9767    | 0.000324 | 0.0138 | 0.0114 |
| 3    | CatBoost                  | 0.9594    | 0.000566 | 0.0190 | 0.0155 |
| 4    | GradientBoostingRegressor | 0.9580    | 0.000585 | 0.0185 | 0.0150 |
| 5    | RandomForest              | 0.9563    | 0.000609 | 0.0196 | 0.0157 |
| 6    | LinearRegression          | 0.9562    | 0.000610 | 0.0184 | 0.0141 |
| 7    | kNN                       | 0.9559    | 0.000615 | 0.0203 | 0.0185 |
| 8    | DecisionTrees             | 0.9538    | 0.000645 | 0.0195 | 0.0156 |
| 9    | XGBoost                   | 0.9547    | 0.000631 | 0.0202 | 0.0169 |
| 10   | GRU                       | 0.9335    | 0.000926 | 0.0234 | 0.0193 |
| 11   | SARIMA                    | 0.9328    | 0.000937 | 0.0232 | 0.0177 |
| 12   | LightGBM                  | 0.9042    | 0.001335 | 0.0315 | 0.0303 |
| 13   | TCN                       | 0.8919    | 0.001506 | 0.0338 | 0.0315 |
| 14   | BiLSTM                    | 0.8129    | 0.002609 | 0.0413 | 0.0397 |
| 15   | Prophet                   | 0.7616    | 0.003324 | 0.0463 | 0.0416 |
| 16   | RNN(LSTM)                 | 0.4478    | 0.007697 | 0.0748 | 0.0657 |
| 17   | WaveNet                   | -29.43    | 0.4241   | 0.6407 | 0.6344 |
| 18   | TransformerModels         | -78.76    | 1.1118   | 0.9151 | 0.8672 |

### **![][image1]**

### Open Price Predictions

| Rank | Model Name                | R-squared | MSE      | MAE    | MedAE  |
| ---- | ------------------------- | --------- | -------- | ------ | ------ |
| 1    | SVR                       | 0.9796    | 0.000270 | 0.0118 | 0.0087 |
| 2    | ARIMA                     | 0.9776    | 0.000298 | 0.0132 | 0.0109 |
| 3    | GradientBoostingRegressor | 0.9621    | 0.000503 | 0.0168 | 0.0130 |
| 4    | LinearRegression          | 0.9552    | 0.000594 | 0.0175 | 0.0143 |
| 5    | RandomForest              | 0.9612    | 0.000515 | 0.0175 | 0.0136 |
| 6    | XGBoost                   | 0.9615    | 0.000511 | 0.0178 | 0.0153 |
| 7    | kNN                       | 0.9630    | 0.000491 | 0.0171 | 0.0149 |
| 8    | DecisionTrees             | 0.9575    | 0.000564 | 0.0186 | 0.0169 |
| 9    | GRU                       | 0.9506    | 0.000656 | 0.0189 | 0.0139 |
| 10   | LightGBM                  | 0.9039    | 0.001276 | 0.0305 | 0.0306 |
| 11   | TCN                       | 0.9167    | 0.001106 | 0.0299 | 0.0304 |
| 12   | BiLSTM                    | 0.7650    | 0.003118 | 0.0465 | 0.0410 |
| 13   | Prophet                   | 0.7597    | 0.003189 | 0.0452 | 0.0408 |
| 14   | SARIMA                    | 0.9350    | 0.000862 | 0.0217 | 0.0173 |
| 15   | RNN(LSTM)                 | 0.3529    | 0.008586 | 0.0810 | 0.0765 |
| 16   | WaveNet                   | -31.43    | 0.4303   | 0.6460 | 0.6400 |
| 17   | TransformerModels         | -67.57    | 0.9098   | 0.8103 | 0.7579 |

### **![][image2]**

### High Price Predictions

| Rank | Model Name                | R-squared | MSE      | MAE    | MedAE  |
| ---- | ------------------------- | --------- | -------- | ------ | ------ |
| 1    | SVR                       | 0.9851    | 0.000207 | 0.0100 | 0.0071 |
| 2    | ARIMA                     | 0.9835    | 0.000230 | 0.0112 | 0.0085 |
| 3    | kNN                       | 0.9711    | 0.000402 | 0.0154 | 0.0125 |
| 4    | XGBoost                   | 0.9682    | 0.000443 | 0.0168 | 0.0138 |
| 5    | CatBoost                  | 0.9695    | 0.000425 | 0.0158 | 0.0126 |
| 6    | GradientBoostingRegressor | 0.9716    | 0.000396 | 0.0141 | 0.0104 |
| 7    | RandomForest              | 0.9701    | 0.000417 | 0.0156 | 0.0126 |
| 8    | DecisionTrees             | 0.9663    | 0.000469 | 0.0166 | 0.0140 |
| 9    | LinearRegression          | 0.9653    | 0.000483 | 0.0158 | 0.0121 |
| 10   | GRU                       | 0.9532    | 0.000652 | 0.0193 | 0.0166 |
| 11   | LightGBM                  | 0.9103    | 0.001249 | 0.0301 | 0.0282 |
| 12   | TCN                       | 0.9002    | 0.001390 | 0.0332 | 0.0332 |
| 13   | BiLSTM                    | 0.7889    | 0.002940 | 0.0463 | 0.0439 |
| 14   | Prophet                   | 0.7863    | 0.002978 | 0.0439 | 0.0432 |
| 15   | SARIMA                    | 0.9469    | 0.000740 | 0.0199 | 0.0157 |
| 16   | RNN(LSTM)                 | 0.4156    | 0.008142 | 0.0780 | 0.0715 |
| 17   | WaveNet                   | -29.78    | 0.4288   | 0.6444 | 0.6444 |
| 18   | TransformerModels         | -65.31    | 0.9237   | 0.8222 | 0.7695 |

### **![][image3]**

### Low Price Predictions

| Rank | Model Name                | R-squared | MSE      | MAE    | MedAE  |
| ---- | ------------------------- | --------- | -------- | ------ | ------ |
| 1    | SVR                       | 0.9810    | 0.000252 | 0.0114 | 0.0084 |
| 2    | ARIMA                     | 0.9792    | 0.000276 | 0.0125 | 0.0096 |
| 3    | kNN                       | 0.9653    | 0.000460 | 0.0166 | 0.0126 |
| 4    | CatBoost                  | 0.9645    | 0.000471 | 0.0170 | 0.0148 |
| 5    | GradientBoostingRegressor | 0.9651    | 0.000462 | 0.0163 | 0.0130 |
| 6    | RandomForest              | 0.9663    | 0.000447 | 0.0162 | 0.0140 |
| 7    | XGBoost                   | 0.9623    | 0.000499 | 0.0176 | 0.0154 |
| 8    | DecisionTrees             | 0.9601    | 0.000529 | 0.0179 | 0.0133 |
| 9    | LinearRegression          | 0.9559    | 0.000585 | 0.0178 | 0.0136 |
| 10   | GRU                       | 0.9493    | 0.000673 | 0.0199 | 0.0167 |
| 11   | LightGBM                  | 0.9069    | 0.001235 | 0.0296 | 0.0279 |
| 12   | TCN                       | 0.9110    | 0.001180 | 0.0299 | 0.0303 |
| 13   | BiLSTM                    | 0.8005    | 0.002646 | 0.0422 | 0.0375 |
| 14   | Prophet                   | 0.7439    | 0.003396 | 0.0473 | 0.0411 |
| 15   | SARIMA                    | 0.9328    | 0.000891 | 0.0222 | 0.0174 |
| 16   | RNN(LSTM)                 | 0.3936    | 0.008043 | 0.0776 | 0.0724 |
| 17   | WaveNet                   | -30.97    | 0.4240   | 0.6411 | 0.6329 |
| 18   | TransformerModels         | -73.82    | 0.9922   | 0.8660 | 0.8785 |

### **![][image4]**

## Findings

- **Top Performers**: SVR and ARIMA dominate across all price categories.
- **Ensemble Methods**: CatBoost, GradientBoostingRegressor, and RandomForest show consistent results.
- **Neural Networks**: Models like GRU and BiLSTM underperform compared to simpler models.
- **Poor Performers**: WaveNet and TransformerModels exhibit poor fit, likely due to overfitting or data inadequacy.

## Observations

- Simpler models like SVR and ARIMA outperform complex models in this dataset.
- Traditional machine learning methods are robust and effective for GSPC prediction.
- Neural network models require further optimization or larger datasets to compete effectively.

## Conclusion

- **Best Models**: SVR and ARIMA are recommended for GSPC prediction tasks due to their balance of accuracy and interpretability. These models excel at capturing essential patterns in structured financial data, making them suitable for robust forecasting tasks across various market conditions.

- **Practical Use**: Ensemble methods also provide reliable performance for structured data. Their ability to combine predictions from multiple learners enhances accuracy and stability, making them a strong choice for scenarios requiring balanced trade-offs between complexity and interpretability.

- **Insights for Neural Networks**: While neural networks like GRU and BiLSTM offer the potential for complex pattern recognition, their underperformance in this study highlights the importance of dataset size and feature richness. Future efforts could explore hybrid models or optimized preprocessing techniques to leverage their strengths.

- **General Observations**: This analysis underscores the effectiveness of traditional and ensemble methods in financial prediction tasks. However, the evolving nature of market dynamics may require adaptive techniques in future implementations.

- **Final Recommendations**: For practical applications, prioritize SVR and ARIMA for their proven reliability. Consider ensemble methods for added robustness, and cautiously explore neural networks when sufficient computational resources and data are available.

## Recommendations

- Use SVR or ARIMA for accurate and interpretable results.
- Avoid complex neural networks unless data volume and quality can support their use.

## Code Access

The code for all the models used in this project is available on my GitHub repository: [GitHub - taleblou](https://github.com/taleblou). You are free to use it for your own projects.

## Research Access

You can access this research through the following links:

1. [Predict-Price](https://predict-price.com/): This platform focuses on price and trend prediction using advanced AI models. It provides actionable insights for financial forecasting.

2. [MagicalPrediction](https://magicalprediction.com/): This site offers daily predictions and signals derived from a variety of AI models, tailored for accurate market analysis.

3. [MagicalAnalysis](https://magicalanalysis.com/): A resource for daily technical analysis-based signals, designed for traders and analysts seeking data-driven insights.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or contributions, please contact my.

---

Feel free to explore and contribute to this project!



[image1]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/GSPC/^GSPC_Close.png>
[image2]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/GSPC/^GSPC_Open.png>
[image3]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/GSPC/^GSPC_High.png>
[image4]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/GSPC/^GSPC_Low.png>
