# Term deposit marketing predicition and analysis
I decided to go through with this project after checking the dataset and it made me think of how much of an interesting project this would be as it pushes me to cover multiple aspects
of data science and statistics in general.

The dataset's source: https://www.kaggle.com/janiobachmann/bank-marketing-dataset

#### -- Project Status: Completed

## Project Intro/Objective

The aim of this project is to identify customers who are more inclined into making a deposit. The data source provides over 16 personal details about contacted indivduals and their response to the possibility of making a deposit with a yes/no response
I divided the project into 2 notebooks:
* EDA and inferential statistics where i explore the data, extract insights and determine how features influence the outcome. 
notebook's link : https://github.com/HakimFerch/Marketing-Data-analysis-and-ML-classififcation/blob/master/Exploratory%20and%20Inferential%20data%20analysis.ipynb

* Feature engineering, model selection, implementing the classifcation model and optimizing the model to improve accuracy.
notebook's link :https://github.com/HakimFerch/Marketing-Data-analysis-and-ML-classififcation/blob/master/Classification%20model.ipynb

### Methods Used

* Descriptive statistics
* Inferential Statistics
* Statistical modelling
* Feature Engineering
* Machine Learning
* Data Visualization
* Hyperparameter Optimization
* Resamling Techniques
* Marketing Strategy

### Technologies

* Python
* Pandas, jupyter
* Matplotlib,Seaborn
* Scikit-learn 
* numpy
* Hyperopt
* Statsmodels

## Project Overview

For banking and financial institutions, deposits represent a major souce of income to give loans and make profits off of interest rates, therefore banks usually invest in advertisement campaigns using differen outreach to reach 
to attract potential depositors.

In our case of study the bank used **telephonic marketing**, one of the most common and effective strategies to collect data, and in many cases call centers are hired to implement these kind of surveys. 
Finally, the collected data could be used in the training of a high accuracy model would be tremendously beneficial as it helps to identify potential customers and consequently improve the bank's number of depositors.

The dataset consists of 16 features and a binary ouput variable
![image](https://user-images.githubusercontent.com/60581207/119861551-d003e000-bf17-11eb-9a9d-fde85de606df.png)

### Exploratory and inferential Analysis
 
 The porject starts with exploratory data analysis to understand the general layout of the data, discover anomalies and hidden patterns that can provide valuable details.I tried to showcase the insights i uncovered using graphs for a more compelling representation of the data with barchats, distribution plots, correlation heatmaps and boxplots.
 
 ![image](https://user-images.githubusercontent.com/60581207/119907190-065d5180-bf50-11eb-8008-158f19be87b9.png) ![image](https://user-images.githubusercontent.com/60581207/119907465-a31fef00-bf50-11eb-83d9-df7166247318.png)
![image](https://user-images.githubusercontent.com/60581207/119907834-791afc80-bf51-11eb-862f-c79e579bd5b8.png)



 Next comes the inferential statistics section where i try to estimate differences between groups using statistical tests such as :
* T-tests 
* analysis of variance (ANOVA)
* Chi-squared tests
* CRAMER's V test

Moreover, i determine the confidence intervals with alpha=0.05 of different variables means specially the ones with the highest correlation with our target variable.
![image](https://user-images.githubusercontent.com/60581207/119908866-db74fc80-bf53-11eb-99fb-46cc8e83b4cb.png)

### Machine learning Classification model:

The problem is to build a model which classifies individuals into potential depositors and not, hence the necessity to choose the most fitting classification model available.

But before diving into the model selection phase, it is imperative to go through preprocessing.Data should be transformed and scaleed for a better functioning model. 
Our data contains multiple categorical string type features that need encoding and numerical data that has to be scaled or mormalized depending on the case.

The scikit-learn library provides multiple classification algorithms like logistic regression, decision trees, K-nearest neighbors and bagging techniques. So it's tricky to determine the right one off the bat without proper testing. Gridsearchcv the scikit-learn function offers a way to navigate through this problem. Basically it outputs the optimal hyperparameters that can gurantee the highest performance a model. It was intuitive to make the Gridsearchcv loop through a list of classification models as to tell which is the most suitableate model.
























