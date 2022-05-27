# Project_4

# Deployed Link: https://rebecca-kwon.github.io/Project_4/


## DataSets used 

https://www.kaggle.com/competitions/home-credit-default-risk/data

application_train.csv

## Objective

Using the application train datasets, we used machine learning models to predict on loan defaults. 

## Method

The Raw data was simply visualized using Tableau to show all column names, interesting columns and their ranges, overall look at the number of defaulted loans, as well as multiple outcomes based on different factors such as occupation, housing type, and family type. 

Next, data clean up was performed to remove unnecessary data as well as to perform imputation on missing data fields. Initial columns were dropped to simplify the process before proceeding to checking and removing any outliers. Then, Nulls were removed to reduce the dataset. One Hot coding was implemented for categorical values and a simple imputer was used to impute for missing values within the dataset. Dimensionality reduction was performed using the Random Forest Classifier model. With each model, there was a test/train and split set for the data. 

From the Random Forest Classifier model, a horizontal plot of column names were ranked on importance to the dataset. The outcome of the RFC model was a training score of 1.0 and a testing score of 0.918. 

Next, using a supervised learning method, Logistic Regression Classifier, the model was fit on the data to produce a training data score of 92% and a testing score of 92%. 

![image](https://user-images.githubusercontent.com/95327812/170607442-76acf6ed-deab-4f4b-aae7-20fd631f5c75.png)

Because the dataset was over 100K samples, the SGD classifier was used to produce the following results: 

![image](https://user-images.githubusercontent.com/95327812/170607506-a0271e3c-3cf7-4399-b681-b40793678023.png)

Finally, a deep learning model with neural network optimizers was used to create an outcome of a loss of 27% and an accuracy of 92%. The data was split and scaled. Then a new sequential model was created with hyperparameter options. The Kerastuner Library was used to create the best hyperparameter options. A Total of 4 layers with the tanh activation method was used to optimize the results. Each had 16 units. The last layer consisted of 1 unit using the Sigmoid Activation Method. 

Overall, each machine learning method produced similar accuracy scores. 


## Machine Learning Tools used:

- Logistic Regression
- Deep Learning with Neural Network Optimizers
- RandomForest Classifier 
- Simple Imputation 


## Tools used

- Machine Learning
  - Static images
- Python Pandas
- Python Matplotlib
- MongoDB (&MongoDB Cloud)
- Tableau
- HTML - Deployed on GitHub
- Javascript


## Group Members 

- Angele Yazbec
- Rebecca Kwon
- Turgut Ozsirkinti
- Neil Tipton
- Daniel Garza 
