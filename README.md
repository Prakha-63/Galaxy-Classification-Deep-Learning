# 🌌 Galaxy Morphology Classification using Deep Learning

> A comparative deep learning approach for classifying galaxies as **Round Smooth** or **Barred Spiral** using a Custom CNN and MobileNetV2 Transfer Learning on the Galaxy Zoo dataset.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-red?logo=keras)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📖 Overview

Galaxy morphology provides valuable insight into the formation and evolution of galaxies. Manual classification of large astronomical datasets is time-consuming, making automated classification an important application of deep learning.

This project develops and compares two deep learning approaches for binary galaxy morphology classification using the **Galaxy Zoo** dataset:

- **Custom Convolutional Neural Network (CNN)** built from scratch
- **MobileNetV2 Transfer Learning** using pretrained ImageNet weights

The project demonstrates the complete machine learning workflow, including:

- Data exploration
- Image preprocessing
- Model development
- Training and evaluation
- Error analysis
- Model comparison

---

# 🎯 Objectives

- Automatically classify galaxies into:
  - **Round Smooth**
  - **Barred Spiral**
- Compare a custom CNN against MobileNetV2 transfer learning.
- Evaluate model performance using multiple metrics.
- Analyze misclassified galaxies to understand model limitations.

---

# 🛰 Dataset

**Dataset:** Galaxy Zoo

The dataset contains RGB astronomical images belonging to two morphology classes.

| Label | Galaxy Type |
|--------|-------------|
| 0 | Round Smooth Galaxy |
| 1 | Barred Spiral Galaxy |

The images are stored in HDF5 format and preprocessed before training.

---

# 🧠 Models Implemented

## 1️⃣ Custom CNN

A CNN designed from scratch consisting of:

- Convolution Layers
- Max Pooling
- Global Average Pooling
- Dropout
- Fully Connected Layer
- Sigmoid Output

Purpose:

- Understand CNN fundamentals
- Establish a performance baseline

---

## 2️⃣ MobileNetV2 Transfer Learning

Transfer learning using MobileNetV2 pretrained on ImageNet.

Features:

- Frozen pretrained feature extractor
- GlobalAveragePooling
- Dropout
- Binary classifier head

Purpose:

- Improve generalization
- Reduce overfitting
- Compare against the baseline CNN

---

# 📊 Evaluation Metrics

The models are evaluated using:

- Test Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

The notebook also includes:

- Training Accuracy Curve
- Validation Accuracy Curve
- Training Loss Curve
- Validation Loss Curve

---

# 🔬 Error Analysis

Beyond reporting accuracy, this project investigates model behavior by visualizing:

- Correctly classified galaxies
- Misclassified galaxies
- Prediction confidence
- Possible reasons for incorrect predictions, including:
  - Low image contrast
  - Faint spiral arms
  - Edge-on galaxies
  - Ambiguous morphology

---

# 📈 Model Comparison

The notebook compares the performance of:

| Model | Description |
|--------|-------------|
| Custom CNN | Baseline model built from scratch |
| MobileNetV2 | Transfer Learning model |

Comparison includes:

- Accuracy
- Precision
- Recall
- F1 Score
- Training Time
- Model Complexity

---

# 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- scikit-learn
- h5py
- Jupyter Notebook

---

# 📂 Project Structure

```
Galaxy-Classification-Deep-Learning/

│── README.md
│── LICENSE
│── requirements.txt
│── Galaxy Classification using CNN.ipynb
│── galaxy_classifier.keras

├── images/
│   ├── sample_galaxies.png
│   ├── training_curves.png
│   ├── confusion_matrix.png
│   ├── correct_predictions.png
│   └── misclassified_predictions.png
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Galaxy-Classification-Deep-Learning.git

cd Galaxy-Classification-Deep-Learning
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
Galaxy Classification using CNN.ipynb
```

---

# 📸 Project Highlights

✔ Custom CNN built from scratch

✔ MobileNetV2 Transfer Learning

✔ Binary Galaxy Morphology Classification

✔ Data Visualization

✔ Training Curves

✔ Confusion Matrix

✔ Classification Report

✔ Error Analysis

✔ Model Comparison

---

# 💡 Future Improvements

- Fine-tune MobileNetV2 layers
- Experiment with EfficientNet and ResNet
- Multi-class galaxy morphology classification
- Grad-CAM visualization for explainability
- Deploy as a Streamlit web application
- Train on larger astronomical datasets

---

# 📚 References

- Galaxy Zoo Project
- TensorFlow Documentation
- Keras Documentation
- MobileNetV2 Research Paper

---

# 👨‍💻 Author

**Prakhar Neve**

B.Tech (Computer Science & Business Systems)

Interested in:

- Artificial Intelligence
- Machine Learning
- Computer Vision
- Computational Astrophysics
- Scientific AI

---

# 📜 License

This project is licensed under the MIT License.
