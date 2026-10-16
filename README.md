SuicideWatch-CNN: Suicide Detection Using Text Classification

 Overview

This project focuses on **detecting suicidal intent from text data** using Natural Language Processing (NLP) and Machine Learning / Deep Learning techniques.

The goal of this project is **strictly for educational purposes and academic research** into text-based suicide detection, covering:

- data preprocessing
- training and comparing multiple models
- selecting the best-performing model
- deploying the final trained model via Kaggle

⚠️ **EDUCATIONAL PURPOSES ONLY. This project is NOT a medical or clinical diagnostic system and must not be used for real-world mental health diagnosis or intervention.**



 Dataset

The dataset used for this project is the **Suicide And Depression Detection** dataset, originally published on Kaggle.

Original Dataset Link:  
  [https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch](https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch)

Due to GitHub file size limitations, the dataset is **not included** in this repository.

All credit for the dataset goes to the original author.



 Preprocessing Pipeline

The raw text data was cleaned and normalized using the following preprocessing steps:

1. Lowercasing
2. Punctuation Removal
3. Stopword Removal
4. Lemmatization
5. Rare Word Removal



 Models Trained

A total of **six models** were trained and evaluated.

 Classical Machine Learning Models

1. Logistic Regression
2. Linear Support Vector Machine (SVM)

 Deep Learning Models

3. Artificial Neural Network (ANN)
4. Convolutional Neural Network (CNN)
5. Bidirectional Long Short-Term Memory (BiLSTM)
6. Gated Recurrent Unit (GRU)

Each model was trained using the same preprocessed dataset to support a fair comparison of model performance.



 Model Performance (Summary)

| **Model** | **Approx. Accuracy** |
|---|---:|
| Logistic Regression | ~0.9337 |
| Linear SVM | ~0.9323 |
| ANN | ~0.9373 |
| BiLSTM | ~0.9400 |
| GRU | ~0.9351 |
| **CNN (Tuned)** | **~0.9462 (Best)** |

> Accuracy values are approximate and may vary slightly depending on training conditions and model configurations.



 Best Model: SuicideWatch-CNN

The **Convolutional Neural Network (CNN)** achieved the best overall performance after **hyperparameter tuning**, reaching an approximate accuracy of **0.9462 (94.62%)**.

Based on the experimental results, the tuned CNN was selected as the final model for this project.



 Pretrained Model (Kaggle)

Due to GitHub file size limitations, the **final trained CNN model** is hosted on Kaggle.

Kaggle Model Link:  
  [https://www.kaggle.com/models/jayindukarunanayaka/suicide-detection](https://www.kaggle.com/models/jayindukarunanayaka/suicide-detection)



 Repository Structure

SuicideWatch-CNN/
│
├── preprocessing/
│   ├── lowercasing.ipynb
│   ├── punctuation_removal.ipynb
│   ├── stopword_removal.ipynb
│   ├── lemmatization.ipynb
│   └── rare_word_removed.ipynb
│
├── models/
│   ├── logistic_regression.ipynb
│   ├── linear_svm.ipynb
│   ├── ann_model.ipynb
│   ├── cnn_model.ipynb
│   ├── BiLSTM_model.ipynb
│   └── GRU_model.ipynb
│
├── results/
│   └── preprocessing_visualizations/
│
└── README.md




 Ethical Considerations & Disclaimer

⚠️ THIS PROJECT IS STRICTLY FOR EDUCATIONAL PURPOSES ONLY.

- This project is intended solely for learning, academic study, and research into NLP, Machine Learning, and Deep Learning.
- The model is **not** a medical or clinical diagnostic system.
- It must not be used for real-world mental health diagnosis, clinical intervention, or definitive suicide risk assessment.
- Model predictions may be inaccurate and should not be treated as definitive assessments of suicidal intent or individual risk.
- Predictions must never replace professional medical or psychological support.

