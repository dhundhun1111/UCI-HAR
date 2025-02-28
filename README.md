# Human Activity Recognition (HAR) Using Deep Learning and Machine Learning

This project uses the **UCI HAR Dataset** to classify human activities based on raw inertial sensor data from smartphones. It implements **Deep Learning (CNN, LSTM)** on raw sensor signals and **Machine Learning (Random Forest, SVM, Logistic Regression)** on engineered features extracted using **TSFEL**.

## 📌 Project Overview

### **1. Data Processing & Exploration**
- Load **raw accelerometer and gyroscope signals** from the UCI HAR Dataset.
- Visualize sample signals and class distributions.
- Normalize raw signals using training set statistics.

### **2. Deep Learning on Raw Data**
- Train **1D CNN** and **LSTM** models directly on raw sensor data.
- Evaluate performance using accuracy and confusion matrices.

### **3. Feature Engineering & Machine Learning**
- Extract features using **TSFEL** (Time Series Feature Extraction Library).
- Handle missing values in extracted features.
- Load original **561 precomputed features** provided by dataset authors.
- Train **Random Forest, SVM, and Logistic Regression** on both feature sets.

### **4. Model Comparison & Analysis**
- Compare **Deep Learning vs. Machine Learning** models.
- Compare **TSFEL-generated features vs. original features**.
- Summarize results using tables and bar plots.

---

## 🚀 Installation & Setup

1. **Clone the Repository**
   ```sh
   git clone https://github.com/dhundhun1111/UCI-HAR.git
   cd UCI-HAR
   ```

2. **Install the Required Dependencies**

3. **Run the Jupyter Notebook**
   ```sh
   jupyter notebook UCIHAR.ipynb
   ```

---

## 📊 Dataset
The **UCI HAR Dataset** consists of raw accelerometer and gyroscope signals from a smartphone worn by 30 individuals performing six activities:
- **WALKING**
- **WALKING_UPSTAIRS**
- **WALKING_DOWNSTAIRS**
- **SITTING**
- **STANDING**
- **LAYING**

🔗 **Dataset Source:** [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

---

## 🧠 Models Implemented

### **1. Deep Learning Models (Raw Data)**
✅ **1D CNN** - Convolutional layers extract spatial patterns from time-series signals.  
✅ **LSTM** - Recurrent layers capture sequential dependencies in sensor data.

### **2. Machine Learning Models (Feature Engineering)**
✅ **Random Forest** - Ensemble learning for robust activity recognition.  
✅ **SVM** - Support Vector Machine for feature-based classification.  
✅ **Logistic Regression** - Baseline ML model for comparison.

---

## 📈 Results & Analysis
- **Deep Learning models** achieved high accuracy without requiring feature extraction.
- **Feature engineering with TSFEL** improved ML model performance.
- **Comparison:**
  - CNN performed best among DL models.
  - Random Forest performed best among ML models.
  - TSFEL features were comparable to original features.

📌 **Final Model Accuracies:** _(Replace with actual values)_
| Model               | Accuracy |
|---------------------|----------|
| 1D CNN (DL)        | 93.18%   |
| LSTM (DL)          | 87.98%   |
| Random Forest (TSFEL) | 93.04% |
| SVM (TSFEL)        | 81.30%   |
| Logistic Regression (TSFEL) | 89.38% |

---

## 📜 Repository Structure
```
├── UCIHAR.ipynb        # Jupyter Notebook with full code
├── dataset/    # Dataset directory (downloaded separately)
└── README.md           # Project documentation
```

---

## 📧 Contact
📩 **Subhrajit Deb**  
🔗 GitHub: [dhundhun1111](https://github.com/dhundhun1111)  
📧 Email: subhrajitd28@gmail.com  

---

