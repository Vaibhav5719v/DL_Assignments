# Multi-Layer Perceptron (MLP) Classifier on Iris Dataset

This project implements a Multi-Layer Perceptron (MLP) Neural Network using `scikit-learn` to perform multi-class classification on the classic Iris Flower Dataset. The pipeline includes data preprocessing, feature standardization, model training, and performance visualization.

---

## 📌 Features & Workflow

- **Dataset**: Iris dataset containing 150 samples across 3 species (`setosa`, `versicolor`, `virginica`) with 4 features per sample.
- **Data Preprocessing**:
  - Stratified 80/20 train-test split (`train_test_split`) to preserve class proportions (`random_state=42`).
  - Feature scaling using `StandardScaler` fitted strictly on training data.
- **Model Architecture**:
  - **Type**: `MLPClassifier` (Feedforward Neural Network)
  - **Hidden Layers**: Two hidden layers with shape `(16, 8)`
  - **Activation**: ReLU
  - **Optimizer**: Adam (`learning_rate_init=0.001`)
  - **Max Iterations**: 500
- **Evaluation & Visualization**:
  - Classification Metrics (Accuracy, Precision, Recall, F1-Score)
  - Heatmap Confusion Matrix via Seaborn
  - Training Loss curve plot (`mlp.loss_curve_`)

---

## 📁 Repository Structure

```text
DL_Assignments/
└── Assignment_2/
    └── Assignment_2.ipynb    # Jupyter Notebook containing full implementation

```

---

## ⚙️ Setup & Requirements

### Dependencies

Ensure you have Python 3.8+ installed along with the required libraries:

```bash
pip install numpy matplotlib seaborn scikit-learn

```

---

## 🚀 How to Run

1. **Clone the repository:**
```bash
git clone [https://github.com/Vaibhav5719v/DL_Assignments.git](https://github.com/Vaibhav5719v/DL_Assignments.git)
cd DL_Assignments/Assignment_2

```


2. **Launch Jupyter Notebook:**
```bash
jupyter notebook Assignment_2.ipynb

```


3. **Run all cells** to execute data loading, model training, and visualization outputs.

---

## 📊 Results & Performance

* **Test Accuracy**: **96.67%**

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
| --- | --- | --- | --- | --- |
| **Setosa** | 1.00 | 1.00 | 1.00 | 10 |
| **Versicolor** | 1.00 | 0.90 | 0.95 | 10 |
| **Virginica** | 0.91 | 1.00 | 0.95 | 10 |
| **Accuracy** |  |  | **0.97** | **30** |
| **Macro Avg** | 0.97 | 0.97 | 0.97 | 30 |
| **Weighted Avg** | 0.97 | 0.97 | 0.97 | 30 |

```

```
