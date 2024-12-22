# **Gold Price Prediction using Machine Learning and Statistical Models**

This repository contains experiments and analyses for predicting gold prices using various machine learning and statistical models. The performance of each model has been evaluated across four price categories: **Close Price**, **Open Price**, **High Price**, and **Low Price**, using metrics such as R-squared, Explained Variance Score, Mean Squared Error (MSE), Mean Absolute Error (MAE), and Median Absolute Error (MedAE).

## **Overview**

The analysis compares the performance of 18 models, ranging from traditional statistical models (e.g., ARIMA, SARIMA) to machine learning methods (e.g., SVR, Gradient Boosting) and neural network architectures (e.g., GRU, BiLSTM).

## **Models Analyzed**

* **Statistical Models**: ARIMA, SARIMA  
* **Machine Learning Models**: Support Vector Regression (SVR), Random Forest, Gradient Boosting (CatBoost, XGBoost), k-Nearest Neighbors (kNN)  
* **Neural Networks**: GRU, BiLSTM, Transformer Models, WaveNet  
* **Hybrid/Other Models**: Prophet, TCN

## **Ranking Criteria**

Models are ranked based on the following metrics:

1. **R-squared** (higher is better)  
2. **Explained Variance Score** (higher is better)  
3. **Mean Squared Error (MSE)** (lower is better)  
4. **Mean Absolute Error (MAE)** (lower is better)  
5. **Median Absolute Error (MedAE)** (lower is better)

## **Key Findings**

### **Best Performers**

* **Close Price**: ARIMA (0.974851 R-squared), SVR (0.976642 R-squared)  
* **Open Price**: SVR (0.978980 R-squared), ARIMA (0.976893 R-squared)  
* **High Price**: SVR (0.981728 R-squared), ARIMA (0.979900 R-squared)  
* **Low Price**: ARIMA (0.979164 R-squared), SVR (0.980899 R-squared)

### **Observations**

* Statistical models like **ARIMA** excel in time-series predictions.  
* **SVR** is the most consistent among machine learning models.  
* Neural networks underperform compared to simpler models, highlighting the need for task-specific tuning.

## **Tables of Model Performance**

### **Close Price**

| Rank | Model | R-squared | Explained Variance | MSE | MAE | MedAE |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | ARIMA | 0.974851 | 0.977691 | 0.000496 | 0.018047 | 0.015874 |
| 2 | SVR | 0.976642 | 0.976703 | 0.000460 | 0.016052 | 0.013009 |
| 3 | LinearRegression | 0.956899 | 0.957550 | 0.000849 | 0.023148 | 0.020328 |
| 4 | CatBoost | 0.956492 | 0.961351 | 0.000857 | 0.022946 | 0.018310 |
| 5 | GradientBoostingRegressor | 0.955353 | 0.958979 | 0.000879 | 0.022884 | 0.017424 |
| 6 | XGBoost | 0.950820 | 0.958656 | 0.000968 | 0.024699 | 0.019063 |
| 7 | RandomForest | 0.948139 | 0.956120 | 0.001021 | 0.025027 | 0.021902 |
| 8 | DecisionTrees | 0.947277 | 0.951722 | 0.001038 | 0.025632 | 0.021270 |
| 9 | GRU | 0.946930 | 0.951302 | 0.001046 | 0.026183 | 0.022244 |
| 10 | kNN | 0.943190 | 0.951556 | 0.001119 | 0.026116 | 0.022467 |
| 11 | SARIMA | 0.939977 | 0.941410 | 0.001182 | 0.027761 | 0.024155 |
| 12 | TCN | 0.930320 | 0.965090 | 0.001372 | 0.031242 | 0.030047 |
| 13 | BiLSTM | 0.853745 | 0.921510 | 0.002884 | 0.042023 | 0.033127 |
| 14 | LightGBM | 0.855436 | 0.906360 | 0.002847 | 0.042387 | 0.033170 |
| 15 | Prophet | 0.685251 | 0.781322 | 0.006198 | 0.068943 | 0.068640 |
| 16 | RNN(LSTM) | 0.527307 | 0.840264 | 0.009304 | 0.079385 | 0.065264 |
| 17 | TransformerModels | \-47.607737 | \-19.426501 | 0.957144 | 0.829888 | 0.760408 |
| 18 | WaveNet | \-17.643760 | 0.032877 | 0.367118 | 0.589978 | 0.556717 |

