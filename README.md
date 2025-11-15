# Lung Cancer Prediction Project

This project builds and evaluates several machine learning models to predict lung cancer based on patient survey data. It performs exploratory data analysis (EDA), preprocessing, model training, evaluation, and provides a simple CLI-style prediction function.

---

## 📁 Dataset

The project uses a CSV dataset named **`survey lung cancer.csv`**, which contains patient attributes such as:

* Age
* Gender
* Smoking habits
* Symptoms (shortness of breath, chest pain, etc.)
* Lung cancer diagnosis label

The dataset is loaded using `pandas` and explored through:

* Data preview (`head()`)
* Datatypes (`info()`)
* Duplicate and null-value checks
* Countplots and heatmaps for visualization

---

## 🧹 Data Preprocessing

The notebook performs:

* Label encoding of categorical features
* Conversion of gender and other binary attributes into numerical format
* Feature/target split (`X`, `y`)
* Train/test split using `train_test_split()`

---

## 📊 Exploratory Data Analysis (EDA)

The EDA includes:

* Distribution visualizations using `seaborn`
* Correlation heatmap
* Feature countplots highlighting class imbalances

These visualizations help understand the data structure and feature relationships.

---

## 🤖 Models Trained

Multiple machine learning models are trained and compared:

### 1. **Random Forest Classifier**

* Demonstrates strong performance
* Accuracy printed after evaluation

### 2. **Gaussian Naive Bayes**

* Evaluated using accuracy score and confusion matrix
* Good baseline classifier

### 3. **Linear Regression (RMSE Evaluation)**

* Tested but not ideal for classification
* RMSE score is computed

A combined metrics summary is plotted using `matplotlib`, comparing model accuracies.

---

## 🧪 Model Evaluation

Evaluation techniques include:

* Accuracy score
* Confusion matrix
* Mean squared error (MSE) and RMSE

Results are plotted for easier visual comparison.

---

## 🔍 Prediction Function

A custom function `predict_lung_cancer()` is included, allowing manual entry of patient attributes to get a prediction using the selected classifier.

This acts as a basic command-line interface for testing the model.

---

## 🛠️ Technologies & Libraries

* **Python 3**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**

---

## 🚀 How to Run the Project

1. Clone the repository:

   ```bash
   git clone <repo-url>
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook Lung_Cancer.ipynb
   ```
