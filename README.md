# Risk of Stroke Prediction 
Author: Juliana Sahagun
## Goal: The goal is to help predict if a person is high risk for a stroke considering their health conditons.
### Data:
1. Source :
    * https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

### Methods
* Data Cleaning:
    - Dropped the columns id because it was unnesary towards finding our target
    - Imputed missing value by removing the rows with missng values to not introduce any errors to the datas(less than 1% was missing)
    -Changed the incorrect datatypes to its correct type : 'age' → integer & 'bmi' → float
    -Removed value 'other' in the gender column as it was insignifcant to our data
* Preprocessing: 
    -Set target to 'stroke' and split features
    -Validatation Split
    -OneHotEncoded the categorical features since they were all nominal and StandardScaler the numerical features
    -Made a ColumnTransformer to match the transformation to the type of column
* Testing LogisticRegression, DecisionTree, and KNearestNeighbors:
    -Made three different models and hypertuned them to their optimal potiental using GridSearchCV
    -Evaluated each model with 'evaluate_classification' and 'classification_report'
    -

### Results
-Overall, people who have health conditons that are high risk tend to be at higher risk for stroke danger.
- Key Findings:
#### Visual 1
![image](https://user-images.githubusercontent.com/104885846/181685229-b388229c-b7e8-47f4-87d2-07409e17822c.png)

#### Visual 2
![image](https://user-images.githubusercontent.com/104885846/181685255-4a0be2d9-4e35-4c35-ae96-096206e8caa8.png)


#### Machine learning Results:
-

###### Recommendations:

# For Further Information:
For any additional questions or concerns in regards to my sales predictions, please contact me at julianas4013@gmail.com. Thank you!
