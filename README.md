# Data-Science-in-Python
Data Science Projects in Python


Project: Apriori Algorithm 
Objective:  
The purpose of the project is to write a program to generate all association rules whose support is greater 
than a user-supplied minimum support and whose confidence is greater than a user supplied minimum 
confidence. Implement all the steps of the Apriori algorithm.  
Program should take as a command line option for the five parameters in the following order: 
(i)  minimum support
(ii) minimum confidence
(iii) input file name
(iv) output name. 
The output name will be used to identify the output files from each run. 
When minconf=-1, do not generate rules. 

Input file format:
The input file, small.txt, consists of a set of lines, each line containing two numbers. The first number is the 
transaction ID, and the second number is the item ID. The lines in the file are ordered in increasing transaction 
ID order. Note that a transaction will be derived by combining the item IDs of all the lines that correspond to 
the same transaction ID. The input file is provided (small.txt).

Output file format:
Generate three different output files.  
1) <output_name>_items.txt: This output file will contain as many lines as the number of frequent 
itemsets, with their support count. The format of each line will be *exactly* as follows:  
ITEMSETS|SUPPORT_COUNT 
ITEMSETS will correspond to the items (space delimited). E.g., “item1 item2 item3|10”. 
Notice that there are no other spaces other than the ones that separate the items. 

2) <output_name>_rules.txt: This output file will contain as many lines as the number of high-confidence 
frequent rules that you found. The format of each line will be *exactly* as follows:  
LHS|RHS|SUPPORT|CONFIDENCE  
Both LHS and RHS will contain the items that make up the left- and right-hand side of the rule in a 
space-delimited fashion. E.g., “item1 item2|item3|0.2|0.3”. Notice that there are no other 
spaces other than the ones that separate the items. When minconf=-1, the file will not be generated. 
3) <output_name>_info.txt: This file will have a line for each piece of information. More specifically, it 
will need to include the following information: 
- minsup: 
- minconf: 
- input file: 
- output name:
- Number of items: 
- Number of transactions: 
- Number of frequent 1-itemsets: 
- Number of frequent 2-itemsets: 
- Number of frequent 𝑘 –itemsets: 
- Total number of frequent items: 
- The length 𝑘 of the largest 𝑘 -itemset: 
- The most frequent itemset:  
- Number of high confidence rules: 
- The rule with the highest confidence: 
- Time in seconds to find the frequent itemsets:  
- Time in seconds to find the confident rules:


Must know how to do the following: 
 Read input data, generate F_1 (frequent 1-itemsets), create output files, and plots. 
 Candidate itemset generation 
 Candidate pruning 
 Support counting with dictionaries (hash tables, i.e., create the dictionary and a function for the prefix tree of a transaction) 
 Candidate rule generation and elimination.
