# LAB5

## Tasks done for this lab:

### Task 1
A new engineered feature called **age_risk_group** was created by categorizing patient age into meaningful cardiovascular risk ranges. This feature helps the model capture nonlinear effects of age, since the relationship between age and heart disease is not always perfectly linear. Grouping ages into categories such as low, medium, high, and very high risk can improve interpretability and may also slightly improve model performance.

### Task 2
A different rule was tested by creating a binary feature called **high_cholesterol**, where cholesterol values greater than 240 were labeled as 1 and the rest as 0. This rule is medically meaningful and easier for the model to interpret than raw values alone. After testing, the performance can be compared with the baseline to determine whether the engineered threshold adds useful predictive information.

### Task 3
Instead of changing `top_k` for item names, we compared models trained on the **top 5**, **top 10**, and **all** important features. The results show how reducing the number of features affects model accuracy and which predictors remain most influential. In most cases, features such as age, cholesterol, maximum heart rate, chest pain, and oldpeak tend to stay among the most important.

### Task 4
Feature selection was applied using a model-based approach. This reduced the number of predictors while keeping the most important ones. If the selected-features model achieved similar accuracy to the baseline, then feature selection was beneficial because it simplified the model without losing much predictive power. If accuracy dropped, then keeping all features was more effective for this dataset.

### You can find the notebook in the src directory
