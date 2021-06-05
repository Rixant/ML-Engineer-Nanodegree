# Proposal

## Domain Background
This is the proposal for Starbucks Capstone project for Machine Learning Engineer Nanodegree. Nowadays every company has their own app to sell their products. Starbucks is one of them who uses their app to market their products and interact with their customers. Starbucks sends out an offer to their mobile users as a part of rewards program every week inorder to retain and attract the customers. The offers may vary upon users and some users might not recieve any kind of offers for certain weeks.An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO. It uses it mobile app to make online orders, analyze customer behavioursa and predict wait time. 

## Problem Statement
The purpose of the project is to prepare a suitable Machine Learning Model to predict the users response to offers and rewards program provided by Starbucks. We will analyze the users interaction with offers through offers recieved, offers viewed, offers expired, transaction and offers completed to improve marketing strategy to targetted users and increase the overall profit. 

The model will use binary classification and  datasets used in this project is already provided by udacity.

## Datasets and Inputs
The data is contained in three files:\
portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)\
profile.json - demographic data for each customer\
transcript.json - records for transactions, offers received, offers viewed, and offers completed\

***Schema and explaination of variables:***

**portfolio.json**\
id (string) - offer id\
offer_type (string) - type of offer ie BOGO, discount, informational\
difficulty (int) - minimum required spend to complete an offer\
reward (int) - reward given for completing an offer\
duration (int) - time for offer to be open, in days\
channels (list of strings)

**profile.json**\
age (int) - age of the customer
became_member_on (int) - date when customer created an app account\
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)\
id (str) - customer id\
income (float) - customer's income

**transcript.json**\
event (str) - record description (ie transaction, offer received, offer viewed, etc.)\
person (str) - customer id\
time (int) - time in hours since start of test. The data begins at time t=0\
value - (dict of strings) - either an offer id or transaction amount depending on the record\

## Solution Statement
The solution of this project will be achieved using the following steps given below:
1. **Data Preprocessing** - remove missing and duplicate values, data normalization, data type conversion and correcting the errors.
2. **Data Exploration** - data visualization, determine interdependencies and distribution of data, split data into training and test set
3. **Build a Model** - Appropriate machine learning model will be built. Logistic Regression, XGBoost, SVM are the few options that we can try.
4. **Model Evaluation** - accuracy and f1 metrics will be used to evaluated model performance.

## Benchmark Model

## Evaluation Metrics

## Project Design
