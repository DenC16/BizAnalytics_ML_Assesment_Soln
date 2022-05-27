# Spam Classification
Training a spam classifier on the Apache SpamAssassin datasets.

## Overview
I used the [Apache SpamAssassin public data](https://spamassassin.apache.org/old/publiccorpus/) to train a few classification models and picked the one with the best precision and recall. To run this project,these are dependencies required (see below).

## Steps Involved
- Download and understand the data format
- Handling the imbalance and Splitting the data into training and test sets
- Prepare the data:
  - Remove email headers
  - Lowercase the email body
  - Convert urls to the word 'URL'
  - Convert numbers to the word 'NUM'
  - Remove punctuation
  - Convert the resulting text to bag-of-words representation
- Train and evaluate a few models on recall, precision and ROC:
  - MLP
  - Decision Tree
  - Random Forest
  - AdaBoost
  - KNN
  - SVM classifier
- Fine-tune the best classifiers (MLP, AdaBoost and Random Forest)
- Evaluate on the test set

## Best Model
The best classifier is the MLP classifier with about:
- 99.1% accuracy
- 100% precision
- 98.2% recall
- 99.09% f1-score

## Models Link

Given below is where models are stored in pkl form :
<https://drive.google.com/drive/folders/106VCuoeaGhn0-wP-kgONbIqtQ7BM-3Ex?usp=sharing>

## Libraries Used :
- Numpy 
- Scipy 
- Scikit-Learn
- Matplotlib 
- Joblib 
- Urllib
- Shutil
- Os
- Glob
- Re
- Warnings

## Setup Instructions

### Global setup

  Download and install Git
  git config --global user.email EMAIL_ADDRESS
  
### Next steps

  mkdir email_spam_classification
  cd email_spam_classification
  git init
  touch README
  git add README
  git commit -m 'first commit'
  git remote add origin 
  git push origin master
  
You may also want to track the master branch for easy pull/push
<ul>
  <li>git config branch.master.merge refs/heads/master</li>
  <li>git config branch.master.remote origin</li>
</ul>

## Execution Intructions

You can clone this repository in your local system by using the following command.
git clone <https://github.com/DenC16/BizAnaytics-ML--Assesment-Solution>

Once the repository is installed, you can run the Jupyter Notebook through the Anaconda3 Jupyter Notebook Environment.

