# Amazon Product Reviews Analysis

## Data Source
- [Amazon Product Reviews Dataset](https://www.kaggle.com/datasets/yasserh/amazon-product-reviews-dataset)
- Folder: Amazon

## Description
The dataset consists of samples from Amazon Ratings for select products. The reviews are randomly picked, and the corpus has nearly 1.6k reviews from different customers. The goal is to understand the main topics of these reviews for easier classification.

### Tasks
1. **Data Cleanup, Analysis, Visualization, and Modeling**
   - Understand the Dataset and perform necessary cleanup.
   - Add additional algorithms to go in-depth on the positivity of each review.
   - Build a strong Topic Modelling Algorithm to classify topics beyond what is provided in each review's title.
   - Create a regression model to predict product ratings based on the length of reviews.

2. **Libraries and Tools Used**
   - Pandas (data cleaning and manipulation)
   - NLTK & spaCy (NLP)
   - scikit-learn (regression)
   - langdetect & googletrans (detecting non-English languages and translating to English)
   - Gensim (topic modeling)
   - pyLDAvis & matplotlib (visualizing topic model)
   - warnings (prevent certain warnings from showing up and display personal information on the user's device after cell execution)

## Usage Instructions
### Possible Errors:
1. **Missing Libraries:** Ensure all Python libraries are installed on your machine or within your directory.
2. **Cell Edits:** Avoid making problematic edits to the cells. This notebook is designed to run seamlessly with no manual edits.
3. **Python Kernel:** Ensure you are running a Python kernel or use an up-to-date version.
4. **Library Downloads:** Some libraries or necessary downloads may be required for the operation of certain parts or the entirety of certain libraries. For example, vader_lexicon is required to be downloaded for Sentiment Analysis (later in the notebook).

### Execution
1. Execute the following initial setup code:
    ```python
    import pandas as pd
    from pandas.errors import SettingWithCopyWarning
    from sklearn.linear_model import LinearRegression
    import nltk
    import warnings

    # warnings.filterwarnings("ignore")  # ignore all overall
    warnings.filterwarnings("ignore", category=SettingWithCopyWarning)  # ignore a warning later on for copying over on a dataframe.
    warnings.filterwarnings("ignore", category=FutureWarning)

    df = pd.read_csv('product_reviews.csv')
    df.head()
    ```

2. Continue executing subsequent cells to perform data cleaning, analysis, visualization, and modeling.

### Relevant Columns
- `id`, `asins`, `brand`, `categories`, `colors`, `manufacturer`, `name`, `prices`, `reviews.date`, `reviews.doRecommend`, `reviews.numHelpful`, `reviews.rating`, `reviews.text`, `reviews.title`, `sizes`, `weight`.

3. After cleaning the data, sentiment analysis, and creating positivity scores, the notebook proceeds to topic modeling using NLP techniques.

4. **Visualization of Main Topics**
   - The notebook utilizes pyLDAvis to visualize the clusters of topics obtained from the reviews.

5. **Main Topics Identified**
   - 1: Device and Display Experience
   - 2: Audio and Speaker Performance
   - 3: Headphones and Sound Quality
   - 4: Content Consumption and App/Software Experience
   - 5: General Product Review and Comparison
   - 6: TV Box and Streaming Experience

Feel free to explore and adapt the notebook for your specific needs.

