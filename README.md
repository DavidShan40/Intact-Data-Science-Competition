# CXC Datathon - Intact Data Science Challenge
# Description: https://devpost.com/software/m3-biubiubiu

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

## Solution

In this competition, our team successfully developed a document classification system that can automatically categorize medical transcriptions into their respective medical specialties. By implementing a range of machine learning models and leveraging state-of-the-art pre-trained models like BERT, we achieved a significant improvement in classification accuracy compared to the baseline.

### Model Performance
* Baseline Accuracy: 0.206
* Best Model Test Accuracy: 0.354
* Best Model macro-averaged F1-score: 0.110

The BERT model outperformed traditional classification models like Xgboost, SVM, and Rigid Classifier, with an accuracy of 0.354 on the test set. This result represents a considerable improvement over the baseline accuracy of 0.2.

### Key Takeaways
* The BERT model's superior performance highlights the importance of leveraging advanced pre-trained models in text classification tasks. By utilizing the knowledge gained from pre-training on a massive corpus of text, BERT is better equipped to understand and classify the medical transcriptions in our dataset.

* Our team's data exploration and preprocessing efforts played a crucial role in improving model performance. By thoroughly understanding the dataset and applying appropriate preprocessing techniques, we were able to feed cleaner and more meaningful input data into our models, ultimately leading to better classification results.

* The use of macro-averaged F1-score as the evaluation metric ensured that our models were evaluated fairly, taking into account the varying number of samples per class. This metric is particularly relevant in real-world applications, where imbalanced class distributions are common.

## Files

*   Code_final_submission.ipynb: Final submitted code for evaluation
*   BERT_2.ipynb: Pruning parameters such as epoch for BERT model
*   predictions.csv: submission solution
