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

Here we can see the distribution of age groups among our clients. It is very important because the largest age group (18-29) buys a small number of insurers, as compared to the other in percentage.
![Age_Groups](/graphs/age_groups.png)

Annual premium had many emissions that we eliminated in the next step, but after elimination we can see the normal distribution. As we can see, the number of people paying less than 10,000 is enough, so we need to work on that later. But that’s another task.
![Annual_Premium](/graphs/annual_premium.png)


Vintage is the number of days a customer has spent with the company. As we can see, people usually stop buying our insurance for 100 and 200 days.
![Vintage](/graphs/vintage_response.png)

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
