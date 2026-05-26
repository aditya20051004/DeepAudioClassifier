# 🎙️ DeepFake Audio Detector

A deep learning-based audio classification system designed to detect AI-generated or manipulated audio using spectrogram analysis and Convolutional Neural Networks (CNNs).

This project uses modern TensorFlow + Librosa pipelines compatible with Kaggle 2026 and Python 3.12.

---

# 📌 Project Overview

This system:

- Processes `.wav` audio files
- Converts audio into spectrograms
- Trains a CNN model for classification
- Detects fake vs real audio
- Performs inference on unseen audio samples
- Exports predictions into CSV format

---

# 🚀 Features

✅ DeepFake audio detection  
✅ CNN-based spectrogram classification  
✅ TensorFlow 2.16+ compatible  
✅ Python 3.12 compatible  
✅ Kaggle-ready pipeline  
✅ Modern audio preprocessing using Librosa  
✅ CSV prediction export  
✅ Stable preprocessing without `tensorflow-io`  

---

# 🧠 Deep Learning Pipeline

## Audio Processing
- Mono conversion
- 16kHz resampling
- Audio normalization
- Padding/truncation
- Spectrogram generation

## Model Architecture
- Convolutional Neural Networks (CNN)
- MaxPooling layers
- Dense classification layers
- Dropout regularization
- Binary output layer

---

# 📂 Dataset Structure

```bash
dataset/

├── real_audio/
├── fake_audio/
└── test_audio/
```

---

# 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- Librosa
- NumPy
- Pandas
- Matplotlib
- Kaggle Notebooks

---

# 📊 Workflow

## 1️⃣ Audio Loading

```python
librosa.load()
```

Audio is converted into:
- mono channel
- 16kHz sample rate

---

## 2️⃣ Spectrogram Generation

Using:

```python
tf.signal.stft()
```

to transform audio into frequency-domain representations.

---

## 3️⃣ CNN Training

The CNN learns hidden frequency patterns between:
- Real human audio
- AI-generated / fake audio

---

## 4️⃣ Prediction Pipeline

The trained model predicts whether an audio sample is:

```python
0 → Real Audio
1 → Fake Audio
```

---

# 📈 Evaluation Metrics

The model supports evaluation using:

- Accuracy
- Precision
- Recall
- Confusion Matrix
- Validation Loss

---

# 📄 CSV Output

Example:

```csv
file_name,prediction
audio_1.wav,1
audio_2.wav,0
audio_3.wav,1
```

---

# ⚡ Modernization Fixes

This project modernizes older TensorFlow audio tutorials.

## Problems Fixed

❌ Broken `tensorflow-io`  
❌ Old TensorFlow 2.4 APIs  
❌ Deprecated Keras syntax  
❌ Python 3.12 incompatibilities  
❌ Legacy Kaggle notebook issues  

## Modern Replacements

✅ Librosa preprocessing  
✅ TensorFlow 2.16+ support  
✅ Modern Keras Sequential API  
✅ Stable TF Dataset pipelines  
✅ Dynamic preprocessing workflow  

---

# 📸 Results

## Training Accuracy
> *(Insert screenshot here)*

## Loss Curve
> *(Insert graph here)*

## Confusion Matrix
> *(Insert confusion matrix here)*

---

# 🧪 Example Predictions

```python
audio_1.wav → Fake
audio_2.wav → Real
audio_3.wav → Fake
```

---

# 💡 Future Improvements

- Transformer-based audio models
- Real-time fake audio detection
- Voice cloning detection
- Multi-class audio forgery detection
- Mobile deployment
- Edge AI optimization

---

# 📚 Learning Outcomes

Concepts explored in this project:

- Audio Signal Processing
- Spectrogram Analysis
- Deep Learning for Audio
- CNN-based Classification
- TensorFlow Data Pipelines
- Model Evaluation
- Real-world ML Debugging

---

# 🙌 Acknowledgements

Inspired by:
- Kaggle Audio ML Community
- TensorFlow Audio Processing Tutorials
- Modern DeepFake Detection Research

---

# ⭐ If You Like This Project

Consider starring the repository 🚀
