# DSND - Sparkify Project to predict Customer Churn

### Project Motivation:
Sparkify is digial music streaming provider similar to other popular music streaming providers like Spotify or Pandora.
User can use Sparkify to play their favourite music either using free tier ( which has advertisemetns playing between songs ) or a paid subscription model. 

While users use Sparify to play their favourite music, different interactions which a user makes with Sparkify are captured as various events. 
Out of total users of Sparkify, some users do cancel their subscription ( called as Churn in this context) with Sparkify which means a possible business loss for Sparkify. And hence if there is a way to identify if a particular user is going to churn then an appropriate action can be initiated by Sparkify team to possibly avoid this churn and also avoiding potential business loss for Sparkify.

In this project, we would try to evaluate if there is a way to make a prediction (using machine learning) about if a user may churn in future by analysing past interactions of users with Sparkify.     

### Important Files:

dsnd-sparkify-project.ipynb : python3 notebook with code to perform EDA as well to build a predictive model to predict customer churn

### Results Summary:
As we compare results from 3 different models we understand that, both Random Forest as well as GBT models perform quite better than Logistic model when using F1-score for model performance evaluation. And GBT performing even slightly better than Random Forest model.

Considering the fact that we are able to get a considerably good f1-score with mini-dataset, we can expect to  improve on model performance even further when we train and test model on entire dataset in either AWS. 

Basis this, we choose GBT as final model to scale with full dataset. 
Another added advantage with GBT ( and even Random Forest ) is that it also gives us feature importance of each of attributes in predicting customer churn.

Read more here: https://medium.com/@shrirang16/customer-churn-prediction-with-pyspark-ec6557e60c98?source=friends_link&sk=fb068c2fc026c17a08237a5adb4018d5

### Requirements:
Since this notebook was run in IDE provided by Udacity which also had data present. hence we cannot run & execute this notebook as a standalone file.
This notebook uses following main libraries:
- pandas
- matplotlib
- seaborn
- pyspark