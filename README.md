# Implementation Practice of Kaggle M5 Forecasting
> Task source: [Kaggle M5 Forecasting Accuracy](https://www.kaggle.com/c/m5-forecasting-accuracy)

## Project Overview
This repository contains implementations and experiments for the Kaggle M5 Forecasting competition. The goal is to predict sales for Walmart products using various machine learning and deep learning techniques.

## File Explanation
1. `m5-forecast-with-lgbm_yuga.ipynb`: Tree-based method using LightGBM (LGBM).
   - Preprocesses the dataset, including handling missing values and encoding categorical variables.
   - Performs feature engineering, such as creating lag features and rolling statistics.
   - Trains a LightGBM model and evaluates its performance using metrics like RMSE.

2. `m5-forecast-with-simple-lstm_yuga.ipynb`: Neural network method using a simple LSTM architecture.
   - Prepares time-series data by normalizing and reshaping it for input into the LSTM model.
   - Defines and trains a simple LSTM model for sales forecasting.
   - Visualizes the model's predictions and compares them with actual sales data.

3. `M5-Forecasting-EDA_yuga.ipynb`: Basic exploratory data analysis (EDA) to understand the dataset.
   - Analyzes sales trends over time and across different categories.
   - Visualizes data distributions and relationships using plots (e.g., histograms, line plots).
   - Identifies potential challenges, such as seasonality and sparsity in the data.

## Conclusion and Insights
The Kaggle M5 Forecasting competition provided a valuable opportunity to explore and compare different forecasting techniques. Key takeaways include:
- **Feature Engineering Matters**: Creating lag features and rolling statistics significantly improved the performance of the LightGBM model.
- **Neural Networks for Time-Series**: While the LSTM model captured temporal patterns, its performance was sensitive to data preprocessing and hyperparameter tuning.
- **EDA is Crucial**: Understanding the dataset through exploratory data analysis helped identify challenges like seasonality and sparsity, guiding the choice of modeling techniques.
- **Hybrid Approaches**: Combining tree-based methods with neural networks could leverage the strengths of both approaches for better accuracy.

These insights will inform future work, including the application of advanced techniques like Attention mechanisms and hybrid modeling strategies.

## Future Work
1. Apply an Attention mechanism to neural networks to improve forecasting accuracy.
2. Explore and implement additional feature engineering techniques to enhance model performance.
3. Experiment with hybrid models combining tree-based methods and neural networks.
4. Evaluate the impact of hyperparameter tuning on model performance.