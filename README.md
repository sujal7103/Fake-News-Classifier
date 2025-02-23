# Fake_news_Classifier

# Data_set : - 
* True.csv : https://drive.google.com/file/d/16UuUit9yibFQ5m7BHGP67AA246pOZ9Qq/view?usp=sharing
* Fake.csv : https://drive.google.com/file/d/1wMGIkkWnE3rOLd4LzCDiVDC3rr7dmY2n/view?usp=sharing

# How to run: -
1. Download and Install Jupyter notebook.
2. Download ipynb and dataset file
3. Import the original  file in jupyter notebook and change the necessary dataset paths in the notebook.

# Project Description :- 
* Introduction
  * This project involves the detection of fake news using a dataset of real and fake news articles. The primary objective is to build a machine learning model that can accurately classify news articles as real or fake based on their content. This document outlines the various steps taken in the project, including data exploration, preprocessing, and model training.

* Data Exploration and Analysis
1. Dataset Overview:
   * The dataset comprises two CSV files: one for real news and one for fake news.
   * Each dataset contains columns such as title, text, subject, date, and target (label for classification).
2.Combining Datasets:
   * The real news articles were labeled with a target value of 1 and the fake news articles with a target value of 0.
   * Both datasets were concatenated and shuffled to ensure a random distribution.
3. Dataset Characteristics:
   * The combined dataset has 44,898 rows and 5 columns.
   * There are no missing values in the dataset.
   * The distribution of fake and real news articles is slightly imbalanced, with approximately 52% fake news and 48% real news.
4. Subject Analysis:
   * The dataset contains various subjects such as politics, world news, and US news.
   * Fake news articles are predominantly found under subjects like "News", "PoliticsNews", and "left-news".
   * Real news articles are mainly categorized under "PoliticsNews" and "worldnews".
* Visualization
1. Distribution of News Articles:
   * A bar chart was used to visualize the distribution of fake and real news articles across different subjects.
   * Pie charts were created to show the percentage distribution of different subjects in the dataset.
2. Year and Month Distribution:
   * The distribution of articles over different years and months was visualized using count plots.
   * This helped in understanding the temporal distribution of the news articles.
3. Title and Text Length Analysis:
   * The number of words in the title and text for both fake and real news articles was analyzed.  
   * Box plots revealed that fake news tends to have longer titles but shorter content compared to real news.
* Text Preprocessing
1. Text Cleaning:
   * All text data was converted to lowercase.
   * Special characters, URLs, HTML tags, punctuation, and digits were removed.
   * This cleaning process was applied to both the title and text columns, creating a combined column for analysis.
* Feature Extraction
1. TF-IDF Vectorization:
   * The cleaned text data was transformed into numerical features using TF-IDF vectorization.
   * This method converts text into a matrix of TF-IDF features, which are used for model training.
* Model Training and Evaluation
1. Initial Model:
   * A Naive Bayes classifier was trained on the TF-IDF features.
   * The model achieved an accuracy of approximately 95.6%.
2. Pipeline Creation:
   * A pipeline was created to streamline the process of vectorization and model training.
   * Three different models were tested: Logistic Regression, Decision Tree, and Random Forest.
3. Model Comparison:
   * Logistic Regression achieved an accuracy of 98.9%.
   * Decision Tree achieved an accuracy of 99.6%.
   * Random Forest achieved an accuracy of 99.3%.
   * A bar chart was created to visualize and compare the accuracies of these models.
* Conclusion
   * The project successfully demonstrated the detection of fake news using various machine learning models. The models achieved high accuracy, with the Decision Tree model performing the best. This comprehensive approach, from data exploration to model evaluation, provides a robust framework for fake news detection.

