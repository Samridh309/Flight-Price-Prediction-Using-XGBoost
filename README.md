# ✈️ Flight Price Prediction Using XGBoost

This project uses machine learning techniques—specifically, the Gradient Boosting Regressor (with scikit-learn) and a user-friendly Gradio interface—to predict the price of flights based on various features such as airline, source/destination, departure/arrival time, stops, class, duration, and days left to departure.

## 🚀 Features

- **Exploratory Data Analysis (EDA):**
  - Visualizations for feature distributions, correlations, and categorical impacts on price.
  - Outlier analysis and class distribution plots.
- **Data Preprocessing:**
  - Label encoding for categorical variables.
  - Feature scaling for numerical columns.
- **Model Building:**
  - Gradient Boosting Regressor for robust regression.
  - Model evaluation using R², MAE, RMSE, and feature importances.
- **Interactive Web App:**
  - Gradio-powered GUI for flight price predictions, allowing easy user input and instant results.

## 🗃️ Dataset

- The dataset (`flight price prediction.csv`) contains 300,153 flight records, with features:
  - `airline`, `source_city`, `departure_time`, `stops`, `arrival_time`, `destination_city`, `class`, `duration`, `days_left`, `price`
- **Note:** The dataset is not included in this repo for size/licensing reasons. Please provide your own or obtain from a suitable source.

## 🏗️ Project Structure

```
.
├── FLIGHT_PRICE_PREDICTION.ipynb
├── requirements.txt
└── README.md
```

- **FLIGHT_PRICE_PREDICTION.ipynb:** Main Jupyter notebook containing all code for preprocessing, EDA, model training, and Gradio app.
- **requirements.txt:** All dependencies required to run the notebook and the Gradio app.
- **README.md:** This file.

## 📊 How it Works

1. **Data Loading:**  
   Upload the CSV file through the notebook (using Colab's `files.upload()`).

2. **Preprocessing:**
   - Remove unnecessary columns.
   - Encode categorical features using LabelEncoder.
   - Scale numerical features (`duration`, `days_left`).

3. **Exploratory Analysis:**  
   Visualize feature distributions, relationships, and correlations to understand data patterns.

4. **Model Training:**
   - Split data into train/test sets.
   - Train a Gradient Boosting Regressor.
   - Evaluate with R², MAE, MSE, RMSE.

5. **Feature Importance:**  
   Plot and analyze which features are most influential in price prediction.

6. **Interactive Gradio App:**  
   Users can select flight details via dropdowns and sliders to get instant price predictions.
   

## 🧩 Requirements

- Python 3.7+
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- gradio

## 📈 Model Performance

- **R² Score:** ~0.975
- **MAE:** ~₹2042.42
- **RMSE:** ~₹3582.32

*(Values above based on sample dataset. Actual results may vary depending on your data.)*

## 📋 Acknowledgements

- Dataset: [Kaggle]
- Libraries: scikit-learn, pandas, seaborn, matplotlib, gradio

## 🤝 Contributing

Pull requests and suggestions are welcome! Please open an issue to discuss changes or improvements.


**Author:** [Samridh309](https://github.com/Samridh309)
