# Sentiment-Analysis-using-Naive-Bayes-classifier

### Overview
This project performs sentiment analysis on a dataset of text reviews using the Naive Bayes classifier. The goal is to classify the reviews as positive or negative based on their content. The dataset consists of pre-labeled positive and negative reviews, where I apply text preprocessing techniques, followed by model training and evaluation.

### Dataset
The dataset is structured as follows:
- Train Set:
  - Positive reviews: ./Dataset/train/pos
  - Negative reviews: ./Dataset/train/neg
- Test Set:
  - Positive reviews: ./Dataset/test/pos
  - Negative reviews: ./Dataset/test/neg
  - Stop Words: A list of common stop words is provided in ./Dataset/stop_words.txt.
### Data Preprocessing
The raw text data undergoes several preprocessing steps to prepare it for model training:

- **Text Cleaning:**
  - Convert all text to lowercase.
  - Remove hyperlinks.
  - Remove punctuation marks.
  - Remove numerical characters.

- **Stop Words Removal:**
  - Stop words from the given list are removed from the text.


### Feature Extraction
We use the **Bag of Words (BoW)** approach to convert the cleaned text into a matrix of token counts using the `CountVectorizer` from `sklearn`.

### Model
We train the model using the **Multinomial Naive Bayes** algorithm:

- **Model:** `MultinomialNB()`
- **Training Data Size:** 25,000 reviews
- **Testing Data Size:** 25,000 reviews

### Results
The model's performance is evaluated using accuracy and a confusion matrix. The results are as follows:

- **Accuracy:** 82.43%

- **Confusion Matrix:**
    [[10992  2884]
    [ 1508  9616]]

### Skills
- **Programming Languages:**
  - Python
  
- **Libraries/Frameworks:**
  - Scikit-learn
  - NumPy
  - Pandas
  
- **Machine Learning:**
  - Naive Bayes Classifier
  - Natural Language Processing (NLP)

