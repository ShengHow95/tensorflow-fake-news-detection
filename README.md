# FakeNewsDetection Overview

Contributors:
  1. Kong Sheng How
  2. Tan Li Mei
  3. Dr. Gan Keng Hoon
  4. Dr. Nur Hana Samsudin


Fake News Detection With NLP using Tensorflow Keras Simple Neural Network Model

Fake News Datasets can be obtained from:
  1. https://www.kaggle.com/jruvika/fake-news-detection
  2. https://www.kaggle.com/nopdev/real-and-fake-news-dataset

# Methodology

### Dataset CleanUp and Combination
1. Remove empty rows
2. Remove problematic rows (Some data points are problematic due to newlines ("\n") making the texts go into new rows)
3. Remove URL or ID columns

### Data Exploration
1. Dataset Ratio (Real News vs Fake News)
2. Word Cloud
3. Word Count in respective labelled dataset 

### Data Preprocessing
1. Text Preprocessing
  - Regular Expression (Remove punctuations and special characters)
  - Tokenization (Split texts into individual words)
  - Lemmatization (Turn words back to their root word)
  - Stop words removal (Remove stop words in texts)
  
  
2. Vectorization
  - N-Gram Vectors (TF-IDF Encoding)
  - Sequence Vectors (One-Hot Encoding)
  

### Model Training
1. Tensorflow Keras Neural Network Model (2 similar models created: 1 for N-Gram Vectors, 1 for Sequence Vectors)
  - Layer 1 (Input Dense): 64 nodes, RELU activation
  - Layer 2 (Dropout): 20% dropout
  - Layer 3 (Dense): 16 nodes, RELU activation
  - Layer 4 (Dropout): 20% dropout
  - Layer 5 (Dense): 8 nodes, RELU activation
  - Layer 6 (Dense): 2 nodes, Sigmoid activation 
  

### Model Evaluation
1. Comparison between 2 Tensorflow Keras Network Model (Using 3 different metrics)
  - Accuracy  
  - Recall   
  - Computational Time
  
