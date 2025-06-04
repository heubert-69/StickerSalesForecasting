Sticker Sales Forecasting
This project focuses on forecasting sticker sales across different countries, stores, and product types using historical sales data. It was developed as part of a Kaggle competition and employs time series machine learning techniques to predict future sales.

Project Overview
The goal is to accurately predict sticker sales by leveraging various time-based, economic, and categorical features. The model built here is a Ridge Regression pipeline optimized via hyperparameter tuning.

Features
Time-based features:

Lag variables capturing past sales data

Rolling averages and expanding means to smooth trends

Sales momentum indicators

Holiday detection:

Utilizes the holidays Python library to mark special dates by country, accounting for holiday effects on sales

Economic context:

Incorporates economic indicators such as GDP, inflation, unemployment, and interest rates sourced from the World Bank to provide macroeconomic insights

Cyclical encoding:

Applies sine and cosine transformations to encode cyclical patterns in months and weekdays, helping the model understand periodicity

Categorical encoding:

Uses label encoding and creates combination features (e.g., country_product) to capture interaction effects

Model
Algorithm: Ridge Regression

Preprocessing: Implemented through a scikit-learn pipeline, ensuring clean and reproducible feature transformations

Optimization: Hyperparameter tuning performed with GridSearchCV to find the best model parameters

Output
The model generates sales predictions formatted according to Kaggle’s required submission.csv for evaluation.

Getting Started
Prerequisites
Python 3.x

Libraries: pandas, numpy, scikit-learn, holidays, matplotlib (optional for visualization)

You can install the required packages with:
```bash
pip install pandas numpy scikit-learn holidays matplotlib
```

Running the Project
1. Clone the repo:
```bash
git clone https://github.com/heubert-69/StickerSalesForecasting.git
cd StickerSalesForecasting
```

2. Prepare your dataset following the Kaggle competition instructions.

3. Run the main script (replace with your actual script name):
```bash
python main.py
```

License
This project is licensed under the MIT License.
