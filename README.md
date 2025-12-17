
```markdown
# Heart Disease Prediction

## Overview
This project aims to predict the presence of heart disease in patients based on various health parameters using several machine learning classification algorithms. The analysis involves data exploration, visualization, and model training with Logistic Regression, Decision Tree, and Random Forest classifiers.

## Dataset
The dataset used in this project is `Heart Disease.csv`, which contains 303 records and 14 features related to heart disease. Key features include age, sex, chest pain type (cp), resting blood pressure (trestbps), cholesterol (chol), fasting blood sugar (fbs), resting electrocardiographic results (restecg), maximum heart rate achieved (thalach), exercise-induced angina (exang), ST depression induced by exercise relative to rest (oldpeak), the slope of the peak exercise ST segment (slope), number of major vessels colored by fluoroscopy (ca), and thal (a blood disorder). The target variable indicates the presence (1) or absence (0) of heart disease.

## Methodology
1.  **Data Loading and Initial Exploration**: Loaded the dataset and performed initial checks for missing values, data types, and descriptive statistics.
2.  **Data Visualization**: Visualized the distribution of heart disease, age vs. heart disease, and a correlation heatmap to understand relationships between features.
3.  **Model Training and Evaluation**:
    *   **Logistic Regression**: Trained a Logistic Regression model and evaluated its performance using a confusion matrix and accuracy score.
    *   **Decision Tree Classifier**: Trained a Decision Tree Classifier and evaluated its performance, including a visualization of the decision tree.
    *   **Random Forest Classifier**: Trained a Random Forest Classifier, evaluated its performance, and analyzed feature importance.

## Results
The models were evaluated based on accuracy, precision, recall, and F1-score. Below is a summary of the performance:

| Model               | Accuracy | Precision | Recall | F1-Score |
| :------------------ | :------- | :-------- | :----- | :------- |
| Logistic Regression | 81.32%   | 0.82      | 0.84   | 0.83     |
| Decision Tree       | 73.63%   | 0.80      | 0.70   | 0.74     |
| Random Forest       | 82.42%   | 0.84      | 0.84   | 0.84     |

Random Forest achieved the highest accuracy of 82.42% among the models tested, demonstrating a strong capability in predicting heart disease from the given features.

### Feature Importance (Random Forest)
The Random Forest model also provided insights into feature importance, indicating which features were most influential in predicting heart disease.

## Setup and Usage
To run this project locally, you will need Python 3.x and the following libraries:

*   pandas
*   numpy
*   matplotlib
*   seaborn
*   scikit-learn
*   graphviz

You can install them using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn graphviz
```

1.  Clone the repository:
    ```bash
    git clone <repository-url>
    cd heart-disease-prediction
    ```
2.  Place the `Heart Disease.csv` file in the project directory.
3.  Run the Jupyter Notebook or Python script.

## Conclusion
This project successfully implemented and evaluated multiple machine learning models for heart disease prediction. The Random Forest Classifier showed the most promising results. Further improvements could involve more advanced feature engineering, hyperparameter tuning, and exploring other ensemble methods.

```
