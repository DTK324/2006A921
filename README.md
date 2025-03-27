# Machine Learning Course GUI (MKT3434_2025)

This GUI application is developed as part of the MKT3434 Machine Learning course. It provides an interactive interface to experiment with classical machine learning and deep learning algorithms, visualize training outcomes, and evaluate the impact of preprocessing techniques.

---

## 🚀 Features Implemented

### ✅ Dataset Selection
- Built-in datasets: Iris, Breast Cancer, Digits, Diabetes, MNIST
- Load custom datasets via CSV
- Target column selection via dialog window

### 🧪 Preprocessing
- **Missing Value Handling** (using `SimpleImputer`)
  - Mean Imputation
  - Median Imputation
  - Most Frequent
  - Constant Fill
- **Scaling Methods**
  - No Scaling
  - StandardScaler
  - MinMaxScaler
  - RobustScaler
- **Train/Test Split Control** using QDoubleSpinBox

### 📊 Visualization
- PCA visualization for classification datasets
- Scatter plots for regression results
- Confusion matrix and metrics display
- Live training history (accuracy/loss) for deep learning

### 🧠 Classical ML Algorithms
- Linear Regression (MSE, MAE, Huber Loss)
- Logistic Regression (Cross-Entropy, Hinge Loss)
- SVM (Classification & Regression) with kernel/C/epsilon control
- Naive Bayes (GaussianNB with priors: uniform, auto, manual)
- Decision Tree
- Random Forest
- K-Nearest Neighbors


### 📈 Imputation Strategy Comparison
- Compare Mean, Median, Most Frequent, and Constant strategies on MSE (for regression tasks)
- Display results within GUI for selected dataset (e.g., Diabetes)

---

## ⚙️ How to Run

### 🔧 Requirements
```bash
pip install -r requirements.txt
```

### ▶️ Launch the GUI
```bash
python 2006A921.py
```

---

## 🧾 Submission

- ✅ Python file: `2006A921.py`
- ✅ README.md (this file)
- ✅ PDF Report (2–3 pages) with:
  - GUI Screenshots
  - Description of enhancements
  - Results of imputation method comparisons

---

## 🔗 Repository Instructions

- Fork the course repo: https://github.com/bayraktare/MKT3434_2025
- Create a branch named `2006A921`
- Push your code + documentation to your branch

---
### 🏠 Boston Housing Note
- The original `load_boston` dataset has been removed from `scikit-learn` due to ethical concerns.
- In this project, a local alternative dataset `BostonHousing.csv` is used instead.

### 🐍 Python Version
- Developed and tested with Python 3.10.11


## 🧭 How to Use New Features

### 1. 📂 Dataset Selection
- Choose from built-in datasets (e.g., **Iris**, **Diabetes**, **Digits**, etc.) using the top-left dropdown.
- To load your own dataset, click the **"Load Data"** button and select a `.csv` file.
- A popup dialog allows you to choose the target (label) column.

### 2. 🧪 Preprocessing Options
- **Missing Value Handling** (via `SimpleImputer`):
  - Options: `Mean Imputation`, `Median`, `Most Frequent`, `Constant`
- **Scaling**:
  - Choose from `Standard`, `MinMax`, `Robust`, or no scaling at all.
- **Train/Test Split**:
  - Set the split ratio using the provided QDoubleSpinBox (from 10% to 90% test size).

### 3. 🤖 Model Training (Classical ML)
- Navigate to the respective tab (e.g., `Linear Regression`, `SVM`, `Naive Bayes`, etc.).
- Adjust model parameters directly from the GUI (e.g., `C`, `kernel`, `loss function`, etc.).
- Click the `Train [ModelName]` button to initiate training.
- Model evaluation results (MSE, Accuracy, etc.) and visualizations are displayed automatically.

### 4. 📈 Imputation Strategy Comparison
- The GUI allows comparison of imputation strategies (`Mean`, `Median`, `Most Frequent`, `Constant`) for regression models.
- Results (e.g., MSE) are displayed in the visualization panel using the selected dataset (e.g., **Diabetes**).

### 5. 📊 Visualization Panel
- **Classification**: PCA projection is used for 2D visualization.
- **Regression**: Scatter plot of actual vs. predicted values.
- **Metrics Panel**: Displays Accuracy, Confusion Matrix, MSE, and more in the text box.
