# 🚢 Titanic Survival Prediction (Machine Learning Project)

This project predicts the survival of passengers on the Titanic using supervised machine learning models. Based on historical passenger data such as age, gender, class, etc., the model determines the likelihood of survival.

## 📊 Objective

To apply classification algorithms (like Logistic Regression, Decision Trees, Random Forest) to predict whether a passenger survived the Titanic disaster or not.

## 📁 Dataset

We use the famous Titanic dataset available from Kaggle:

- **Source**: [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)
- **Files**:
  - `train.csv` - contains the training data with labels (survived or not).
  - `test.csv` - used for testing the model predictions.
  - `gender_submission.csv` - sample submission format.

### 🔢 Sample Raw Data (train.csv)

| PassengerId | Survived | Pclass | Name                             | Sex    | Age  | SibSp | Parch | Ticket   | Fare   | Cabin | Embarked |
|-------------|----------|--------|----------------------------------|--------|------|--------|--------|----------|--------|--------|-----------|
| 1           | 0        | 3      | Braund, Mr. Owen Harris          | male   | 22   | 1      | 0      | A/5 21171| 7.25   | NaN    | S         |
| 2           | 1        | 1      | Cumings, Mrs. John Bradley (Florence Briggs Thayer)| female | 38 | 1 | 0 | PC 17599 | 71.2833| C85   | C         |
| ...         | ...      | ...    | ...                              | ...    | ...  | ...    | ...    | ...      | ...    | ...    | ...       |

## 🧠 Features Used

- `Pclass` (Ticket class)
- `Sex` (Gender)
- `Age`
- `SibSp` (No. of siblings/spouses aboard)
- `Parch` (No. of parents/children aboard)
- `Fare`
- `Embarked` (Port of Embarkation)

## 🛠️ Technologies

- Python 3
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Google Colab / Jupyter Notebook

## 🧪 Model Pipeline

1. **Data Cleaning**: Handle missing values, encode categorical variables.
2. **Feature Engineering**: Extract titles from names, create family size feature, etc.
3. **Modeling**:
    - Logistic Regression
    - Decision Tree
    - Random Forest
    - Support Vector Machine
4. **Evaluation**: Accuracy, Confusion Matrix, Cross-Validation
5. **Visualization**: Survival rates by sex, class, and age group

## 📈 Example Output

- Accuracy Score: ~80%
- Confusion Matrix: shows TP, FP, FN, TN
- Graphs: Survival rate by gender/class, Age distribution, etc.

## 🚀 How to Run

### In Google Colab:
1. Upload `train.csv` and `test.csv` files.
2. Open the notebook: [Titanic_Prediction.ipynb](#)
3. Run all cells step-by-step.

### Locally:
```bash
git clone https://github.com/yourusername/titanic-prediction.git
cd titanic-prediction
pip install -r requirements.txt
python titanic_model.py
