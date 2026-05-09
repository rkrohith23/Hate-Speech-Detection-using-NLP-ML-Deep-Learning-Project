# Hate-Speech-Detection-using-NLP-ML-Deep-Learning-Project

##  Project Overview
This project focuses on detecting hate speech in social media text using Natural Language Processing (NLP), Deep Learning, and Transformer-based models. The study compares the performance of traditional machine learning approaches with advanced neural network architectures for binary hate speech classification.

The project implements and evaluates:
- TF-IDF + Logistic Regression
- Bidirectional LSTM (BiLSTM)
- DistilBERT Transformer Model



##  Objectives
- Detect hate speech in social media text
- Compare traditional ML, deep learning, and transformer models
- Handle class imbalance effectively
- Evaluate models using multiple performance metrics
- Build a real-time hate speech prediction system



#  Dataset Description
The dataset contains social media posts categorized into:
- Hate Speech
- Offensive Language
- Neutral Content

The original multiclass dataset was converted into binary classification:
- Hate Speech → 1
- Non-Hate Speech → 0



#  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Hugging Face Transformers
- NLTK
- PyTorch



#  Text Preprocessing
The following preprocessing techniques were applied:
- Lowercasing
- Removing punctuation
- Stopword removal
- Lemmatization
- Tokenization
- Sequence padding



#  Handling Class Imbalance
The dataset was highly imbalanced. To improve model performance:
- Minority class was oversampled
- Majority class was undersampled
- Balanced dataset was shuffled before training



#  Models Implemented

## 1️⃣ TF-IDF + Logistic Regression
Traditional machine learning baseline model using:
- TF-IDF vectorization
- Logistic Regression classifier
- N-gram features

### Advantages
- Fast training
- Interpretable
- Lightweight

### Limitations
- Cannot capture contextual meaning
- Limited sequential understanding



## 2️⃣ Bidirectional LSTM (BiLSTM)
Deep learning model capable of learning:
- Sequential dependencies
- Bidirectional contextual information
- Long-term relationships in text

### Architecture
- Embedding Layer
- Bidirectional LSTM
- Dense Layer
- Batch Normalization
- Dropout Layer
- Sigmoid Output Layer



## 3️⃣ DistilBERT
Transformer-based pretrained language model using:
- Attention mechanisms
- Context-aware embeddings
- Transfer learning

### Advantages
- Strong contextual understanding
- Excellent recall performance
- Handles semantic meaning effectively



#  Model Performance

| Model | Accuracy | Precision | Recall | F1-Score |
|------|------|------|------|------|
| TF-IDF + LR | 0.89 | 0.83 | 0.87 | 0.85 |
| BiLSTM | 0.97 | 0.97 | 0.96 | 0.96 |
| DistilBERT | 0.95 | 0.89 | 0.98 | 0.94 |



#  Model Comparison

A comparative evaluation was conducted across three models: TF-IDF with Logistic Regression, BiLSTM, and DistilBERT to analyse their effectiveness in hate speech detection.

The TF-IDF + Logistic Regression model achieved an accuracy of 0.89, providing a strong traditional machine learning baseline. However, the model struggles to capture contextual and sequential meaning because it treats text as independent tokens.

The BiLSTM model delivered the best overall performance, achieving an accuracy of 0.97 and the highest F1-score of 0.96. Its bidirectional sequential learning capability enables the model to effectively capture contextual relationships and long-term dependencies within text, making it highly reliable for hate speech classification.

DistilBERT achieved an accuracy of 0.95 with the highest recall of 0.98, demonstrating exceptional capability in identifying hate speech instances with minimal false negatives. This makes DistilBERT particularly suitable for safety-sensitive applications where detecting harmful content is prioritised.


#  Best Performing Model
BiLSTM achieved the best overall balanced performance across:
- Accuracy
- Precision
- Recall
- F1-Score

Therefore, BiLSTM is considered the most effective model in this study for hate speech detection.

---


