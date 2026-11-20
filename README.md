# ❤️ Heart Disease Prediction – Machine Learning

## 📌 Overview
This project explores a heart disease dataset using Exploratory Data Analysis (EDA) and Machine Learning techniques. It focuses on identifying patterns in health-related attributes and comparing different classification algorithms to predict the presence of heart disease.

The project includes data exploration, handling invalid values, categorical encoding, feature scaling, model training, and evaluation.

## 📊 Exploratory Data Analysis (EDA)
The dataset was explored to understand its structure, distributions, and relationships between features.

EDA included:
- Dataset inspection using `head()`, `info()`, and `describe()`.
- Checking duplicate records and missing values.
- Examining the distribution of the target variable.
- Visualizing numerical feature distributions using histograms and KDE.
- Analyzing categorical features against heart disease outcomes.
- Exploring relationships between features using boxplots, violin plots, and correlation heatmaps.

## 🧹 Data Preprocessing
The following preprocessing steps were performed:

- **Handling invalid values:** Zero values in `Cholesterol` and `RestingBP` were identified as potentially invalid and replaced using the respective feature means calculated from non-zero values.
- **Categorical encoding:** Categorical features were transformed using Pandas `get_dummies()` with `drop_first=True`.
- **Feature scaling:** Standardization was applied to numerical features using `StandardScaler`.

## 🤖 Machine Learning Models
Five classification algorithms were trained and compared:

| Algorithm | Library |
|---|---|
| Logistic Regression | Scikit-learn |
| K-Nearest Neighbors (KNN) | Scikit-learn |
| Gaussian Naive Bayes | Scikit-learn |
| Decision Tree Classifier | Scikit-learn |
| Support Vector Machine (SVM) | Scikit-learn |

### Model Evaluation
The dataset was split into training and testing sets using an 80:20 ratio.

Models were evaluated using:
- Accuracy
- F1-score

The model comparison was used to examine the performance of different classification algorithms on the dataset.

## 💾 Model Export
The notebook exports the following files using Joblib:

- `KNN_heart.pkl` – Trained KNN model.
- `scaler.pkl` – Scaler object.
- `columns.pkl` – List of feature columns.

These artifacts were saved for potential future use in a prediction application.

## 🛠️ Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## 📁 Project Structure

```text
Heart-Disease-Prediction/
│
├── Heart_Disease_Prediction.ipynb
├── heart.csv
├── KNN_heart.pkl
├── scaler.pkl
├── columns.pkl
└── README.md
```

*The structure above represents the potential project structure; only files actually uploaded to the repository are included.*

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/Heart-Disease-Prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Heart-Disease-Prediction
   ```

3. Install the required libraries:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn joblib jupyter
   ```

4. Ensure the dataset `heart.csv` is available in the project directory.

5. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open `Heart_Disease_Prediction.ipynb` and run the notebook cells.

## ⚠️ Disclaimer
This project is intended for educational and machine learning practice purposes only. It is not intended for medical diagnosis, treatment, or clinical decision-making.



Once you have the notebook and README on GitHub, we can make this repository genuinely internship-ready without unnecessarily complicating it.
