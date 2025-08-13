# breast-cancer-classification
Binary classification using logistic regression on the Breast Cancer Wisconsin dataset.

---

## Dataset

**Source:** [Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)  
- **Samples:** 569  
- **Features:** 30 numeric diagnostic features (e.g., radius, texture, smoothness)  
- **Target:** `diagnosis` — B (benign) or M (malignant)

---

## Technologies Used

- **Python 3**
- **Jupyter Lab**
- [pandas](https://pandas.pydata.org/) — Data manipulation
- [numpy](https://numpy.org/) — Numerical computations
- [scikit-learn](https://scikit-learn.org/) — Machine learning model & metrics
- [matplotlib](https://matplotlib.org/) & [seaborn](https://seaborn.pydata.org/) — Visualization

---

## Workflow

1. **Data Loading & Exploration**
   - Read CSV data into pandas DataFrame
   - View first rows, check for missing values

2. **Data Preprocessing**
   - Encode target variable (`diagnosis`) into binary values: 0 = benign, 1 = malignant
   - Scale numeric features with `StandardScaler` to improve model performance

3. **Model Training**
   - Split data into training and test sets (80/20 split)
   - Train a `LogisticRegression` model

4. **Evaluation**
   - Accuracy score
   - Confusion matrix
   - Classification report (precision, recall, F1-score)

5. **Visualization**
   - Confusion matrix heatmap
   - Bar chart of feature importance (optional)

---

## Results

Confusion Matrix:

[[70 1]
[ 2 41]]


- **Accuracy:** 97.4%  
- **Interpretation:** Out of all test samples, the model correctly classified 97% of tumors.

---

## How to Run This Project

```bash
# Clone this repository
git clone https://github.com/sablermead/breast-cancer-classification.git
cd breast-cancer-classification

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Lab
jupyter lab
