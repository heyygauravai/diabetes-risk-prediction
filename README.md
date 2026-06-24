# diabetes-risk-prediction
# Diabetes Risk Prediction

Predicting diabetes risk using the Pima Indians Diabetes Dataset.

## Business Context
Early diabetes detection can prevent blindness, kidney failure, and amputation. 
This model identifies high-risk patients using standard diagnostic measurements 
available at any clinic.

## Dataset
- 768 patients, 8 diagnostic features
- Target: 1 = Diabetes, 0 = No Diabetes
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes)

## How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Open `diabetes-risk-prediction.ipynb` in Jupyter or Google Colab
3. Run all cells

## Key Steps
1. **Data Cleaning:** Replaced biologically impossible 0 values with median of non-zero values
2. **EDA:** Analyzed distributions and correlations between diabetic and non-diabetic patients
3. **Modeling:** Trained and compared Logistic Regression, Random Forest, and XGBoost
4. **Evaluation:** Cross-validation, confusion matrix, and classification report

## Results
| Model | Accuracy | CV Score |
|-------|----------|----------|
| Logistic Regression | 78.6% | 76.4% |
| Random Forest | 76.6% | 76.2% |
| XGBoost | 72.7% | 74.5% |

## Key Insights
- **Glucose** is the strongest predictor of diabetes
- **BMI** is the second strongest predictor  
- **Age** contributes significantly, particularly after 45
- Logistic Regression generalized best on this small dataset

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost
