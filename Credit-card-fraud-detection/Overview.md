
## Statement of Problem
## Propose
+ Build real time predictive algorithms
  1. Build variables using all the data
  2. Separate the Out of Time data and put it away till the end
  3. Split the rest of data into training and testing dataset to build the best model, including bootstrap, bagging and cross validation
  4. Test the model on OOT data after finalizing it
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
