# CXC Datathon - Intact Data Science Challenge

## Background

*   Intact is Canada's largest P&C (property and casualty) insurer. We insure millions of homes, vehicles, and businesses domestically and international through our flagship brand and our subsidiaries.
*   At Intact, data is our competitive advantage. Data is the key to optimizing our prices, ensuring top customer satisfaction, and to getting the most out of our business processes.
*   The Data Lab is Intact's in-house Data Science shop, employing hundreds of actuaries, software engineers, and data scientists. Our goal is to develop and deploy data driven solutions to drive change across the organization.

## Description

*   Intact's claims department receives thousands of documents every day. Among these are medical documents, as Intact provides compensation to those who have sustained injuries in automobile accidents. Due to the volume of data received on a daily basis, it is difficult to keep every document neatly organized for easy retrieval. Thus, it would be helpful to have a system that automatically makes sense of the content of the document and can classify it into one of a set number of categories.

*   Our group classifies each medical transcription into a medical specialty

*   The evaluation is based on F1-score with macro averaging on the test set

## Methods

*   Data Exploration 
    * Plots for showing basic information in text words
*   Data Preprocessing
    * Preprocess the text words for better analysis
*   Data Modeling
    *   Split train/test sets for model comparison
    *   Normal Classification Models (Xgboost, SVM, Rigid Classifier)
    *   Pre-trained Model - BERT
    
# Files

*   Code_final_submission.ipynb: Final submitted code for evaluation
*   BERT_2.ipynb: Pruning parameters such as epoch for BERT model
*   predictions.csv: submission solution
