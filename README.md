# Twitter Sentiment Analysis using BiLSTM

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)](https://tensorflow.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/yourusername/twitter-sentiment-analysis.svg)](https://github.com/yourusername/twitter-sentiment-analysis/stargazers)

A deep learning project for sentiment analysis on Twitter data using **Bidirectional LSTM (BiLSTM)** neural networks, achieving **95% accuracy** in sentiment classification.

---

## 📊 Project Overview

This project implements a robust sentiment analysis system that classifies Twitter posts into four categories:

- 😊 Positive  
- 😔 Negative  
- 😐 Neutral  
- ❌ Irrelevant  

---

## 🎯 Key Features

- **Bidirectional LSTM Architecture** for superior sequence understanding  
- **95% Accuracy** on test dataset  
- **Comprehensive Text Preprocessing** with NLTK  
- **Class Imbalance Handling** using SMOTE  
- **Real-time Sentiment Prediction**  
- **Model Visualization** and performance metrics  

---

## 🚀 Quick Start

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/twitter-sentiment-analysis.git
cd twitter-sentiment-analysis

```
### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the Jupyter notebook:
```bash

jupyter notebook notebooks/twitter-sentiment-analysis-bilstm-acc-95.ipynb

```



## 📈 Results

### Confusion Matrix
![Confusion Matrix](docs/demo_images/confusion_matrix.png)

### Training History
![Training History](docs/demo_images/training_history.png)

---

## 🎥 Demo

### Video Demonstration
[![Demo Video](docs/demo_images/video_thumbnail.png)](docs/demo_videos/demo.mp4)  
*Click the image above to watch the full demo video*

### Live Prediction Examples

| Tweet | Predicted Sentiment | Confidence |
|-------|-------------------|------------|
| "I love this new feature! 😍" | Positive | 98% |
| "This is terrible, worst experience ever 😠" | Negative | 96% |
| "The weather is okay today" | Neutral | 89% |
| "Buy now at 50% discount!" | Irrelevant | 92% |

---

## 🔧 Technical Details

### Model Architecture
- **Embedding Layer**: 100 dimensions  
- **Bidirectional LSTM**: 128 units  
- **Dense Layers**: 64, 32 units with Dropout  
- **Output Layer**: 4 units (Softmax)  

### Data Preprocessing
- Text cleaning and normalization  
- Tokenization with NLTK  
- Stop words removal  
- Lemmatization  
- Sequence padding  
