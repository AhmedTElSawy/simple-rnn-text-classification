# Simple RNN Text Classification

TensorFlow/Keras Recurrent Neural Network (RNN) for classifying text data.

## Overview
- **Dataset**: BBC News Articles (2,225 documents, 5 categories: business, entertainment, politics, sport, tech).
- **Model**: Recurrent Neural Network  
  Embedding → GlobalAveragePooling1D → Dense(24, ReLU) → Dense(6, Softmax).
- **Preprocessing**: Tokenization (vocab_size=1000), padding (max_length=120), stopwords removal.
- **Training**: Adam optimizer, sparse categorical cross-entropy loss, 30 epochs.
- **Results**: **Training accuracy ~99%**, validation accuracy **~92%** (shows good generalization).

## How to Run
1. Clone the repo: `git clone https://github.com/AhmedTElSawy/simple-rnn-text-classification.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Open and run the notebook: `jupyter notebook bbc-news-rnn.ipynb`

## Dependencies
- TensorFlow/Keras
- Numpy
- Matplotlib
- CSV
