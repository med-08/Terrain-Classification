# Terrain Classification

This project focuses on classifying aerial terrain images into four distinct categories — **Desert**, **Forest**, **Mountain**, and **Plains** — using **Convolutional Neural Networks (CNN)**.

[Kaggle Link](https://www.kaggle.com/code/medhavitripathi/terrain-classification/)

[Link to Dataset](https://www.kaggle.com/datasets/krishuppal/terrain-recognition)

The dataset contains **799 images per class** and is structured for use in image classification tasks.

- **Name:** SIH_NN Terrain Dataset  
- **Classes:** `Desert`, `Forest`, `Mountain`, `Plains`  
- **Total Images:** 3,196 (799 per class)  
- **Image Type:** Aerial imagery  

---

## Project Structure

- **Data Preprocessing**:
  - Normalization and rescaling of pixel values (0–1)
  - Image resizing to 128×128
  - Data augmentation using rotation, zoom, and flipping

- **Feature Mapping**:
  - Raw pixel values from RGB channels used as features
  - Image tensors mapped to categorical labels

- **Data Splitting**:
  - Training and validation split (80-20) using `ImageDataGenerator`

- **Model Training using ML Algorithms**:
  - CNN Model:
    - 3 Convolutional Layers + MaxPooling
    - Fully connected Dense layers
    - Dropout for regularization
    - Softmax output layer for classification

- **Model Evaluation and Performance Analysis**:
  - Accuracy and loss curves over epochs
  - Confusion Matrix for class-level performance
  - Classification Report (Precision, Recall, F1-score)

---

## Technologies and Tools

- **Languages**: Python
- **Libraries**: TensorFlow / Keras, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn 
