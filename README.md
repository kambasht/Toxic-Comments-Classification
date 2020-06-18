# Classifying Toxic comments on social networking sites

Analyzing toxic comments on social media to help prevent toxicity, obscenity and threats.

# Table of Contents
1. Project Motivation
2. Project Tasks
3. File Descriptions
4. Running the code
5. Results
6. Licensing, Authors, and Acknowledgements

## Project Motivation 

Cyberbullying is a form of harassment using electronic means. With the advent of modern day technology, it is becoming increasingly common for people to interact on social platforms and inadvertently engage in cyber bullying, especially among teenagers. Harmful bullying behaviour ranges from spreading rumors, toxic comments, threats, identity hate, misinformation and hate speech.

Victims of cyberbulling may experience lower self-esteem, increased suicidal ideation, and a variety of negative emotional responses including being scared, frustrated, angry, or depressed. Between 20% and 40% of adolescents are victims of cyberbullying worldwide.The youth slowly change their behaviors and actions so they become more withdrawn and quiet, but this may go unnoticed since the change is subtle.

The project motivation is derived from a Kaggle based [dataset] (https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data) released by The Conversation AI team, a research initiative founded by Jigsaw and Google (both a part of Alphabet) who are working on tools to help improve online conversation with platforms like [Perspective](https://perspectiveapi.com/#/home) . Based on a labelled dataset of toxic and non-toxic comments from Wikipedia, we plan to model our response to pre-emptively and actively keep cyber bullying at bay.

Our task will be to train a model on detecting toxicity, identity hate and threat and consequently using them to actively mark and review toxic comments on social platforms.

## Project Tasks

I. Exploratory Data Analysis

Exploring the data to find patterns and dive into the details of the provided dataset

II. Data Cleaning and Merge

The raw data needs to be cleaned up and transformed to prepare it for analysis. We use data cleaning and transformation method to help derive a merged database for analysis

III. Observations and Recommendations

We look at specific words in the comments to help us identify hate and threats.

IV. Data Modeling and Prediction

We compare a NaiveBayes, a Logistic Regression and a Linear SVC model to help predict which comments fall into the category of toxicity.

V. Conclusion

Discussion on which model performs better and why.

## File Descriptions

The data is contained in three files:

train.csv

test.csv

### train.csv

the training set, contains comments with their binary labels

### test.csv

the test set, you must predict the toxicity probabilities for these comments. To deter hand labeling, the test set contains some comments which are not included in scoring.


## Running the code

Installations required before running the code:
- no external libraries are required for installation

Folder structure:
- Place the method file 'method.py', data files and the jupyter notebook from the repo into a single folder and then run the notebook

## Results

Based on our analysis of the model, the LinearSVC model is able to perform most efficiently in terms of training time and the ROC AUC Score. One of the reasons LinearSVC works better than Logistic Regression because LinearSVC tries to finds the “best” margin (distance between the line and the support vectors) that separates the classes and this reduces the risk of error on the data, while logistic regression does not, instead it can have different decision boundaries with different weights that are near the optimal point.

SVM works well with unstructured and semi-structured data like text and images while logistic regression works with already identified independent variables. SVM is based on geometrical properties of the data while logistic regression is based on statistical approaches

The main findings of the code can be found at a post available 

## Licensing, Authors, Acknowledgements

Credits to [Wikipedia] (https://en.wikipedia.org/wiki/Cyberbullying)

Credits to [Kaggle] (https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data) for the dataset

Knowledge credits:
https://medium.com/axum-labs/logistic-regression-vs-support-vector-machines-svm-c335610a3d16

https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html
