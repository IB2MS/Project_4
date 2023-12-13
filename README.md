# Sleep Efficiency Model and Analysis
Rutgers University Data Analysis Bootcamp
December 14, 2023
# Authors
Aditi Garg, Olesya Gaeva, Allison Potestio, Anusha Sekhar, Brendan Smith, Neha Changela, Susan Ombwayo
# Description
## Overview
In this project, we examine the Sleep Efficiency Dataset in order to learn more about factors that contribute to sleep efficiency. Sleep efficiency is a metric used to describe the quality of one's sleep, which is something that we feel is important for us to learn about. Improving one's sleep efficiency is something we feel that many people would be interested in learning more about. 

### Dataset and Research Questions
This project was built using dataset [Sleep Efficiency Updated](https://www.kaggle.com/datasets/ishhjain/sleep-efficiency-updated-dataset) sourced from Kaggle. 
This data set comprises 619 records with 15 columns listing participants' sleep data, including sleep efficiency and duration, as well as demographic (age, gender) and habitual information (caffeine intake, exercise frequency, smoking, alcohol consumption). 
This dataset leads us to question what effects the demographic and habitual factors included for each participant have on one's sleep efficiency. Do factors like age and gender affect sleep efficiency? We also took a look at those with high sleep efficiency and examined their habits. Do the best sleepers limit caffeine or alcohol intake? 
With this exercise, we are able to determine that these factors do affect sleep efficiency for these participants. 

### Data Preparation and Analysis 
This data was read into a jupyter notebook and cleaned using the pandas library





The data was then queried using Spark SQL so that we could learn more about our data and answer the following questions:
  

![image](https://github.com/IB2MS/Project_4/assets/135725909/a87fa97b-1953-419b-9f74-3341b8c206dc)


### Machine Learning Models
We created two machine learning models. Using the Tensor Flow model and the linear regression model, we are able to determine that the information in the columns has a strong impact on sleep efficiency.
#### TensorFlow
After splitting our cleaned dataset into training and testing data, we created a neural net model and used our testing data to determine the model's accuracy. 
On our first run, we were able to use days per week of alcohol consumption as a predictor for sleep efficiency with 87% accuracy

![image](https://github.com/IB2MS/Project_4/assets/135725909/e5e53152-2a40-41d1-9742-02ae51b6b483)

This process was repeated using caffeine consumption, smoking status, and exercise frequency to predict sleep efficiency. Due to the high accuracy of all models, we can determine that these factors affect sleep efficiency. 

#### Logistic Regression


### Tableau Visualizations
We used Tableau Desktop to find interesting takeaways from the data and to visualize comparisons between sleep efficiency and the other factors in our dataset. 

### Takeaways- Key Observations
  1. Like all datasets, outliers impacted our data analysis. For visualization purposes, with the exception of the Box Plot, we excluded outliers
  2. Our model had the best accuracy when run with maximum attributes as available in the data set
  3. Removing even a few rows containing null values had a high impact on the Model's efficiency.
  4. We found interesting trends while analyzing and visualizing the impact of habits on sleep efficiency by gender.
       For example, alcohol consumption and smoking affect sleep efficiency
  6. There are many different ways to achieve our goals - using what works best for the team allowed us to work well together

## Dependencies
Pandas, TensorFlow, Logistic Regression