### **![][image1]**

### **Open Price**

| Rank | Model | R-squared | Explained Variance | MSE | MAE | MedAE |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | SVR | 0.978980 | 0.979054 | 0.000417 | 0.015383 | 0.011464 |
| 2 | ARIMA | 0.976893 | 0.979746 | 0.000458 | 0.016683 | 0.013496 |
| 3 | GRU | 0.966560 | 0.966770 | 0.000664 | 0.020703 | 0.017758 |
| 4 | CatBoost | 0.956237 | 0.960702 | 0.000867 | 0.023099 | 0.017451 |
| 5 | DecisionTrees | 0.956292 | 0.960043 | 0.000866 | 0.022793 | 0.017595 |
| 6 | LinearRegression | 0.957523 | 0.958210 | 0.000842 | 0.023272 | 0.018114 |
| 7 | XGBoost | 0.954154 | 0.960307 | 0.000908 | 0.023744 | 0.019351 |
| 8 | RandomForest | 0.953632 | 0.960903 | 0.000919 | 0.023913 | 0.018671 |
| 9 | TCN | 0.950812 | 0.984635 | 0.000975 | 0.027130 | 0.025609 |
| 10 | GradientBoostingRegressor | 0.933775 | 0.957777 | 0.001312 | 0.028672 | 0.024685 |
| 11 | kNN | 0.939625 | 0.950866 | 0.001196 | 0.026123 | 0.019048 |
| 12 | SARIMA | 0.938528 | 0.940161 | 0.001218 | 0.028272 | 0.027554 |
| 13 | BiLSTM | 0.816377 | 0.926231 | 0.003643 | 0.048746 | 0.039378 |
| 14 | LightGBM | 0.851762 | 0.905525 | 0.002937 | 0.042482 | 0.035013 |
| 15 | Prophet | 0.677394 | 0.780211 | 0.006392 | 0.070236 | 0.069005 |
| 16 | RNN(LSTM) | 0.476609 | 0.853575 | 0.010385 | 0.087094 | 0.079421 |
| 17 | TransformerModels | \-46.028476 | \-17.033527 | 0.931855 | 0.827136 | 0.804697 |
| 18 | WaveNet | \-17.585111 | 0.032181 | 0.368258 | 0.590831 | 0.558333 |

### **![][image1]**

### **High Price**

| Rank | Model | R-squared | Explained Variance | MSE | MAE | MedAE |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | ARIMA | 0.979900 | 0.982585 | 0.000395 | 0.015901 | 0.013434 |
| 2 | SVR | 0.981728 | 0.981757 | 0.000359 | 0.014462 | 0.012142 |
| 3 | DecisionTrees | 0.964768 | 0.966689 | 0.000692 | 0.020602 | 0.016671 |
| 4 | GradientBoostingRegressor | 0.964581 | 0.966003 | 0.000695 | 0.019956 | 0.014546 |
| 5 | RandomForest | 0.964025 | 0.966318 | 0.000706 | 0.020334 | 0.014447 |
| 6 | CatBoost | 0.959967 | 0.964683 | 0.000786 | 0.021411 | 0.014410 |
| 7 | kNN | 0.961117 | 0.964744 | 0.000763 | 0.021273 | 0.014935 |
| 8 | LinearRegression | 0.959160 | 0.959713 | 0.000802 | 0.022348 | 0.019437 |
| 9 | XGBoost | 0.955666 | 0.963837 | 0.000870 | 0.022946 | 0.016166 |
| 10 | GRU | 0.953272 | 0.953323 | 0.000919 | 0.022843 | 0.017026 |
| 11 | TCN | 0.947191 | 0.978763 | 0.001037 | 0.027370 | 0.025640 |
| 12 | SARIMA | 0.939148 | 0.940599 | 0.001195 | 0.027752 | 0.024388 |
| 13 | BiLSTM | 0.773161 | 0.916862 | 0.004461 | 0.054905 | 0.048132 |
| 14 | LightGBM | 0.849927 | 0.901709 | 0.002946 | 0.041650 | 0.033402 |
| 15 | Prophet | 0.675472 | 0.777045 | 0.006371 | 0.069837 | 0.066357 |
| 16 | RNN(LSTM) | 0.343324 | 0.812294 | 0.012913 | 0.096822 | 0.090037 |
| 17 | TransformerModels | \-38.402792 | \-16.581745 | 0.773535 | 0.742963 | 0.671446 |
| 18 | WaveNet | \-18.279980 | 0.031525 | 0.378494 | 0.599568 | 0.567255 |

