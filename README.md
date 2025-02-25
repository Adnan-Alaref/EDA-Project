# Car Price Prediction - EDA, Stacking Regression & Polynomial Regression & Assumptions

## 📌 Project Overview
This project aims to predict car prices using multiple machine learning models, including ensemble techniques like stacking and bagging. The dataset is sourced from Cardekho and contains various car features such as year, fuel type, seller type, and transmission. We perform Exploratory Data Analysis (EDA) to uncover trends, preprocess data, and implement a range of regression models to achieve accurate predictions.

## 📂 Dataset
- **Source**: Kaggle (Vehicle Dataset from Cardekho)
- **Features**:
  - `Year` - Manufacturing year of the car
  - `Present Price` - Current market price of the car (in lakhs)
  - `Selling Price` - The price at which the car was sold (target variable)
  - `Fuel Type` - Petrol/Diesel/CNG
  - `Seller Type` - Dealer or individual seller
  - `Transmission` - Manual or automatic
  - `Owner` - Number of previous owners
- **Target Variable**: `Selling Price`

## 🛠️ Methodology
### 1️⃣ Data Preprocessing
- Handled missing values and outliers
- Encoded categorical features
- Standardized numerical features using `StandardScaler`
- Split data into training and test sets

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized distributions and relationships between features
- Checked correlation heatmaps
- Used scatter plots and boxplots to detect patterns

### 3️⃣ Model Selection & Training
Implemented and compared multiple regression models:
- **Linear Models**: Linear Regression, Ridge Regression
- **Tree-based Models**: Decision Tree, Random Forest, Extra Trees, Gradient Boosting
- **Advanced Models**: XGBoost, K-Nearest Neighbors
- **Ensemble Learning**:
  - **Bagging**: Random Forest, ExtraTrees, Bagging Regressor
  - **Stacking**: Combined multiple models to improve predictions
  - **Voting Regressor**: Combined predictions from different models

### 4️⃣ Model Evaluation
- Used `Mean Squared Error (MSE)`, `Root Mean Squared Error (RMSE)`, and `R² Score`
- Compared model performances with visualizations
- Identified the best-performing model based on metrics and computational efficiency

## 📊 Results
- The **Stacking Regressor** achieved the best performance with a high R² score and low RMSE.
- Feature importance analysis showed that `Present Price` and `Year` were the most influential factors.
- Ensemble models outperformed individual models, confirming the strength of combined learning approaches.

## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/your-username/car-price-prediction.git

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook car-prediction-eda-stackingregression.ipynb
```

## 📌 Future Improvements
- Hyperparameter tuning with GridSearchCV
- Deployment using Flask/Django
- Explainability using SHAP for feature contributions

## 📜 License
This project is licensed under the MIT License.

---
Feel free to contribute or suggest improvements! 😊
