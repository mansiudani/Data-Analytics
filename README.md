# Predicting the likelihood of success for Start up Companies  
Introduction : 
All startups begin with a great idea which with time turns into a great hypothesis. Most of the innovators and entrepreneurs attempt to establish a business which leads to failure. Entrepreneurs understand the key factors involved in creating a successful company are skill, idea, knowledge, market scenario but the most important factor is funds. There are different kinds of funds like Seed funding, Angel investors, Silent investors and many more. Our work here is to predict if the startup status which is operating, acquired or closed.

Data Collection:
The startup crunch investments database is collect from Kaggle. The dataset comprises of 54294 rows and 39 columns. The dataset contains information of all the funding sources and their types.

Data Cleaning:
The dataset comprises of 54,294 rows and 39 columns. Intensive cleaning is required to the data ready for analysis. First, a stripping of spaces is done for column names. These spaces could cause errors while calling through a column name. Second, for the status attribute. This column is our dependent variables, so the null values are deleted. Then the attribute is converted to integers which help in the plotting of the correlation heat map. A plot to show the missing data is generated. Third, fundings obtained from separate sources are placed to 13 separate columns. Here, all the fundings are summed up in a single row [total_fundings]. Fourth, after summing the fundings in a single row, the funding channels (13) are deleted. Fifth, the date of the last updated column is split into two columns of year and month. Sixth, the columns which are of low significance to the analysis are dropped like: Founded_month, founded_quarter and many more. Seventh, again missing data plot is generated.

Data Selection and Transformation:
Performing a thorough cleaning of the dataset, 37,564 rows and 13 columns are left which will be further used for analysis. The aim is to develop a model to identify the status of the company. The dataset specifically has 4 ordinal target variables which indicate the status of the company. The target variables are 1: acquired, 2: operating and 3: closed. To fulfil our purpose, one hot encoding is performed, which means converting the categorical variable into integer or numeric. Applying this sort ML algorithm would enhance the success rate of predicting the status and also eliminate errors. A unique integer is applied to each variable and a new column is created (Status).

Training and Testing Data :
For the application of machine learning algorithms, splitting the preprocessed data into training and testing tests by 75% and 25% respectively. Next step involves constructing a model on the training data using data mining models.

Methodology:

A Naive Bayes classifier assumes that the presence (or absence) of a particular feature of a class is unrelated to the presence (or absence) of any other feature. Depending on the precise nature of the probability model, naive Bayes classifiers can be trained very efficiently in a supervised learning setting. In many practical applications, parameter estimation for naive Bayes models uses the method of maximum likelihood. This algorithm is a bad fit for the dataset.
Support Vector Machine is a supervised learning method which defines a separating hyperplane of the data. The algorithm takes in labelled training data and an optimal hyperplane comes out as an output. The objective is to find a hyperplane which distinctly points out all the data points. This algorithm can work best for the share market dataset as the probability of an event is easily adjusted as and when new data is introduced. SVM proves to be a good fit for this dataset.

Results:
I predicted the status of the company along with the funds factor and types. I applied SVM which proved to be a good fit, whereas Naïve Bayes was typically a bad fit. As for the future work of the startup investments, more factors can be considered and predicted on the basic factors like location, employees, growth rate and much more.



