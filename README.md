Group 7 report about Titanic incident analyzing

Abstract 
This report was written to create a model capable of predicting whether a traveler survived or not. In the model, Gender, Age and Pclass will be included and we will use two machine learning method which is Linear regression.

I.Introduction

Incident can happen anytime in any era. While it takes away money, asset and human life sometimes it still can spare some survivors. When looking at the data about some incident, we question ourself, are survivors predictable? Looking at the chart you can see that with the change in gender the percent that one can survive have already been significantly different.  In other words, we want to find out a feature that will make an individual more likely to survive in an incident. This report will use some predict model to answer this question. 
!{}()
While there is many infamous incident, the data we will use belong to Titanic incident which happen in 1911. On that ship in 4/1911, there was 2204 and there was only 1502 people suvived.
II. Methodology

2.1. Source of data

We will use the provided data which come from Kaggle. Kaggle give us two excel files which include file for training and for testing model. We will only use train.csv for our model.
2.2. Variable

2.2.1. Data dictionary

The table was provided by Kaggle. 

![](images/dictionary-table.png)

2.2.2. Variable Selection

In the model we created, we will only use three variable which is Sex, Age and Pclass.

2.2.3. Preprocessing data

As the age is hard to predict, for null value in the Age column, we decide to drop it. 
As for Sex, we will change variable into 1/0(male/female).

2.2.4. Model
In this report only two model will be use which is linear regression model.

III. Result
After training our model we come up with a equation like below:
ŷ= 0.40 + -0.16 * Pclass + -0.07 * Age + -0.22 * Sex

This equation indicate that the decrease in Pclass and the increase in Age will lead to the decrease in the total resule. If the gender is male(which is one in the model) will also decrease the survivor chance.

But is this model reliable? If we looking at 
