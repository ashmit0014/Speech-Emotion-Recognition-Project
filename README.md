# Speech Emotion Recognition using CNN and RAVDESS Dataset

This project implements a Speech Emotion Recognition (SER) system using deep learning. The model is trained to identify emotions from audio recordings using the **RAVDESS dataset**. It utilizes **Convolutional Neural Networks (CNNs)** with extracted audio features like **MFCCs (Mel-frequency cepstral coefficients)** for emotion classification.

---

## Project Overview

Speech Emotion Recognition (SER) is the task of identifying human emotions from speech signals. Unlike speech recognition, SER focuses on *how* something is said rather than *what* is said. This has applications in virtual assistants, customer service analytics, and mental health monitoring.

---

## Dataset

- **Name**: RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
- **Source**: [Official RAVDESS on Kaggle](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio)
- **Classes**: Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, Surprised
- **Format**: 735 speech audio files from 24 speakers (16-bit WAV, 48kHz)

---

## Features Extracted

The following audio features were extracted using Librosa:

- MFCCs (Mel-Frequency Cepstral Coefficients)
- Chroma
- Spectral Contrast
- Tonnetz
- Zero-Crossing Rate
- Root Mean Square Energy

---

## Model Architecture

A Convolutional Neural Network (CNN) was built using Keras:

- 1D Convolutional Layers with ReLU activation
- Batch Normalization
- MaxPooling layers
- Dropout for regularization
- Dense layers for classification
- Softmax activation in the output layer

---
