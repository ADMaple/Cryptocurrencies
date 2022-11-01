# Cryptocurrencies Analysis

## Overview

The purpose of this analysis is to report what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for the Advisory Services Team at Accountability Accounting, a prominent investment bank.  The data will need to be processed to fit the unsupervised machine learning models to group the cryptocurrencies, using a clustering algorithm. 

Deliverable 1: Preprocessing the Data for Principal Component Analysis (PCA) algorithm

Deliverable 2: Reducing Data Dimensions Using PCA

Deliverable 3: Clustering Cryptocurrencies Using K-means

Deliverable 4: Visualizing Cryptocurrencies Results


## Resources
 
 -Data Source: crypto_data.csv
 
 -Software and Data Tools: Juptyer Notebook, Python, Sklearn, Pandas, and Unsupervised Machine Learning
 
 ## Analysis and Results of Data
 
After cleaning the data to remove All cryptocurrencies that are not being traded, dropping the IsTrading column, remove all the rows that have at least one null value, remove all the rows that do not have coins being mined, dropping the CoinName column, removing null values and filtering it for the required information, a PCA model was crafted using 3 principal components. That information was then used to create a elbow curve to identify the best value for k. The diagram is as follows:
 
 ![Elbow_Curve](https://user-images.githubusercontent.com/108022219/198353166-88a2a1c9-8458-4f3b-bdbb-92af3a11f1cb.png)
 
 A new DataFrame was created that stores all cryptocurrency names from the CoinName column and retains the index from the DataFrame.
 
 ![New_df](https://user-images.githubusercontent.com/108022219/198353908-888b3bcd-9d41-47d8-8ee1-553fe8b6708b.png)

By applying the Principal Component Analysis (PCA) algorithm, the dimensions of the X DataFrame was reduced to three principal components then placed in a new DataFrame.
 
![D2_3df](https://user-images.githubusercontent.com/108022219/198355700-e66b01f0-a5ce-44b8-860c-8a09c8758fd7.png)

After using the K-means algorithm to create an elbow curve using hvPlot to find the best value for K. 

![Elbow_Curve](https://user-images.githubusercontent.com/108022219/198353166-88a2a1c9-8458-4f3b-bdbb-92af3a11f1cb.png)

The K-means algorithm is then used to make predictions of the K clusters for the cryptocurrencies by creating a new dataframe. 
Using Plotly Express and hvplot to create a scatter plot, and create a table with tradable cryptocurrencies.

![Scatter](https://user-images.githubusercontent.com/108022219/198359499-c330d0db-05e7-45d8-a7de-027ad5195d34.png)

![3D_Cluster](https://user-images.githubusercontent.com/108022219/198359591-67b58ae8-8688-40c4-a528-16d7eb6823ce.png)

![Tradeable_Crypto](https://user-images.githubusercontent.com/108022219/198357278-8a100bde-3127-4766-9a6b-b9ac62a7d372.png)

 ## Summary
 
After creating the report that includes and specific cryptocurrencies that are on the trading market, grouped to create a classification system for Accountability Accounting, this new cryptocurrency investment portfolio would prove benefitical for its customers. 
 
