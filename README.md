<div align="center">

# 🎙️ Speech Emotion Recognition

**Recognise emotions from voice recordings using MFCC audio features and a recurrent neural network.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Librosa](https://img.shields.io/badge/Librosa-audio-informational)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?logo=googlecolab&logoColor=white)

</div>

---

## ✨ Overview

`Untitled1.ipynb` (built for Google Colab):

1. 📥 Downloads the **TESS - Toronto Emotional Speech Set** from Kaggle.
2. 📊 **EDA** - label distribution, waveform and spectrogram plots per emotion (Librosa).
3. 🎼 **Feature extraction** - 40 **MFCC** coefficients (mean over time) per 3-second clip.
4. 🧠 **Model** - a Keras `Sequential` recurrent network (LSTM / SimpleRNN, Dropout, BatchNormalization, Adam, EarlyStopping).

**Honest note:** in the recorded run the training accuracy approaches 99 % while validation accuracy stays low (~40 %), a sign of over-fitting. Ideas to improve: speaker-independent splits, data augmentation, regularisation and a CNN on mel-spectrograms.

## 🚀 Getting Started

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload your Kaggle API token (`kaggle.json`) when prompted.
3. Run all cells.

Local run:

```bash
git clone https://github.com/Arashomranpour/Emotion_detector_voice.git
cd Emotion_detector_voice
pip install librosa tensorflow keras scikit-learn pandas seaborn matplotlib kaggle jupyter
jupyter notebook Untitled1.ipynb
```

## 📁 Project Structure

```
.
└── Untitled1.ipynb
```

## 🛠️ Tech Stack

`Librosa` · `Keras / TensorFlow` · `scikit-learn` · `pandas` · `Seaborn`
