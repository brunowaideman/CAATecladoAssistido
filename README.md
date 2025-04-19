# 👁️‍🗨️ AUGMENTATIVE AND ALTERNATIVE COMMUNICATION USING EYE TRACKING AND WORD RECOMMENDATION USING LANGUAGE MODELS

## 🧠 Overview

This project aims to develop an **assistive virtual keyboard** that uses **eye-tracking** technology for text input. It is especially designed for users with **motor disabilities**, enabling them to interact with a computer using only **eye movements**.

The system consists of three main stages:

1. 🎯 **Data Collection**: Gathers eye gaze data while the user selects characters on the screen using a traditional input method.
2. 🧪 **Model Training**: Trains a machine learning model to predict the selected character based on the eye data.
3. 💬 **Virtual Keyboard Interaction**: Allows typing using only the eyes through a virtual keyboard interface powered by the trained model.

Additionally, it includes:
- 📚 An **N-gram Language Model** to enhance typing prediction.
- 📉 A **Perplexity Analysis** tool to evaluate prediction accuracy.

---

## 🗂️ Project Structure

| File | Description |
|------|-------------|
| `1_collect_data.ipynb` | Captures eye movement data during typing. |
| `2_train_model.ipynb` | Trains a classification model using collected data. |
| `3_eyetracker.ipynb` | Virtual keyboard interface using the eye-tracking model. |
| `EyeTrackerEyeChimera.ipynb` | Alternative version using the EyeChimera API. |
| `Ngram.ipynb` | Builds the N-gram language model. |
| `perplexity.ipynb` | Calculates perplexity to evaluate language model accuracy. |

---

## ⚙️ Requirements

- 🐍 Python ≥ 3.8  
- 📦 [OpenCV](https://opencv.org/)  
- 📦 [Dlib](http://dlib.net/)  
- 📦 [Scikit-learn](https://scikit-learn.org/)  
- 📦 Pandas  
- 📦 NumPy  
- 📊 Matplotlib

---

## 🚀 How to Run

1. Run `1_collect_data.ipynb` to collect training data.
2. Run `2_train_model.ipynb` to train the eye-gaze prediction model.
3. Run `3_eyetracker.ipynb` to interact with the assistive virtual keyboard.
4. Optionally, run `Ngram.ipynb` and `perplexity.ipynb` to improve and evaluate typing predictions.

---

## 📝 License

This project is licensed under the **MIT License**.
