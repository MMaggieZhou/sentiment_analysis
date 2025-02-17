# [Sentiment Classificatin](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/twitter_entity_sentiment_analysis_v2.ipynb)
## Data 
medium size data from [kaggle](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis/data)

## Techniques 
### Preprocessing 
- Data Cleaning
  - To Lower Case
  - unicode normalization
  - special characters removal 
- Text Processing
  - Stop-word Removal
  - Lemmatization
  - Tf-idf Tokenization
  - Text Embedding
  - Sentence Embedding
- Categorical Data Processing
  - One-Hot Cncoding
  - Label Encoding 

### Training 
- Logistic Regression
- Support Vector Machine (With Linear Kernel) - LinearSVC
- BERT with AdamW optimizer

### Evaluation 
- Accuracy
- Confusion Metric
- AUC-ROC
- F1, Precision, Recall 

### Library
- Panda
- sklearn
- spaCy
- matplotlib
- torch
- transformers
- sentence_transformers
## Pretrained Models 
- bert-base-uncased
- all-MiniLM-L6-v2
  
## Results Comparison 
| Setup    | Accuracy | AUC-ROC | F1 Score | Precision | Recall |
| -------- | -------- | ------- | -------- | --------- | ------ |
| (CPU) [Tf-idf + Logistic Regression](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_tfidf.ipynb)  | 0.90   | | 0.90 | 0.90 | 0.90 |
| (CPU) [Tf-idf + SVM](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_tfidf.ipynb)  | 0.94    | | 0.94 | 0.94 | 0.94|
| (GPU) [sentence embedding (sbert) + Logistic Regression](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_sbert_embedding.ipynb) | 0.62 |  | 0.62 | 0.62 | 0.62|
| (GPU) [sentence embedding (sbert) + SVM](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_sbert_embedding.ipynb) | 0.62 | | 0.61 | 0.62 | 0.62|
| (GPU) [bert embedding + Logistic Regression](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_bert_embedding.ipynb) | 0.60| | 0.59 | 0.60 | 0.60 | 
| (GPU) [bert embedding + SVM](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_bert_embedding.ipynb) | 0.60| | 0.59 | 0.60 | 0.60|
| (GPU) [finetune pretrained bert model](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/sentiment_analysis_bert_finetune.ipynb) | 0.97| | 0.97 | 0.97 | 0.97|


# [Topic Modeling](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/topic_modeling.ipynb)
## preprocessing 
- Bad of Words (BOW)

## Training 
- Latent Dirichlet Allocation (LDA)

## Topic Summarization 
- Prompt Engineering
  
## Library 
- gensim
- pyLDAvis
- nltk
- openai

# [Topic Meling with BERTopic + OpenAI ](https://github.com/MMaggieZhou/sentiment_analysis/blob/main/bertopic%2Bchatgpt.ipynb)
## preprocessing 
- Data Cleaning
  - To Lower Case
  - unicode normalization
  - special characters removal
## Training 
- BERTopic
  
## Topic Summarization 
- Prompt Engineering

## Library
- bertopic
- hdbscan
- openai

## References 
- [DL foundation](https://docs.google.com/document/d/1-srAw0XsSiD_-CdzYtD-2r4Y7on-4JySuE-qp7GY6Io) 

# [Exploratory Data Analysis](http://localhost:8888/lab/tree/sentiment_analysis/eda_tweets.ipynb)
## Data Clearning and Processing 
- Duplicate Data
- Empty Data
- Ordinal Encoding for Categorical Data 
## Data Distribution 
- Imbalanced Data
### Numerical Data 
- AVG, MAX, Mean, Percentile, std
### Text Data 
- Text Length Distribution 
- Ngram: 
- Visualizatin: wordcloud, histogram 
### Categorical Data 
- Label Distribution
- Visualization: pie chart
## Covariance Analysis
- Pearson Correlation Coefficient
- Visualization: heatmap
## Library 
- sklean
- scipy
- nltk
- matplotlib
- wordcloud
- seaborn
