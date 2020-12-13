# PPI-bias
This is the repository for course project. 

# Setup
First the requirements.txt file has to be installed, that contains all the necessary libraries for python code.
Secondly be sure that powerful PC is used (32GB RAM and 6 core CPU at least, >GTX1080 GPU), scripts are quite resource consuming.

# Additional files
First datasets and Prot2Vec models have to be downloaded:
 - Dataset 1 from [article](https://academic.oup.com/bioinformatics/article/35/14/i305/5529260) [repository](https://github.com/muhaochen/seq_ppi).
 - Dataset 2 from this article [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3531800/]. train_11.txt; test_11.txt
 - Prot2Vec model from [article](https://arxiv.org/pdf/1503.05140v1.pdf) [repository](https://github.com/kyu999/biovec).
 
# Script order
First pre-processing script has to launched, which will convert .seq and .txt files from Dataset 2 into .csv files that .ipnyb will be able to read-in.
Then .ipnyb files can be launched, which contain step-by-step explanation and will print out the necessary results and save additional .csv files.

# Script Description
Description of scripts and what and how they do is inside the .ipnyb files.
