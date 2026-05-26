# 🐒 Capuchin Bird Audio Detection using Deep Learning

An end-to-end deep learning pipeline for detecting and counting **Capuchin bird calls** from forest audio recordings using **TensorFlow**, **Librosa**, and **CNN-based spectrogram classification**.

This project modernizes an older TensorFlow audio-classification workflow into a fully compatible **2026 Kaggle + Python 3.12 pipeline**.

---

# 📌 Project Overview

This system:

- Processes raw `.wav` forest recordings
- Converts audio into spectrograms
- Trains a Convolutional Neural Network (CNN)
- Detects Capuchin bird vocalizations
- Counts bird calls in long forest recordings
- Exports predictions into CSV format

---

# 🚀 Features

✅ Modern TensorFlow 2.16+ compatible  
✅ Kaggle 2026 compatible  
✅ Python 3.12 compatible  
✅ Sliding-window bird call detection  
✅ Spectrogram-based CNN classification  
✅ Forest recording inference pipeline  
✅ CSV export support  
✅ Removed deprecated `tensorflow-io` dependency  
✅ Uses `librosa` for robust audio preprocessing  

---

# 🧠 Deep Learning Pipeline

## Audio Processing
- Mono audio conversion
- Resampling to 16kHz
- Audio padding/truncation
- STFT spectrogram generation

## Model Architecture
- 3 Convolutional Layers
- MaxPooling Layers
- Dense Fully Connected Layer
- Dropout Regularization
- Binary Classification Output

---

# 📂 Dataset Structure

```bash
/kaggle/input/datasets/kenjee/z-by-hp-unlocked-challenge-3-signal-processing/

│
├── Forest Recordings/
├── Parsed_Capuchinbird_Clips/
└── Parsed_Not_Capuchinbird_Clips/
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

# 📊 Model Workflow

## 1️⃣ Audio Loading

Audio files are loaded using:

```python
librosa.load()
```

and resampled to:

```python
16 kHz
```

---

## 2️⃣ Spectrogram Generation

Short-Time Fourier Transform (STFT):

```python
tf.signal.stft()
```

creates frequency-domain representations of audio.

---

## 3️⃣ CNN Training

The model learns spectral patterns of:
- Capuchin bird calls
- Non-bird forest sounds

---

## 4️⃣ Sliding Window Detection

Long forest recordings are split into:

```python
3-second windows
```

Each window is independently classified.

---

## 5️⃣ Bird Call Counting

Predicted positive windows are counted to estimate:

```python
Number of Capuchin calls per recording
```

---

# 📈 Evaluation Metrics

The project supports:

- Accuracy
- Precision
- Recall
- Confusion Matrix

---

# 📄 CSV Output

Example output:

```csv
file_name,capuchin_calls
recording_1.wav,8
recording_2.wav,3
recording_3.wav,10
```

---

# ⚡ Key Modernization Fixes

The original tutorial used outdated components that failed in modern environments.

## Problems Fixed

❌ Broken `tensorflow-io`  
❌ Old TensorFlow 2.4 code  
❌ Deprecated Keras APIs  
❌ Incompatible Python 3.12 operations  
❌ Invalid Kaggle dataset paths  

## Modern Replacements

✅ `librosa` audio preprocessing  
✅ TensorFlow 2.16+ support  
✅ Modern Keras Sequential API  
✅ Stable TF Dataset pipelines  
✅ Dynamic preprocessing workflow  

---

# 📸 Results

## Training Accuracy
> *(Insert training accuracy screenshot here)*

## Spectrogram Visualization
> *(Insert spectrogram image here)*

## Confusion Matrix
> *(Insert confusion matrix here)*

---

# 🧪 Example Prediction

```python
forest_1.wav → 8 detections
forest_2.wav → 3 detections
forest_3.wav → 10 detections
```

---

# 💡 Future Improvements

- Transformer-based audio models
- Real-time bird call detection
- Multi-species classification
- Audio augmentation
- Mobile deployment
- Edge AI optimization

---

# 📚 Learning Outcomes

Through this project, concepts explored include:

- Audio Signal Processing
- Spectrogram Analysis
- Deep Learning for Audio
- TensorFlow Data Pipelines
- CNN-based Audio Classification
- Model Evaluation
- Real-world ML debugging

---

# 🙌 Acknowledgements

Dataset inspired by:
- Z by HP Unlocked Challenge
- Kaggle Audio Processing Community

---

# ⭐ If You Like This Project

Consider starring the repository and sharing feedback 🚀