### **![][image2]**

### **Low Price**

| Rank | Model | R-squared | Explained Variance | MSE | MAE | MedAE |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| 1 | ARIMA | 0.979164 | 0.981729 | 0.000415 | 0.015761 | 0.011898 |
| 2 | SVR | 0.980899 | 0.980903 | 0.000380 | 0.014096 | 0.009831 |
| 3 | CatBoost | 0.959462 | 0.963862 | 0.000807 | 0.022101 | 0.017838 |
| 4 | GradientBoostingRegressor | 0.961054 | 0.964912 | 0.000776 | 0.021332 | 0.016975 |
| 5 | LinearRegression | 0.960932 | 0.961478 | 0.000778 | 0.021926 | 0.018177 |
| 6 | DecisionTrees | 0.958237 | 0.962023 | 0.000832 | 0.022309 | 0.016886 |
| 7 | XGBoost | 0.956030 | 0.962835 | 0.000876 | 0.022929 | 0.017975 |
| 8 | RandomForest | 0.957980 | 0.963416 | 0.000837 | 0.022506 | 0.017796 |
| 9 | kNN | 0.953751 | 0.960062 | 0.000921 | 0.022730 | 0.016884 |
| 10 | GRU | 0.953421 | 0.959394 | 0.000929 | 0.024820 | 0.021201 |
| 11 | TCN | 0.939437 | 0.975727 | 0.001206 | 0.030907 | 0.030480 |
| 12 | SARIMA | 0.945075 | 0.946594 | 0.001094 | 0.026908 | 0.024031 |
| 13 | BiLSTM | 0.869943 | 0.930095 | 0.002593 | 0.038860 | 0.028439 |
| 14 | LightGBM | 0.860326 | 0.913561 | 0.002782 | 0.041315 | 0.033606 |
| 15 | Prophet | 0.685058 | 0.782527 | 0.006273 | 0.070054 | 0.069611 |
| 16 | RNN(LSTM) | 0.560358 | 0.857794 | 0.008765 | 0.077681 | 0.065039 |
| 17 | TransformerModels | \-40.146335 | \-17.551166 | 0.819503 | 0.764926 | 0.740248 |
| 18 | WaveNet | \-17.441391 | 0.031986 | 0.367293 | 0.589927 | 0.557800 |

### **![][image4]**

## **Code Availability**

All model implementation code is available in this [GitHub repository](https://github.com/taleblou) and can be freely accessed and used for non-commercial purposes. Contributions and feedback are welcome to improve the models and experiments.

## **Additional Resources**

You can use the following links to access this research and related tools:

1. [Predict Price](https://predict-price.com/):

   * This platform provides tools and insights for price and trend prediction using advanced AI models. It focuses on leveraging machine learning for precise forecasting in various financial markets.  
2. [Magical Prediction](https://magicalprediction.com/):

   * This website offers daily prediction signals generated by sophisticated AI models. The platform is tailored for traders and analysts who require actionable insights for their decision-making processes.  
3. [Magical Analysis](https://magicalanalysis.com/):

   * This service provides technical analysis signals based on historical data and proven analytical techniques. It is designed for users seeking comprehensive market evaluations supported by AI-driven analysis.

## **Conclusion**

The analysis reveals critical insights into the effectiveness of various models for predicting gold prices. Simpler models like ARIMA and SVR consistently outperform more complex machine learning and neural network architectures in terms of both accuracy and computational efficiency. This suggests that gold price data, being inherently sequential and time-series in nature, aligns well with models

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or contributions, please contact my.

---

Feel free to explore and contribute to this project!


[image1]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/Gold/refs/heads/main/Plot/GC=F_Close.png>
[image2]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/Gold/refs/heads/main/Plot/GC=F_Open.png>
[image3]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/Gold/refs/heads/main/Plot/GC=F_High.png>
[image4]: <https://raw.githubusercontent.com/taleblou/Price-Prediction/Gold/refs/heads/main/Plot/GC=F_Low.png>
