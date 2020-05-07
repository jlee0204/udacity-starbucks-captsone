Udacity Capstone Project 
===========================

## Project motivation

The project motivation is to create a analysis on the accessability of the Starbucks offers

Some of the quesitons answered include:


* What type of users are in this portfolio for starbucks?
* What type of models were the best at predicting if a customer would complete the offer?
* What were the type of variables important for predicting a customer completion.

## Getting Started

### Prerequisite Packages Used for Analysis

```
pip install numpy
pip install sklearn
pip install matplotlib
pip install pandas
pip install seaborn
pip install time
pip install json
```


### Data Files in Repository

```
Files:
```
```
portfolio.json

id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)
```

```
profile.json

age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income
```

```
transcript.json

event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record
```


### Summary of the results
- 

### Acknowledgements:
- Kaggle
- Udacity
