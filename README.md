# HR Promote Analysis

This is the HR datasets. In our dataset 50000 rows and 14 columns. Every year, around 5% of its employees have promoted in the company. So, I have to know, employee is promoted or not?

## Code and Resources Used
Python Version: 3.7

Packages: pandas, numpy, sklearn, matplotlib, seaborn

I got this datasets from Kaggle.com, thanks for Shivan Kumar. It was divided for test and train by Shivan Kumar. This dataset have CC0: Public Domain license.

Dataset link on Kaggle.com: https://www.kaggle.com/shivan118/hranalysis

Shivan Kumar link on Kaggle.com: https://www.kaggle.com/shivan118

## Goals and objectives
My goal to predict: who will be promoted?

To do this I should do next things:

To clean our data

To make exploratory data analysis

To prepare our data for Machine Learning

To build and upgrade our Machine Learning model


## Exploratory Data Analysis

I explored how did our features distribute, how they work together. For more you can look at my EDA part, there are a lot of graph, which is intesting and helpful. They helped we to understand, how our data works. Below you can see most important graphs.

The following conclusions can be drawn from our explanatory data analysis:

  - We have a strong relations between rating and promotions, average training score and promotions and etc.
  - There are a lot of outliers, which we should clean before model building.
  - We need one more feature, in my opinion it should be one productivity feature, because there are a lot of disparate features, which we couldn't express in one, such as KPI,     rating and training score.

For the greatest illustration, I’ll show you some graphs that are most important.

First of all it is worth paying attention to correlation matrix, it is clear which factors are closely related to promotion of the employee.
![Сorrelation Matrix](/graphs/сorr_map.png)

Another important indicator is average training score, it is important to us and this we can see on the graph. Staff with the highest scores are promoted, after some limit (above 90 points) people are promoted with almost 100% probability
![Training score promotion](/graphs/training_score_promotion.png)


But beyond that, we have another measure of efficiency, which is the human rating of the past year. And the graph below shows how the average score, age and progression are related. As we can see from the people who get promoted, the average rating is above 3.5.
![Age_Rating](/graphs/age_rating.png)

## Data Preprocessing

In this part I cleaned data, prepare it for model building and etc. This is the list of things, that I have done.

1. Remove NaN values
2. Handling outliers
3. Remove extra features
4. Transform categorical variable to quantitative
5. Create new features
  a. Start of the career in company
  b. etc.
6. Feature scaling

## Model Building

In this part of the project I have to built models, that will predict, who will be promoted. My goal was to promote right employees, so in this case accuracy and precision was my priority. 

I choosed five perspective models, which could help us. After test review, I stopped on two most effective model:
1. Random Forest Classification
2. XGBoost Classification

## Model Perfomance

After model tuning, I got next results:

1. Random Forest Classification

  Accuracy score: 0.9377850757161103
  
  Precision score: 0.9346153846153846
  
2. XGBoost Classification:

 Accuracy score: 0.9464513774858603
 
 Precision score: 0.883054892601432
