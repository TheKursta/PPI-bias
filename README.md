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
 
# Script execution order
First pre-processing script has to launched, which will convert .seq and .txt files from Dataset 2 into .csv files that .ipnyb will be able to read-in.
Then .ipnyb files can be launched, which contain step-by-step explanation and will print out the necessary results and save additional .csv files.

# Script Description
Dataset_x_analysis.ipnyb analyzes the PPI dataset, by:
- Showing distribution of interacting/non-interacting pairs
- Plotting histogram of interactions for each proteins
- Plotting histogram of non-interactions for each protein
- Plotting histogram of ratio of interaction and non-interaction for each protein.
- Splits data into training and test set.
- Dummy classifier estimates probability of test pair interaction on training data and predicts interaction/non-interaction.
- Dummy accuracy is calculated.
- Sequences are converted into 100-dimensional vectors using Prot2Vec (Word2Vec) NLP model.
- Siamese Neural Network (NN) is fit on training data and performance is estimated on test data.
- Impact of bias is estimated through calculating corellation between NN probabilities and Dummy probabilities.

