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

### Methodology and Insights
- Preprocessing was done to remove any informational that was not available. 
- The offers included variations of bogo, discount, and informational offers. Most of the analysis was completed based on the aggregate data set as well as monetary discounts such as bogo and discount.
- Most of the variables had low correlation and was not revmoed for the initial modeling. Informational offers had the largest negative correlation to the offer being completed.

### Summary of the results
- We analyzed the different datasets to predict the probablity to predict a user ability to complete an offer. In doing this, we ran a set of models to find the best fit. 
- While looking at the feature importance we have noticed that the year that the user joined (tenure) and the amount of the reward was a huge factor in determining if the user would complete the offer.
- In running logistic regression, LDA, KNN, CART, NB, and SVM, we notices that in all models the logistic regression had theb highest average accuracy when running the data in 10 split folds. In addition to this, we found that the All in one model including all of the offers such as bogo and discount had a marginally better accuracy than the bogo and discount model. 



### Future Refinement and Challenges
- Currently the data is based on a small set off of offers listed in this database. Due to this there is a limited amount of factors that are being tested. For future evaluations, it'll be interesting to see a larger set of variables that may potentially impact. 
- Since there are some nuances with the data currently, the modeling was done on users that have received the coupon and does not currently include users that have not received information of the coupon.

### Blog:
- https://medium.com/@jaemo.lee0204/how-to-tell-if-your-promotion-works-a-starbucks-story-a6e853576d2e

### Acknowledgements:
- Kaggle
- Udacity
