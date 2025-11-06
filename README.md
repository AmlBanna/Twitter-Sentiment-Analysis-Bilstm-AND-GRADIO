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
### 📊 Dataset
The project uses the Twitter Sentiment Classification dataset with:

74,681 training samples

999 test samples

4 sentiment classes


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
## 🧪 Initial Experiment - v1-problem.ipynb

This file represents an **initial experiment** for Twitter sentiment analysis.  
In this early version, the model struggled to correctly classify negative tweets.  
To improve handling, emojis were **kept as part of the text** and **not removed** during preprocessing,  
and tweets labeled as "No" or "Not" were carefully treated.  
Additionally, **class imbalance was addressed** to enhance model performance.  
This experiment helped inform the preprocessing and modeling strategies for the final version.

You can check out the notebook [here](notebooks/v1-problem.ipynb).

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

## 📈 Results

### Confusion Matrix
![Confusion Matrix](MEDIA/Screenshot%202025-11-06%20080858.png)



## 🎥 Demo
[![Demo Video](MEDIA/Screen_Recording_2025_11_06_052612.gif)](MEDIA/Screen_Recording_2025_11_06_052612_V1.mp4)
### Video Demonstration
[Watch Demo Video](MEDIA/Screen_Recording_2025_11_06_052612_V1.mp4)


### Live Prediction Examples

| Tweet | Predicted Sentiment | Confidence |
|-------|-------------------|------------|
| "I love this new feature! 😍" | Positive | 98% |
| "This is terrible, worst experience ever 😠" | Negative | 96% |
| "The weather is okay today" | Neutral | 89% |
| "Buy now at 50% discount!" | Irrelevant | 92% |

---



## ⭐ Don't forget to star this repository if you find it helpful!
