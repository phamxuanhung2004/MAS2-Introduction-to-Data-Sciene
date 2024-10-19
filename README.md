# Group 7 Report: 🚢 Titanic Incident Analyzing

**Members**:

Phạm Xuân Hưng: 22080317

Vũ Tiến Phúc: 22080336

Trần Kim Quang Minh: 22080329

Nguyễn Văn Ngọc Sơn: 22080341

Lương Việt Hoàng: 22080313

***`Abstract:`***

`This report was written to create a model capable of predicting whether a traveler survived or not `

`In the model: Gender, Age & Pclass will be included and we will use 2 Machine Learning Method (Linear regression) `

---

## I. Introduction
- Incident can happen anytime in any era. While it takes away money, asset and human life sometimes it still can spare some survivors. 

- When looking at the data about some incidents, we question ourselves, are survivors predictable? 

- Looking at the chart you can see that with the change in gender, the percent that one can survive have already been significantly different.  

In other words, we want to find out a feature that will make an individual more likely to survive in an incident. 

This report will use some predict models to answer this question. 

![](images/maleversusfemale.png)

While there are many infamous incidents, the data we will use belong to Titanic incident which happened in 1911. 

From 2204 individuals on that ship in 4/1911, there was **`only 1502 people suvived`** after the accident.

---

## II. Methodology

### 2.1. Source of data

We will use the provided data which comes from Kaggle. 

Kaggle gives us two excel files which include file for training and for testing model. We will only use train.csv for our model.

### 2.2. Variable

### 2.2.1. Data dictionary

The table was provided by Kaggle. 

![](images/dictionary-table.png)

### 2.2.2. Variable Selection

![](images/coefficientvisualization1.png)

In the model we created, we will only use three variables which is **Sex Age Pclass**.

### 2.2.3. Preprocessing data

As the Age is hard to predict, for Null values in the Age column, we decide to drop it. 

As for Sex, we will change variable into **1 (male) / 0 (female)**

### 2.2.4. Model
In this report the only model will be use which is linear regression model.

---

## III. Result

After training our model, we come up with a equation like below:

**` ŷ= 0.40 + -0.16 * Pclass + -0.07 * Age + -0.22 * Sex `**

This equation indicates that the decrease in Pclass & the increase in Age will lead to the decrease in the total resule. If the gender is male(which is one in the model) will also decrease the survivor chance.

But is this model reliable? If we look at OLS Regression Result, we can see that **all of the P-value is really small**, which is a good sign as every variables that we use are significant. 

But when we look at the R square: **0.37** - not a really good & strong relationship but in fact, it is actually a moderate relationship. 

![](images/OLS_Regression_Result1.png)

So, should we keep trusting the model? Even though the R square is not significant enough, I think the model that we create is still acceptable.

Beside, when we use score funcition to evaluate the R square, it gives us **0.46** which is a better result.

![](images/Score-result.png)

---

## IV. Discussion

When analyzing this model, it tells us something about the attribute that makes we survive:

- First: **Gender & Age** - it is actually commonsense. In every incident, woman, the young and the old is always priority. They are the group which are more likely to receive a lifeboat than the male and adult. It may also explain why the Age value in the model has the coefficent at only **0.07** as not only the young being priority but also the old. 

- Second: **PClass** - it highly recommends that if you book the higher class in a cuisine, it is more likely that you will survived. Perhaps, it happens as the higher class in a voyager is equipped with more emergency equipment that the individuals from lower class have more chance to access rescue transportation than the other people in different classes.

---

## V. Conclusion

- In the last, we want to disclaim that, there will be other models which have the capability to explain the data better than the model we use, but the linear model that we use can easily understand and analyze for most of people. 

- Another thing we want to discuss is that this incident is quite "specific", as there are many kinds of transportation accidents, plus Titanic happened along time ago so it might be a little out of date with the technology, mindset and culture today. 

But we highly believe that the attribute we chose which is sex, age and pclass in any era still have a big impact in the survival rate of a passenger.
