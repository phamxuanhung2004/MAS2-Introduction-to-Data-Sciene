Group 7 report about Titanic incident analyzing

Abstract 
This report was written to create a model capable of predicting whether a traveler survived or not. In the model, Gender, Age and Pclass will be included and we will use two machine learning method which is Linear regression and Logistic regression to predict survival chance. Two model will be compared to each other and to the base to find predicting accuracy. Lastly, we will try to deduce the result that we have.

1. Introduction

Titanic has always been an disaster when talking about voyage. The incident took place way back on April 15th, 1912, when the Titanic
sank during its first voyage after striking an iceberg, resulting in the tragic loss of 1502 passengers and crew out of a total of 2224.This sensational tragedy
horrified the international community and led towards action taking by formulating better safety regulations for ships. While it is still controversial about who took responsibility of the incident, we can agree that there are certain characteristics share between survivors. In this report, we try to find out what features will likely make a individual survive in the Titanic incident and perhaps in a disaster as a whole.

2. Methodology

2.1. Source of data

We will use the provided data which come from Kaggle. Kaggle give us two excel files which include file for training and for testing model. We intend to use one file for training and one file for testing but i find out the the testing file did not include the survived index so in this report the only file that we use will be ![](train.csv)
2.2. Variable

2.2.1 Data dictionary
The table was provided by Kaggle. In the model we will change male to 1 and female to 0.


2.2.2 Variable Selection
There are many variable provided, but in the model, we decide to use only three independent variables which is Sex, Age and Pclass. For dependent variable, we will use survived for our model. 
Why we choose this variable.


For this project we will limit at three varible to keep the result explainable. Beside, we do not w
