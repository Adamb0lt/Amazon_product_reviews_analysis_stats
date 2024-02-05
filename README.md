# Amazon Product Reviews Analysis

## Data Source
[Amazon Product Reviews Dataset](https://www.kaggle.com/datasets/yasserh/amazon-product-reviews-dataset)

## Folder
Amazon

## Description
The dataset contains samples from Amazon Ratings for select products. The reviews are randomly selected, comprising nearly 1.6k reviews from different customers. The goal is to understand the main topics of these reviews for easier search and classification.

### Objectives
1. **Data Cleanup and Exploration**
   - Understand the dataset and perform necessary cleanup.
   - Select relevant columns for analysis.

2. **Analysis and Visualization**
   - Explore the dataset using Pandas for cleaning and manipulation.
   - Utilize NLTK, spaCy, and sklearn for natural language processing (NLP) and sentiment analysis.
   - Implement a regression model to predict the helpfulness of reviews based on their length.

3. **Topic Modeling**
   - Use Gensim for topic modeling to identify the main topics of reviews.
   - Visualize topic clusters using pyLDAvis.

4. **Additional Algorithms**
   - Implement algorithms to gauge the positivity of each review.
   - Create a classification model to classify the level of positivity.

5. **Tools Used**
   - Pandas for data cleaning and manipulation.
   - NLTK & spaCy for NLP.
   - sklearn for regression.
   - Gensim for topic modeling.
   - pyLDAvis & matplotlib for visualizing topic models.
   - langdetect & googletrans for detecting non-English languages and translation.
   - warnings for managing warnings during execution.

### Instructions for Running the Notebook
- Ensure all required Python libraries are installed.
- Make sure to run the notebook sequentially without making any edits.
- Some cells may require additional downloads (e.g., NLTK resources) during execution.
- Check for errors related to missing libraries or dependencies.

### Columns in the Dataset
- **id:** Unique identifier for each product.
- **asins:** ASIN (Amazon Standard Identification Number) associated with the product.
- **brand:** Brand of the product.
- **categories:** Categories to which the product belongs.
- **colors:** Colors available for the product.
- **dateAdded:** Date when the product was added.
- **dateUpdated:** Date when the product information was last updated.
- **dimension:** Dimensions of the product.
- **ean:** EAN (European Article Number) associated with the product.
- **keys:** Unique keys associated with the product.
- **manufacturer:** Manufacturer of the product.
- **manufacturerNumber:** Manufacturer number for the product.
- **name:** Name of the product.
- **prices:** Prices associated with the product, including currency and date information.
- **reviews.date:** Date when the review was posted.
- **reviews.doRecommend:** Indicates whether the reviewer recommends the product.
- **reviews.numHelpful:** Number of users who found the review helpful.
- **reviews.rating:** Rating given by the reviewer.
- **reviews.sourceURLs:** URLs to the source of the reviews.
- **reviews.text:** Text content of the review.
- **reviews.title:** Title of the review.
- **reviews.userCity:** City of the reviewer.
- **reviews.userProvince:** Province of the reviewer.
- **reviews.username:** Username of the reviewer.
- **sizes:** Sizes available for the product.
- **upc:** UPC (Universal Product Code) associated with the product.
- **weight:** Weight of the product.

### Data Cleaning
1. Selected relevant columns for analysis.
2. Restructured the prices column.
3. Converted the reviews.date column to datetime format.

### NLP and Sentiment Analysis
1. Used NLTK and spaCy for natural language processing.
2. Employed sentiment intensity analysis to determine the positivity of each review.
3. Classified reviews into different positivity levels.

### Topic Modeling
1. Tokenized and lemmatized the text for better topic modeling.
2. Applied bigrams and trigrams to the data.
3. Created a bag-of-words representation and developed a dictionary.
4. Implemented LDA (Latent Dirichlet Allocation) for topic modeling.
5. Visualized the topics using pyLDAvis.

### Regression Model
1. Explored the relationship between review length and helpfulness.
2. Implemented a polynomial regression model for prediction.

### Conclusion
The notebook provides comprehensive insights into the Amazon product reviews dataset, covering data cleaning, sentiment analysis, topic modeling, and regression analysis. Users are encouraged to run the notebook sequentially and ensure all dependencies are installed for a seamless execution.
