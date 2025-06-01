# Task 5 - Decision Trees & Random Forests

## 🎯 Objective
Compare Decision Tree and Random Forest models on the Heart Disease dataset.

## 📁 Dataset
- Name: `heart.csv`
- Source: [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

## 🛠 Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## 🧪 Steps Performed
1. Loaded dataset and split into features and labels
2. Trained a basic Decision Tree
3. Visualized the full tree
4. Trained a limited-depth Decision Tree to prevent overfitting
5. Trained a Random Forest and evaluated performance
6. Compared accuracies of models
7. Visualized feature importances
8. Used cross-validation to check stability

## 🧾 Sample Output

✅ Dataset loaded:
   age  sex  cp  trestbps  chol  ...  oldpeak  slope  ca  thal  target
0   52    1   0       125   212  ...      1.0      2   2     3       0
1   53    1   0       140   203  ...      3.1      0   0     3       0
2   70    1   0       145   174  ...      2.6      0   0     3       0
3   61    1   0       148   203  ...      0.0      2   1     3       0
4   62    0   0       138   294  ...      1.9      1   3     2       0

[5 rows x 14 columns]

📊 Decision Tree Accuracy: 0.9853658536585366

Decision Tree Classification Report:
              precision    recall  f1-score   support

           0       0.97      1.00      0.99       102
           1       1.00      0.97      0.99       103

    accuracy                           0.99       205
   macro avg       0.99      0.99      0.99       205
weighted avg       0.99      0.99      0.99       205

📉 Limited Tree Accuracy: 0.7804878048780488

🌲 Random Forest Accuracy: 0.9853658536585366
Random Forest Classification Report:
              precision    recall  f1-score   support

           0       0.97      1.00      0.99       102
           1       1.00      0.97      0.99       103

    accuracy                           0.99       205
   macro avg       0.99      0.99      0.99       205
weighted avg       0.99      0.99      0.99       205


📌 Feature Importances:
 cp          0.135072
ca          0.127327
thalach     0.122169
oldpeak     0.121905
thal        0.110518
age         0.077908
chol        0.074822
trestbps    0.071171
exang       0.057594
slope       0.045782
sex         0.028731
restecg     0.018557
fbs         0.008444
dtype: float64
