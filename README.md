# ml-04-Midterm-Project-Classification-Analysis

# SMS Spam Classification Midterm Project

## Overview

This repository contains my midterm project for an applied machine learning course.  
The goal is to build and evaluate classifiers that predict whether an SMS message is spam or ham using a combination of text features and engineered numeric features.

The work is organized and documented in a single Jupyter Notebook that follows the required sections

* import and inspect the data  
* explore and prepare the data  
* select and justify features  
* train and evaluate a baseline model  
* train alternate models and compare results  
* summarize findings and reflections  

## Repository structure

* `classification_albert_kabore.ipynb`  
  Main notebook with numbered sections and reflections for each section  

* `data/spam.csv`  
  SMS spam dataset used in the project  

* `peer_review.md`  
  Peer review of a classmate project as required for the assignment  

## Notebook and peer review

* Main notebook  
  [classification_albert_kabore.ipynb](classification_albert_kabore.ipynb)

* Peer review document  
  [peer_review.md](peer_review.md)

Both links are relative to the repository root and can be opened directly in GitHub or in a local Jupyter environment.

## Getting started

These instructions assume Python 3 is installed on your system.

### 1 Create and activate a virtual environment

From the repository root directory

On Windows in PowerShell

```powershell
python -m venv .venv
.venv\Scripts\Activate
```

## 2 Install required packages

With the virtual environment active run

pip install pandas numpy scikit-learn matplotlib seaborn wordcloud scipy


If you prefer you can export and share a separate requirements.txt and then run

pip install -r requirements.txt

Running the notebook locally

From the repository root with the virtual environment active

jupyter notebook


Then

In the Jupyter interface open classification_albert_kabore.ipynb

Run all cells from top to bottom

The notebook will

load and inspect the SMS dataset

explore distributions and create visualizations

clean and preprocess the text

engineer numeric features such as message length and word counts

convert text to TF IDF features

train a Random Forest model as the main classifier

train Logistic Regression and Decision Tree alternates

compare model performance using accuracy precision recall and F1 score

display a confusion matrix and feature importance for the Random Forest model

test the best model on several example messages

## Summary of models

The project evaluates three classifiers on the same train and test split

Random Forest

Logistic Regression

Decision Tree

Evaluation focuses on performance for the spam class using precision recall and F1 score because the dataset is imbalanced.
In this project the Random Forest model provides the best overall balance between detecting spam and limiting false alarms.

## Reflections and next steps

The notebook includes short reflections at the end of each section.
If the project were extended future work could include

more systematic hyperparameter tuning

cross validation

additional text feature engineering

experimentation with deep learning models for text

preparation of the model for simple deployment as a spam filter service
