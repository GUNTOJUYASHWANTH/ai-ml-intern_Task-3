#  Housing Price Prediction using Linear Regression

## 📌 Objective
Implement and understand **Simple** and **Multiple Linear Regression** using Scikit-learn to predict house prices based on features like area, bedrooms, bathrooms, location access, etc.

## 🧰 Tools & Libraries
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📁 Dataset
**File:** `Housing.csv`  
The dataset includes features such as:
- `area` – Total square feet
- `bedrooms`, `bathrooms`
- `stories`, `parking`
- `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`
- `furnishingstatus`
- `price` – Target variable

---

## 🔍 Steps Followed

### 1️⃣ Import and Preprocess Dataset
- Loaded the dataset using Pandas
- Performed one-hot encoding on categorical variables using `pd.get_dummies()`
- Dropped the target variable (`price`) to separate features (`X`) and target (`y`)

### 2️⃣ Split into Train-Test Sets
- Used `train_test_split` from Scikit-learn
- 80% data for training and 20% for testing
- ![image](https://github.com/user-attachments/assets/6bc8cec2-42bd-4a6e-8d83-880bf3d35d18)


### 3️⃣ Fit Linear Regression Model
- Created and trained a Linear Regression model using `sklearn.linear_model.LinearRegression`

### 4️⃣ Model Evaluation
Evaluated model performance using:
- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **R² Score**

### 5️⃣ Plot and Interpret
- Plotted a **Simple Linear Regression** (e.g., area vs. price)
- Interpreted coefficients to understand the impact of each feature
![image](https://github.com/user-attachments/assets/3a4c9d50-f157-4a14-95d3-48b40d3837a4)


## 📊 Results

### 🔢 Metrics
- **MAE**: ~ ₹970043.40
- **MSE**: ~ ₹1754318687330.66
- **R² Score**: ~ 0.6529

### 📈 Feature Coefficients (Examples)
Intercept: 260032.35760741401
Coefficients:
area                               2.359688e+02
bedrooms                           7.677870e+04
bathrooms                          1.094445e+06
stories                            4.074766e+05
parking                            2.248419e+05
mainroad_yes                       3.679199e+05
guestroom_yes                      2.316100e+05
basement_yes                       3.902512e+05
hotwaterheating_yes                6.846499e+05
airconditioning_yes                7.914267e+05
prefarea_yes                       6.298906e+05
furnishingstatus_semi-furnished   -1.268818e+05
furnishingstatus_unfurnished      -4.136451e+05
dtype: float64

## 📷 Visualization
A regression line was plotted between `area` and `price` to visualize the trend using simple linear regression.

![image](https://github.com/user-attachments/assets/c1cb676d-b809-4632-8303-fda095ab865d)

![image](https://github.com/user-attachments/assets/d202f7d2-91fe-4147-b8d8-2824bfe3ea1b)
![image](https://github.com/user-attachments/assets/ac44ae8d-0c50-430f-82a6-b63a107dc40b)



## 📦 How to Run
1. Install requirements (optional):
   ```bash
   pip install pandas scikit-learn matplotlib seaborn
