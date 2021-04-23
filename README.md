# ECLAT-implementation
ML project submission on ECLAT algorithm for recommendation system

This project is mainly divided into two parts. 
    1. Frequent itemset generation (ECLAT.ipynb)
    2. Recommending items based on user input (ECLAT_result.ipynb)

ECLAT.ipynb
    This file takes the raw data as an input which has transactionss rows.
    It will fetch the data from data.csv file.
    Some data cleaning tasks are performed.
    Only 2 columns are used for itemset "InvoiceNo" and "Description".
    Description is treated as name of the product here.
    Threshold is set to 0.0005 as number of transactions is large.
    Items with greater support (count) than min_support (no. of transactoins * threshold)
    Frequent itemset is build using ECLAT algorithm.
    We have used maximum 4 items together as frequent itemset.
    Those items are listed and csv file is created called "new_data"

ECLAT_result.ipynb
    This file uses the csv file created by ECLAT.ipynb.
    It asks user to input the item they have purchased and it will recommend the item frequently bought with that.