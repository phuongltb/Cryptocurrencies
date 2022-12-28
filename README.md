# Cryptocurrencies
Create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment 

## Overview of the project
This project consists of the following:
  - Preprocessing the Data for PCA
  - Reducing Data Dimensions Using PCA
  - Clustering Cryptocurrencies Using K-means
  - Visualizing Cryptocurrencies Results

## Results
  - Preprocessing the Data for PCA: removed all cryptocurrencies that are not being traded, dropped the IsTrading column, removed all the rows that have at least one null value, removed all the rows that do not have coins being mined, and dropped the CoinName column. Below is the screenshot of the dataframe after being processing.
  
    ![image](https://user-images.githubusercontent.com/110554264/209747163-c7a79bfb-c19e-47d3-91f1-0ad291b2f044.png)
    
    A new DataFrame is created that stores all cryptocurrency names
    
    ![image](https://user-images.githubusercontent.com/110554264/209747331-10225e1d-a8d6-4034-a84c-d13c29861c7c.png)

  - Reducing Data Dimensions Using PCA: applied PCA to reduce the dimensions to three principal components and created a DataFrame with the three principal components.
  
    ![image](https://user-images.githubusercontent.com/110554264/209747532-9ae5d9e5-773b-4b45-8c90-05eeec63596c.png)

  - Clustering Cryptocurrencies Using K-means: created an elbow curve to find the best value for K, ran the K-means algorithm to make predictions of the K clusters for the cryptocurrencies’ data.
  
    ![image](https://user-images.githubusercontent.com/110554264/209747852-b263507b-3b4e-4581-9d17-0ee9dd8ffa5e.png)
  
    ![image](https://user-images.githubusercontent.com/110554264/209747662-d7931836-a3a0-4a3e-a64f-e99dad524ce1.png)

  - Visualizing Cryptocurrencies Results: created a 3D scatter plot using the Plotly Express scatter_3d() function to plot the three clusters, created a table with tradable cryptocurrencies, used the MinMaxScaler().fit_transform method to scale the TotalCoinSupply and TotalCoinsMined columns between the given range of zero and one, and created an hvplot scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class", and have it show the CoinName when you hover over the the data point.
  
    ![image](https://user-images.githubusercontent.com/110554264/209747950-d24696a7-84f6-4389-87e5-cc4d73178be6.png)

    ![image](https://user-images.githubusercontent.com/110554264/209747992-6fc4f207-77d3-4a42-9908-96728046d966.png)

    ![image](https://user-images.githubusercontent.com/110554264/209748012-78fb9333-89c2-445d-9b0b-7463b60738f0.png)


    
