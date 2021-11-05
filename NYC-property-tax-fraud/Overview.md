
## Statement of Problem
The property tax is the first income of the fiscal revenue, twice as much as the second source, personal income tax. Fraudulence in property tax cause large loss of fiscal revenue each year. The city of NY think there might be some property tax fraud going on their city and want to build an algorithmic system that can look through approximately 1 million property records to find potential tax fraud.

The potential tax fraud is defined as people underpaying tax or otherwise misrepresenting their property characteristics. The property tax is related to the prices of properties which reflect the conditions, locations and market expectations of a property.

To find out the potential fraudulence in property tax, the main purpose here is to find out the outliers in NYC property data. 
## Explore the data
The data is named as 'NY property data.csv', containing 1070994 records and 32 columns for each record.
Before preprocessing the dataset, it's necessary to understand the representation and distribution of each column thoroughly.
### Data Processing
#### Create Variables
#### Feature Selection
## Proposal
1. The relationships between characteristics could be non-linear, so Autoencoder could be considered as the main algorithms to find out the outlier.
2. 
3.
4.
## Algorithms
### Principal Component Analysis

### Autoencoder
Autoencoder is a special type of neural network that copies the input values to the output values and does not require the target variable thus categorized as unsupervised learning.
It has two process: Encoding and Decoding
#### Encoding
Process that extracts the essential information of the input values by reducing the number of neurons layer by layer. So the hidden core layer learned the most important pattern of the data and ignore the noises. 
#### Decoding
Process that reconstruct the information of core layer to produce the outcome without the noises.
## Future work
