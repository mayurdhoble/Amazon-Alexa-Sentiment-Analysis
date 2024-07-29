# Amazon Alexa Sentiment Analysis :
This project implements a sentiment analysis application using Flask to classify Amazon Alexa reviews as positive or negative. The backend utilizes machine learning techniques with Natural Language Processing (NLP) for text pre-processing and classification.

Libraries Used :

1) pandas: Data manipulation

2) re: Regular expressions for HTML tag removal

3) nltk: Natural Language Toolkit for text processing
   
5) stopwords: Provides a list of common English stop words
   
7) PorterStemmer: Reduces words to their root form (stemming)
   
9) word_tokenize: Tokenizes text into individual words
    
11) scikit-learn: Machine learning library
    
13) CountVectorizer: Converts text data into numerical feature vectors
    
15) SVC: Support Vector Classifier for sentiment classification
    
17) Flask: Web framework for building web applications

## Text Preprocessing with NLTK :

The sentiment analysis pipeline involves pre-processing the text data from Amazon Alexa reviews before feeding it into the machine learning model. This pre-processing improves the accuracy and efficiency of the model.

Here's an overview of the steps:

HTML Tag Removal: Regular expressions are used to remove any HTML tags present in the review text.

Tokenization: Words are separated into individual tokens.

Lowercasing: All words are converted to lowercase for case-insensitive processing.

Stop Word Removal: Stop words (e.g., "the", "a", "is") are removed as they don't contribute significantly to sentiment.

Stemming: Words are reduced to their base form (stem) using Porter Stemmer.

After performing these steps, the text data becomes cleaner and more suitable for machine learning algorithms.

# CountVectorizer :

## CountVectorizer is a key NLP technique used to convert textual data into numerical feature vectors.

It works by:

Vocabulary Building: It analyzes the training data and creates a vocabulary of the most frequent words.

Feature Vector Creation: For each review, it counts the occurrences of each word in the vocabulary and represents the review as a vector of these counts. This allows the machine learning model to learn relationships between words and sentiment.

This process allows the model to work with numerical data, which is essential for many machine learning algorithms.

Flask App:

The Flask application provides a user interface for sentiment analysis. Users can enter an Alexa review, and the model predicts its sentiment (positive or negative) based on the pre-processed text features.
