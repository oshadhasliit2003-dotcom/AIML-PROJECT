# SuicideWatch-CNN: Suicide Detection using Text Classification

## Overview
This project focuses on **detecting suicidal intent from text data** using Natural Language Processing (NLP) and Machine Learning / Deep Learning techniques.

The goal of the project is **research and educational exploration** of text-based suicide detection, covering:
- data preprocessing
- multiple model training and comparison
- selection of the best-performing model
- deployment of the final model via Kaggle

⚠️ **This project is NOT a medical or clinical diagnostic system.**

---

## Dataset

The dataset used for this project is the **Suicide And Depression Detection**, originally published on Kaggle.

- **Original Dataset Link**:  
  https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch

Due to GitHub file size limitations, the dataset is **not included** in this repository.  
All credit for the dataset goes to the original author.

---

## Preprocessing Pipeline

The raw text data was cleaned and normalized using the following preprocessing steps:

1. **Lowercasing**  
2. **Punctuation Removal**  
3. **Stopword Removal**  
4. **Lemmatization**  
5. **Rare Word Removal**

---

## Models Trained

A total of **six models** were trained and evaluated:

### Classical Machine Learning Models
1. Logistic Regression  
2. Linear Support Vector Machine (SVM)

### Deep Learning Models
3. Artificial Neural Network (ANN)  
4. Convolutional Neural Network (CNN)  
5. Bidirectional LSTM (BiLSTM)  
6. Gated Recurrent Unit (GRU)

Each model was trained using the same preprocessed dataset to ensure fair comparison.

---

## Model Performance (Summary)

| Model | Approx. Accuracy |
|-----|------------------|
| Logistic Regression | ~0.9337 |
| Linear SVM | ~0.9323 |
| ANN | ~0.9373 |
| BiLSTM | ~0.9400 |
| GRU | ~0.9351 |
| **CNN (Tuned)** | **~0.9462 (Best)** |

> Accuracy values are approximate and may vary slightly depending on training conditions.

---

## Best Model: SuicideWatch-CNN

The **Convolutional Neural Network (CNN)** achieved the best overall performance after **hyperparameter tuning**.

---

## Pretrained Model (Kaggle)

Due to GitHub file size limits, the **final trained CNN model** is hosted on Kaggle.

- **Kaggle Model Link**:  
  https://www.kaggle.com/models/jayindukarunanayaka/suicide-detection

---

## Repository Structure

├── preprocessing/
│ ├── lowercasing.ipynb
│ ├── punctuation_removal.ipynb
│ ├── stopword_removal.ipynb
│ ├── lemmatization.ipynb
│ └── rare_word_removed.ipynb
│
├── models/
│ ├── logistic_regression.ipynb
│ ├── linear_svm.ipynb
│ ├── ann_model.ipynb
│ ├── cnn_model.ipynb
│ ├── BiLSTM_model.ipynb
│ └── GRU_model.ipynb
│
├── results/
│ └── preprocessing_visualizations/
│
├── README.md
└── LICENSE

## Ethical Considerations & Disclaimer

- This project is intended **strictly for research and educational purposes**
- The model **must not** be used for real-world mental health diagnosis or intervention
- Predictions should never replace professional medical or psychological support

If you or someone you know is struggling, please seek help from qualified mental health professionals or local support services.

---

## License

This project is licensed under the **Apache License 2.0**.  
You are free to use, modify, and distribute the code in accordance with the license terms.

---

## Author

**Jayindu Karunanayaka**  
Software Engineering / Machine Learning Enthusiast

---


