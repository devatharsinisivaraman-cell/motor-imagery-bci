# 🧠 EEG Motor Imagery Classification using Machine Learning

A Brain-Computer Interface (BCI) project that classifies **left-hand** and **right-hand motor imagery** using Electroencephalography (EEG) signals. This project uses the PhysioNet EEG Motor Movement/Imagery Dataset, extracts statistical features from EEG signals, and applies a Support Vector Machine (SVM) classifier to recognize imagined hand movements.

---

## 📌 Project Overview

Motor Imagery (MI) refers to the mental simulation of a movement without actually performing it. EEG signals recorded during motor imagery contain patterns that can be analyzed to determine whether a subject is imagining moving their left or right hand.

This project demonstrates a complete EEG signal processing pipeline:

- EEG data acquisition
- Signal preprocessing
- Event extraction
- Feature extraction
- Machine Learning classification
- Performance evaluation
- EEG signal visualization

---

## 🎯 Objectives

- Process raw EEG signals.
- Extract motor imagery events.
- Classify left-hand and right-hand imagination.
- Evaluate model performance using machine learning metrics.
- Visualize EEG signals and classification results.

---

## 📂 Dataset

**Dataset:** EEG Motor Movement/Imagery Dataset

**Source:** PhysioNet

**Subject Used:** Subject 1 – Run 4

Task:
- T1 → Left Hand Motor Imagery
- T2 → Right Hand Motor Imagery

Dataset Format:
- EDF (European Data Format)

---

## 🛠 Technologies Used

- Python
- MNE-Python
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## ⚙️ Methodology

### 1. Data Loading

- Load EEG data (.edf)
- Select EEG channels only

### 2. Signal Preprocessing

- Band-pass filtering (1–40 Hz)
- Remove unwanted frequencies

### 3. Event Extraction

Extract motor imagery events:

- T1 → Left Hand
- T2 → Right Hand

Create 4-second EEG epochs for each event.

### 4. Feature Extraction

Statistical features extracted for every EEG channel:

- Mean
- Standard Deviation

These features form the input for the classifier.

### 5. Feature Scaling

Standardize features using StandardScaler.

### 6. Classification

Train an SVM classifier using:

- RBF Kernel
- C = 1
- Gamma = Scale

### 7. Evaluation

Evaluate using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### 8. Visualization

Generate:

- EEG signal plots
- Confusion Matrix
- Precision & Recall bar chart

---

## 📊 Workflow

```

EEG Dataset
│
▼
Load EDF File
│
▼
Preprocessing
│
▼
Event Extraction
│
▼
Epoch Creation
│
▼
Feature Extraction
│
▼
Feature Scaling
│
▼
SVM Classification
│
▼
Prediction
│
▼
Performance Evaluation

```

---

## 📈 Output

The project provides:

- Classification Report
- Confusion Matrix
- EEG Signal Visualization
- Precision & Recall Comparison

---

## 📁 Repository Structure

```

├── EEG_Motor_Imagery_Classification.ipynb
├── README.md

```

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/motor-imagery-bci.git
```

Install required packages

```bash
pip install mne scikit-learn matplotlib seaborn
```

Run the notebook.

---

## 📚 Applications

- Brain-Computer Interface (BCI)
- Assistive Technology
- Wheelchair Control
- Prosthetic Limb Control
- Neurorehabilitation
- Human-Computer Interaction
- Biomedical Signal Processing

---

## 🔮 Future Improvements

- Power Spectral Density (PSD) features
- Common Spatial Pattern (CSP)
- Wavelet Transform features
- Deep Learning (CNN, EEGNet)
- Multi-class motor imagery classification
- Real-time EEG streaming
- Cross-subject evaluation

---

## 📖 References

1. PhysioNet EEG Motor Movement/Imagery Dataset
2. MNE-Python Documentation
3. Scikit-learn Documentation

---

## 👩‍💻 Author

**Deva Dharsini**

Electronics and Communication Engineering Student

Interested in:
- Artificial Intelligence
- Machine Learning
- Biomedical Signal Processing
- Brain-Computer Interfaces
