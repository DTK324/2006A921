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

Requirements
To run this application, make sure you have the following Python packages installed:

PyQt6 – for creating the GUI interface

matplotlib – for visualizations and charts

numpy – for numerical operations and array handling

pandas – for data loading and manipulation

scikit-learn – for classical ML models, preprocessing, and metrics

tensorflow – for training deep learning models (MLP, CNN, RNN)

plotly – for interactive 2D/3D dimensionality reduction visualization

umap-learn – for UMAP dimensionality reduction

reportlab – (only required for PDF generation, optional)