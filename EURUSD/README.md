# EUR/USD Price Prediction with AI Models

This repository contains experiments and analyses for predicting EUR/USD exchange rates using various machine learning and deep learning models. The models were evaluated based on their performance across different price categories: Close Price, Open Price, High Price, and Low Price.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Models and Performance](#models-and-performance)
  - [Close Price Rankings](#close-price-rankings)
  - [Open Price Rankings](#open-price-rankings)
  - [High Price Rankings](#high-price-rankings)
  - [Low Price Rankings](#low-price-rankings)
- [Key Observations](#key-observations)
- [Insights on Model Selection](#insights-on-model-selection)
- [Conclusions](#conclusions)
- [Code Availability](#code-availability)
- [Research Links](#research-links)
- [License](#license)

## Introduction

The EUR/USD price prediction experiments leverage a variety of AI models to evaluate their performance in financial time-series forecasting. Each model was ranked based on metrics like R-squared, Explained Variance Score, Mean Squared Error (MSE), Mean Absolute Error (MAE), and Median Absolute Error.

## Features

- Comprehensive comparison of traditional, ensemble, and deep learning models.
- Performance evaluation based on standard metrics.
- Insights into model selection and applicability.

## Models and Performance

### Close Price Rankings

| Rank | Model                          | R-squared    | Explained Variance | MSE       | MAE       | Median AE |
|------|--------------------------------|--------------|---------------------|-----------|-----------|-----------|
| 1    | SVR                            | 0.946075     | 0.946134           | 0.000235  | 0.011589  | 0.009070  |
| 2    | ARIMA                          | 0.945953     | 0.946397           | 0.000237  | 0.011679  | 0.009444  |
| 3    | LightGBM                       | 0.939505     | 0.939578           | 0.000264  | 0.012237  | 0.009752  |
| 4    | CatBoost                       | 0.932746     | 0.932751           | 0.000294  | 0.013217  | 0.011689  |
| 5    | XGBoost                        | 0.927137     | 0.927145           | 0.000318  | 0.013970  | 0.011840  |
| 6    | kNN                            | 0.920658     | 0.920669           | 0.000346  | 0.014811  | 0.012976  |
| 7    | DecisionTrees                  | 0.918371     | 0.918371           | 0.000356  | 0.014874  | 0.012940  |
| 8    | GRU                            | 0.917511     | 0.919271           | 0.000361  | 0.015417  | 0.013425  |
| 9    | RandomForest                   | 0.916809     | 0.916818           | 0.000363  | 0.015297  | 0.013383  |
| 10   | GradientBoostingRegressor      | 0.909607     | 0.909617           | 0.000395  | 0.015453  | 0.012661  |
| 11   | TCN                            | 0.910679     | 0.930858           | 0.000390  | 0.016029  | 0.014090  |
| 12   | BiLSTM                         | 0.904495     | 0.914171           | 0.000418  | 0.016439  | 0.014528  |
| 13   | LinearRegression               | 0.901652     | 0.901998           | 0.000429  | 0.016308  | 0.013370  |
| 14   | RNN (LSTM)                     | 0.883763     | 0.910523           | 0.000508  | 0.018262  | 0.016347  |
| 15   | SARIMA                         | 0.848969     | 0.849753           | 0.000659  | 0.020674  | 0.017393  |
| 16   | Prophet                        | -0.698721    | -0.689790          | 0.007415  | 0.067379  | 0.053078  |
| 17   | WaveNet                        | -25.629528   | 0.001559           | 0.116231  | 0.334475  | 0.334090  |
| 18   | TransformerModels              | -128.661550  | -90.436551         | 0.565941  | 0.614295  | 0.533799  |

### **![][image1]**

### Open Price Rankings

| Rank | Model                          | R-squared    | Explained Variance | MSE       | MAE       | Median AE |
|------|--------------------------------|--------------|---------------------|-----------|-----------|-----------|
| 1    | SVR                            | 0.946049     | 0.946114           | 0.000236  | 0.011585  | 0.008941  |
| 2    | ARIMA                          | 0.945922     | 0.946333           | 0.000236  | 0.011632  | 0.009446  |
| 3    | LightGBM                       | 0.938993     | 0.939073           | 0.000266  | 0.012262  | 0.010031  |
| 4    | CatBoost                       | 0.929664     | 0.929665           | 0.000307  | 0.013398  | 0.011823  |
| 5    | XGBoost                        | 0.926474     | 0.926474           | 0.000321  | 0.013996  | 0.011874  |
| 6    | kNN                            | 0.919249     | 0.919251           | 0.000352  | 0.014968  | 0.012549  |
| 7    | TCN                            | 0.915623     | 0.934363           | 0.000368  | 0.015723  | 0.014479  |
| 8    | BiLSTM                         | 0.915364     | 0.923028           | 0.000370  | 0.015693  | 0.013056  |
| 9    | DecisionTrees                  | 0.912335     | 0.912337           | 0.000383  | 0.015029  | 0.011832  |
| 10   | RandomForest                   | 0.911198     | 0.911205           | 0.000388  | 0.015650  | 0.013933  |
| 11   | GRU                            | 0.910611     | 0.911327           | 0.000390  | 0.015814  | 0.013136  |
| 12   | GradientBoostingRegressor      | 0.907235     | 0.907245           | 0.000405  | 0.015565  | 0.011745  |
| 13   | LinearRegression               | 0.901635     | 0.901981           | 0.000429  | 0.016311  | 0.013496  |
| 14   | RNN (LSTM)                     | 0.893254     | 0.921960           | 0.000466  | 0.018006  | 0.015022  |
| 15   | SARIMA                         | 0.848909     | 0.849704           | 0.000660  | 0.020689  | 0.017423  |
| 16   | Prophet                        | -0.694535    | -0.685336          | 0.007397  | 0.067236  | 0.051149  |
| 17   | WaveNet                        | -25.631627   | 0.001641           | 0.116253  | 0.334508  | 0.334199  |
| 18   | TransformerModels              | -131.743529  | -72.823062         | 0.579457  | 0.620594  | 0.545330  |

### **![][image2]**

### High Price Rankings

| Rank | Model                          | R-squared    | Explained Variance | MSE       | MAE       | Median AE |
|------|--------------------------------|--------------|---------------------|-----------|-----------|-----------|
| 1    | SVR                            | 0.959489     | 0.959512           | 0.000181  | 0.010111  | 0.007861  |
| 2    | ARIMA                          | 0.959062     | 0.959468           | 0.000183  | 0.010192  | 0.007829  |
| 3    | LightGBM                       | 0.949926     | 0.950073           | 0.000223  | 0.011605  | 0.008568  |
| 4    | CatBoost                       | 0.944750     | 0.944758           | 0.000246  | 0.012497  | 0.010473  |
| 5    | GradientBoostingRegressor      | 0.942026     | 0.942238           | 0.000258  | 0.012385  | 0.009225  |
| 6    | XGBoost                        | 0.943209     | 0.943210           | 0.000253  | 0.012465  | 0.010745  |
| 7    | kNN                            | 0.940613     | 0.940640           | 0.000265  | 0.012799  | 0.010143  |
| 8    | DecisionTrees                  | 0.917961     | 0.918388           | 0.000366  | 0.014580  | 0.011363  |
| 9    | RandomForest                   | 0.924833     | 0.925059           | 0.000335  | 0.014260  | 0.011217  |
| 10   | BiLSTM                         | 0.898991     | 0.900377           | 0.000450  | 0.017080  | 0.015400  |
| 11   | GRU                            | 0.890233     | 0.891076           | 0.000489  | 0.017931  | 0.015867  |
| 12   | RNN (LSTM)                     | 0.891732     | 0.901317           | 0.000483  | 0.017590  | 0.014340  |
| 13   | TCN                            | 0.893906     | 0.911409           | 0.000473  | 0.016881  | 0.012803  |
| 14   | LinearRegression               | 0.908595     | 0.908947           | 0.000408  | 0.015578  | 0.012854  |
| 15   | SARIMA                         | 0.861903     | 0.862627           | 0.000616  | 0.019420  | 0.015522  |
| 16   | Prophet                        | -0.729126    | -0.718021          | 0.007710  | 0.068955  | 0.053528  |
| 17   | WaveNet                        | -23.849821   | 0.001260           | 0.110800  | 0.326108  | 0.327909  |
| 18   | TransformerModels              | -131.849641  | -77.544845         | 0.592346  | 0.620903  | 0.525489  |

### **![][image3]**

### Low Price Rankings

| Rank | Model                          | R-squared    | Explained Variance | MSE       | MAE       | Median AE |
|------|--------------------------------|--------------|---------------------|-----------|-----------|-----------|
| 1    | SVR                            | 0.959489     | 0.959512           | 0.000181  | 0.010111  | 0.007861  |
| 2    | ARIMA                          | 0.959062     | 0.959468           | 0.000183  | 0.010192  | 0.007829  |
| 3    | LightGBM                       | 0.949926     | 0.950073           | 0.000223  | 0.011605  | 0.008568  |
| 4    | CatBoost                       | 0.944750     | 0.944758           | 0.000246  | 0.012497  | 0.010473  |
| 5    | GradientBoostingRegressor      | 0.942026     | 0.942238           | 0.000258  | 0.012385  | 0.009225  |
| 6    | XGBoost                        | 0.943209     | 0.943210           | 0.000253  | 0.012465  | 0.010745  |
| 7    | kNN                            | 0.940613     | 0.940640           | 0.000265  | 0.012799  | 0.010143  |
| 8    | DecisionTrees                  | 0.917961     | 0.918388           | 0.000366  | 0.014580  | 0.011363  |
| 9    | RandomForest                   | 0.924833     | 0.925059           | 0.000335  | 0.014260  | 0.011217  |
| 10   | BiLSTM                         | 0.898991     | 0.900377           | 0.000450  | 0.017080  | 0.015400  |
| 11   | GRU                            | 0.890233     | 0.891076           | 0.000489  | 0.017931  | 0.015867  |
| 12   | RNN (LSTM)                     | 0.891732     | 0.901317           | 0.000483  | 0.017590  | 0.014340  |
| 13   | TCN                            | 0.893906     | 0.911409           | 0.000473  | 0.016881  | 0.012803  |
| 14   | LinearRegression               | 0.908595     | 0.908947           | 0.000408  | 0.015578  | 0.012854  |
| 15   | SARIMA                         | 0.861903     | 0.862627           | 0.000616  | 0.019420  | 0.015522  |
| 16   | Prophet                        | -0.729126    | -0.718021          | 0.007710  | 0.068955  | 0.053528  |
| 17   | WaveNet                        | -23.849821   | 0.001260           | 0.110800  | 0.326108  | 0.327909  |
| 18   | TransformerModels              | -131.849641  | -77.544845         | 0.592346  | 0.620903  | 0.525489  |

### **![][image4]**

## Key Observations

- **Top Performers:** SVR and ARIMA consistently demonstrate strong predictive capabilities.
- **Underperformers:** TransformerModels and WaveNet struggle with large negative R-squared values and high errors.
- **Ensemble Models:** LightGBM and CatBoost perform well, offering a balance between accuracy and computational cost.

## Insights on Model Selection

- **Support Vector Regression (SVR):** A reliable choice for EUR/USD prediction due to consistent performance.
- **ARIMA:** Highly effective for time-series data.
- **Ensemble Models:** Provide competitive performance with added interpretability.
- **Deep Learning Models:** Show potential but require optimization for this data type.
- **Linear Models:** Perform decently but lag behind advanced approaches.

## Conclusions

- **Recommended Models:** SVR and ARIMA emerge as top choices for EUR/USD prediction tasks due to their high predictive accuracy and robust performance across multiple evaluation metrics. These models are particularly suitable for financial time-series predictions where precision is critical.

- **Deep Learning Challenges:** While deep learning models such as TransformerModels and WaveNet hold potential in other domains, their performance in this application highlights the importance of data-specific optimization. Issues like overfitting and excessive complexity need to be addressed for better results.

- **Hybrid Approaches:** Future research can explore hybrid models that combine traditional methods like ARIMA with machine learning models to leverage the strengths of both approaches. This could improve performance on challenging datasets.

- **Tailored Model Selection:** Each model has its strengths and weaknesses, and selection should be based on specific use cases, resource availability, and computational efficiency.

## Code Availability

The complete implementation code for all models is available on my [GitHub](https://github.com/taleblou). Feel free to use it for your projects and experiments.

## Research Links

You can use the following links to access additional research and related tools:

- [Predict Price](https://predict-price.com/): Provides price and trend predictions using advanced AI models tailored for financial applications.
- [Magical Prediction](https://magicalprediction.com/): Offers daily trading signals based on AI-driven models.
- [Magical Analysis](https://magicalanalysis.com/): Delivers daily trading signals derived from in-depth technical analysis.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute the code as long as proper attribution is given.

## Contact

For questions or contributions, please contact my.

---

Feel free to explore and contribute to this project!



[image1]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/EURUSD/EURUSD=X_Close.png>
[image2]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/EURUSD/EURUSD=X_Open.png>
[image3]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/EURUSD/EURUSD=X_High.png>
[image4]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/refs/heads/main/EURUSD/EURUSD=X_Low.png>
