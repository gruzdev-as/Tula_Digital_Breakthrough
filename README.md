# Tula_Digital_Breakthrough
Link to the championship: https://hacks-ai.ru/championships/758260

The main idea is to try to predict the number of potential patient according to the ICD Code, Patient sex, Date and City. 

What did I do to solve this task: 

1) Did a data preparation:
    * Created new features according to the data,
    * Sorted the data, using new features.
2) Did EDA for the prepared dataset:
    * Visualized the data distribution,
    * Checked whether the data contain any insights,
    * Checked the relationships between the target variable and features,
    * Analyzed target variable as a time series,
    * Hypotheses about how to solve the task have been created.
3) Build CatBoost models to check hypotheses:
    * Decided to use TimeSeriesSplit to keep relationship between date and the target variable;
    * Created a classification model pipelines (Tried to predict range for the target variable); 
    * Created a regression model pipelines; 
    * Tuned the hyperparameters for the models

# Install all the necessary libraries

To install all the libraries do 

```sh
pip install -r requirements.txt
```

# How to check train process

1) To prepare the data for EDA and training launch "Tula Data Preparation.ipynb" 
2) You may skip "Tula_EDA.ipynb" file, because it doesn't contain any code, that modify the train data 
3) Use 'Tula model_building_catBoost.ipynb' for model creation and to create a submission file 
