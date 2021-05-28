# Term deposit marketing predicition and analysis
Marketing strategy have always been an interesting topic for me as it is considered a crucial tool to reach customers. And today in this data driven environemnt, marketing is even more complexe and interesting than ever before specially for someone who is passionate about data driven technology as myself.
This project represented an opportunity to learn and discover how data can actually contribute to the success of marketing campaigns and consequently the business's prosperity. 

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

The scikit-learn library provides multiple classification algorithms like logistic regression, decision trees, K-nearest neighbors and bagging techniques. So it's tricky to determine the right one off the bat without proper testing. Gridsearchcv the scikit-learn function offers a way to navigate through this problem. Basically it outputs the optimal hyperparameters that can gurantee the highest performance a model. It was intuitive to make the Gridsearchcv loop through a list of classification models as to tell which is the most suitable model.

![image](https://user-images.githubusercontent.com/60581207/120047155-3110de00-c014-11eb-9f5f-60030332aec4.png)

Random forest and XGBoost both proved to be the best models according to Gridsearchcv function, but i had to go with the Random forest for its simplicity and the shorter timetime it takes during the training process.

As i stated earlier, the main goal is to build a model that can **identify** potential depositors who are encoded as '1' in the output variable, that's why the **Recall** would be a more insightful metric to assess the model.

The classification report of The model indicated the following:

![image](https://user-images.githubusercontent.com/60581207/120049489-68828900-c01a-11eb-91a5-fcd4e512f492.png)

The recall of the positive class is considered low according to the picture above, it is imperative improve either by feature engineering techniques, feeding more data to the model or hyperparameters optimization.  



























