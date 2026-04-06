# 🎬 IMDB Sentiment Analysis using Simple RNN (Streamlit App)

This project is an end-to-end Deep Learning application that performs **Sentiment Analysis on IMDB movie reviews** using a **Simple Recurrent Neural Network (RNN)** and is deployed as an interactive **Streamlit web app**.

---

## 🚀 Project Overview

The goal of this project is to classify movie reviews as **Positive 😊** or **Negative 😡** by capturing sequential dependencies in text data using RNN.

---

## 🧠 Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Scikit-learn
- Streamlit

---

## 📊 Dataset

- Dataset: **IMDB Movie Reviews Dataset**
- Source: TensorFlow/Keras built-in dataset
- Vocabulary size: 10,000 words
- Preprocessing:
  - Integer encoding of words
  - Padding sequences to fixed length (500)

---

## ⚙️ Model Architecture

- Embedding Layer (Word Representation)
- SimpleRNN Layer (Captures sequence dependencies)
- Dense Layer with Sigmoid Activation (Binary Classification)

---

## 🏋️ Training Details

- Loss Function: Binary Crossentropy  
- Optimizer: Adam  
- Metrics: Accuracy  
- Callback: Early Stopping (to prevent overfitting)  

---

## 📁 Project Structure
SimpleRNN/
│── main.py # Streamlit app
│── simplernn.ipynb # Model training notebook
│── prediction.ipynb # Testing predictions
│── simple_rnn_imdb.h5 # Trained model
│── requirements.txt # Dependencies


---

## 🌐 Streamlit App Features

- User can input custom movie review text  
- Real-time sentiment prediction  
- Displays:
  - Sentiment (Positive/Negative)
  - Prediction Score (confidence)

---

## ▶️ How to Run Locally

```bash
# Create virtual environment
python -m venv venv

# Activate environment
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run main.py