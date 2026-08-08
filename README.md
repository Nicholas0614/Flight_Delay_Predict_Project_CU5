# ✈️ Flight Delay Prediction

A Machine Learning project that predicts whether a flight will be delayed based on flight information such as airline, origin, destination, departure time, day of the week, and distance.

The project uses historical flight data from 2024 and applies data cleaning, exploratory data analysis, feature engineering, preprocessing, and Logistic Regression to build a flight delay prediction model.

## 📌 Project Overview

Flight delays can be caused by many different factors, making them difficult to predict.

The goal of this project is to explore flight data and build a machine learning model that can predict whether a flight will be delayed by more than **15 minutes**.

### 🎯 Target

A flight is classified as:

* `0` → On Time
* `1` → Delayed

A flight is considered delayed when its arrival delay is greater than 15 minutes.

## 📊 Dataset

The dataset contains **7 million+ flight records** from 2024 with information including:

* Flight date
* Airline
* Origin airport
* Destination airport
* Scheduled departure time
* Departure time
* Arrival time
* Distance
* Scheduled flight duration
* Cancellation information
* Diversion information
* Delay information

The original dataset contains **7,079,081 records and 35 columns**.

## 🔎 Data Processing

The project includes several preprocessing steps:

1. Removed cancelled flights
2. Created the `delayed` target variable
3. Removed columns that could cause data leakage
4. Handled missing values
5. Removed duplicate records
6. Extracted departure hour from scheduled departure time
7. Removed invalid departure-hour values
8. Prepared categorical and numerical features for machine learning

### Features Used

**Categorical features:**

* Airline
* Origin
* Destination

**Numerical features:**

* Month
* Day of week
* Scheduled departure hour
* Distance

## 📈 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand patterns in the dataset and investigate relationships between flight characteristics and delays.

The analysis includes visualizations related to:

* Flight delays
* Airlines
* Departure times
* Airports
* Flight distance
* Other flight characteristics

## 🤖 Machine Learning

The project uses **Logistic Regression** for binary classification.

The preprocessing pipeline consists of:

* `OneHotEncoder` for categorical variables
* `StandardScaler` for numerical variables
* `LogisticRegression` for prediction

The model uses balanced class weights to help handle the distribution between delayed and non-delayed flights.

## 📊 Model Performance

The model was evaluated using accuracy, precision, recall, F1-score, and a confusion matrix.

| Metric   |      Score |
| -------- | ---------: |
| Accuracy | **60.73%** |
| F1-Score | **60.91%** |

The results show that the model can identify delayed and on-time flights with a moderate level of performance.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Joblib

## 📁 Project Structure

```text
Flight_Delay_Predict_Project_CU5/
│
├── Flight_Predict.ipynb
├── flight_delay_model_full.joblib
├── Flight_Delay_Prediction_Slides.pdf
├── README.md
└── .gitignore
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Nicholas0614/Flight_Delay_Predict_Project_CU5.git
```

### 2. Navigate to the project

```bash
cd Flight_Delay_Predict_Project_CU5
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib scikit-learn jupyter joblib
```

### 4. Open the notebook

```bash
jupyter notebook Flight_Predict.ipynb
```

Run the notebook cells from top to bottom to reproduce the data processing, analysis, model training, and evaluation.

## 📄 Project Presentation

The project presentation is available here:

`Flight_Delay_Prediction_Slides.pdf`

## 💡 What I Learned

Through this project, I gained practical experience in:

* Working with large datasets
* Data cleaning and preprocessing
* Exploratory Data Analysis
* Feature engineering
* Handling categorical and numerical data
* Building machine learning pipelines
* Training classification models
* Evaluating machine learning performance
* Saving trained models with Joblib

## 👨‍💻 Author

**Nicholas**

GitHub: [Nicholas0614](https://github.com/Nicholas0614)

---

⭐ If you find this project interesting, feel free to explore the notebook!
