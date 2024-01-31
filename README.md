# Amazon Product Reviews Analysis

## Overview

This project focuses on the analysis, data cleaning, and visualization of an Amazon Product Reviews dataset. The primary objectives include:

1. **Understanding the Dataset**: Perform necessary cleanup and exploration of the Amazon Product Reviews dataset.

2. **Sentiment Analysis**: Apply Natural Language Processing (NLP) and Sentiment Analysis to understand the positivity of each review.

3. **Topic Modeling**: Develop a strong Topic Modeling Algorithm to classify the topics within each review.

4. **Regression Analysis**: Create a regression model to predict product ratings based on the length of reviews.

## Data Source

- [Amazon Product Reviews Dataset](https://www.kaggle.com/datasets/yasserh/amazon-product-reviews-dataset)
- Folder: Amazon

## Tools and Libraries Used

- Pandas
- NLTK (Natural Language Toolkit)
- scikit-learn (for regression analysis)
- langdetect & googletrans (for detecting and translating non-English languages)

## Jupyter Notebook Structure

### 1. Data Loading and Initial Exploration

- Importing necessary libraries.
- Loading the dataset and examining the columns.
- Selecting relevant columns for analysis.

### 2. Data Cleaning

- Restructuring columns like 'prices' and 'reviews.date'.
- Handling date formats.
- Extracting relevant information from the 'prices' column.

### 3. Sentiment Analysis

- Utilizing NLTK's SentimentIntensityAnalyzer to determine the positivity of each review.
- Handling non-English reviews by detecting and translating them.

### 4. Topic Modeling

- Exploring NLTK's product_reviews_2 dataset for topic modeling.
- Applying tokenization and exploring sample reviews.

### 5. Regression Analysis

- Building a regression model to predict product ratings based on the length of reviews.

### 6. Visualization and Conclusion

- Visualizing insights obtained from the analysis.
- Drawing conclusions and highlighting key findings.

## Usage Instructions

1. Install the required Python libraries mentioned in the notebook.
2. Ensure a compatible Python environment.
3. Run the notebook cells sequentially.

**Note**: Be cautious about the potential need for library installations and compatibility issues. The dataset path may need adjustment based on your directory structure.

Feel free to explore and modify the notebook for your specific analysis needs. If any issues arise, refer to the error handling instructions provided in the notebook.
