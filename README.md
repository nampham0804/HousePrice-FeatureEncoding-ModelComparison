# House Price Prediction — Impact of Feature Encoding Techniques

## 📌 Project Overview
This project analyzes factors influencing house prices and compares the impact of two feature encoding strategies on model performance:
1. **Using raw numerical variables** directly.
2. **Converting discrete-valued numerical variables** into dummy variables.

The goal is to determine which approach yields better predictive accuracy and model interpretability.

---

## 📂 Dataset & Preprocessing
- **Outlier Detection & Removal**: Applied the Interquartile Range (IQR) method to detect and remove outliers.
- **Missing Values**: Eliminated missing values to ensure data quality and model reliability.
- **Data Visualization**: Explored relationships between numerical, categorical, and target variables to support effective feature selection.

---

## 🛠️ Approach
- **Dummy Encoding**: Applied dummy encoding to selected features, including categorical and discrete numerical variables.
- **Baseline Categories**: Defined baseline categories proactively to minimize multicollinearity.
- **Assumption Checks**: Verified linear regression assumptions (multicollinearity, normality of residuals).
- **Statistical Analysis**: Evaluated the significance of the model and independent variables via F-statistic and p-values.

---

## 📊 Model Evaluation
Performance was measured using:
- **MAE** (Mean Absolute Error)
- **RMSE** (Root Mean Squared Error)
- **R² Score** (Coefficient of Determination)

Both approaches were compared based on these metrics to assess predictive accuracy and model fit.

---

## 🏆 Results
Both models achieved high and closely similar R² scores, making the difference in performance difficult to observe visually.
* **Model 1** (using raw numerical variables) is simpler in structure but delivered slightly lower error rates (MSE and RMSE) and a marginally higher R² compared to **Model 2**.
* **Model 2** (converting discrete-valued numerical variables into dummy variables) is more complex but did not show a clear performance advantage.
Final Decision:
**Model 1** was selected as the preferred model due to its simplicity, slightly better performance on the test set, and suitability for predicting new data.

---

## 📁 Repository Structure
├── data/ # Raw datasets
├── notebooks/ # Jupyter notebooks for data exploration, preprocessing, modeling, evaluation metrics and visualizations
├── requirements.txt # Project dependencies
└── README.md # Project documentation

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/nampham0804/HousePrice-FeatureEncoding-ModelComparison
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Open the notebooks to explore the analysis.
