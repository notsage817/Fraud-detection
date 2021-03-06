
## Statement of Problem
Credit card fraud has been a huge problem as everthing becomes digital. The total credit card outstanding loans in the U.S. are about $2.4 trillion dollars per year and the loss could be $24 billion dollars if the true fraudulent rate is only one percent!

There are basically two types in credit card fraud: application fraud and transaction fraud. The former is similar to identity fraud that one person uses another person's personal data to obtain a new card. Transaction fraud happens when a card is stolen or a lost card is obtained to conduct fraudulent transactions. 

A fraudster will try to abuse the card as much as possible in a short period of time before the card is detected and suspended. So abnormal transactions happend in a short period of time. The main purpose to catch transaction fraud is to catch abnormal trsansactions similar to:
+ Burst of activity at different merchants or increased usage in card-not present
+ Larger than normal purchase amounts
+ Used at merchants not used before for that card or high-risk merchant
+ Used at a very different geography (state)
+ Employee or merchant invents transactions or a fictitious merchant
+ Infrequent recurring charges, same amount or same merchant
## Propose
+ Build real time predictive algorithms
  1. Build variables using all the data
  2. Separate the Out of Time data and put it away till the end
  3. Split the rest of data into training and testing dataset to build the best model, including bootstrap, bagging and cross validation
  4. Test the model on OOT data after finalizing it
+ Feature Engineering
  1. Fraud detection features could be created by **RFM principle**
    + Recency - How recently did the customer purchase - Time passed since last purchase
      Days passed with same (card/merchant/card at the merchant/card in the zip code/card in the state) since last purchase
    + Frequency - How often do they purchase - Total number of transactions
      Number of transactions with this (card/merchant/card at the merchant/card in the zip code/card in the state) over the past (0/1/3/7/14/30) days
    + Monetary - How much do they spend - Amount of transactions
      (Average/maximum/median/total) amount &(ratio of actual amount to (Average/maximum/median/total) amount) at (card/merchant/card at the merchant/card in the zip code/card in the state) over the past (0/1/3/7/14/30) days
  2. Besides, there shoule be velocity change variables
    + The (number/amount) of transactions with same (card/merchant) over the past (0/1) days
    + Average daily (number/amount) of transactions with same (card/merchant) over the past (7/14/30) days

## Data Preprocessing

## Algorithms
### Random Forest
### Support Vector Machine
### Neuron Network
### XG Boost
## Performance Measurement
Assume $2000 gain for each caught fraud and $50 loss for each false positive. As the subpopulations get larger, the fraud detection rate gets larger but the increment of detection rate gets smaller.  
+ Score all records and sort records by descending order
+ Examine subpopulations(top 1%, 2%, 3%..etc) and calculate the %frauds caught in each subpopulations
+ Build fraud detection rate plot and define score cutoff where the profit of fraud detection reach the top
