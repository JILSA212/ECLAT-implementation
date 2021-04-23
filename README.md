# ECLAT-implementation
ML project submission on ECLAT algorithm for recommendation system <br> <br>

This project is mainly divided into two parts. <br> 
<ol>
    <li> Frequent itemset generation (ECLAT.ipynb) </li> <br>
    <li> Recommending items based on user input (ECLAT_result.ipynb) </li> <br> <br>
</ol>

**ECLAT.ipynb** <br>
<ul>
    <li> This file takes the raw data as an input which has transactionss rows. </li> <br>
    <li> It will fetch the data from data.csv file. </li> <br>
    <li> Some data cleaning tasks are performed. </li> <br>
    <li> Only 2 columns are used for itemset "InvoiceNo" and "Description". </li> <br>
    <li> Description is treated as name of the product here. </li> <br>
    <li> Threshold is set to 0.0005 as number of transactions is large. </li> <br>
    <li> Items with greater support (count) than min_support (no. of transactoins * threshold) </li> <br>
    <li> Frequent itemset is build using ECLAT algorithm. </li> <br>
    <li> We have used maximum 4 items together as frequent itemset. </li> <br>
    <li> Those items are listed and csv file is created called "new_data" </li> <br> <br>
</ul>

**ECLAT_result.ipynb** <br>
<ul>
    <li> This file uses the csv file created by ECLAT.ipynb. </li> <br>
    <li> It asks user to input the item they have purchased and it will recommend the item frequently bought with that. </li> <br>
