# KDD-Lab-2
By Kaanan Kharwa and Laura McGann
<br>
## Program Language Description
We decided to implement our program using python because it is the langauge that Google Colab uses. Using Google Colab allowed us to work on the code at the same time.
<br>
## Program Description
KDD_Lab_2.ipynb is the only source file in our zip and contains all the code needed to run Apriori's Algorithm and find the skyline and associations.
## Running the code 
The way to run the code is through the function outer_find_associations.

### Using outer_find_associations
outer_find_associations(csv_filepath, minRSup, minConf, ids_to_names, rules_and_itemsets=0b11)<br>
    csv_filepath - path to csv data file containing sparse vector representation of the data <br>
    minRSup - the min relative support value to use<br>
    minConf - the min confidence value to use<br>
    ids_to_names - a dictionary mapping ids (used in the dataset itself) to more descriptive item names<br>
    rules_and_itemsets - 1 to only print itemsets, 2 to only print association rules, 3 to print both (default)<br><br>
    
The dictionary ids_to_names must be provided by the user. A specific function to do this was not provided as the way the data is represented is not known to the parameter. For an example, in the Bakery dataset you have to combine two columns to get the full name where as in Fantasy Bingo this was not required.<br>

## File Paths
All file paths that were used by the programmers are in the code by default. There is a line commented out under these lines which can be uncommented and will allow the files to be read assuming that they are in the home directory.
<br>
## Potential Errors
Type of id in ids_to_names does not match type in dataset itself --> ids in dict should be strings not integers. <br>
Key not found error: itemset not sorted somehow
